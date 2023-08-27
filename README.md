# TailwindCSS-Steps
Steps to setup TailwindCSS using Tailwind CLI

1.Install Node.js


2.Create 2 files 'dist' and 'src'

  dist > index.html
  
  src > input.css
  
  
3.Open terminal and run the following code:

  npx tailwindcss init - creates 'tailwind.config.js'
  Add the paths to all of your template files in your tailwind.config.js file.
    
    /** @type {import('tailwindcss').Config} */
      module.exports = {
    content: ["*"],
    theme: {
    extend: {},
    },
    plugins: [],
    }
  
4.src/input.css

  @tailwind base;

  @tailwind components;
  
  @tailwind utilities;
  

5.Start the Tailwind CLI build process

  npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch


6.Start using Tailwind in your HTML

  link the stylesheet to the HTML file

  
