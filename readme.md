# REPEATITION IS THE MOTHER OF LEARNING!

## Getting  started with Tailwind CSS.

Why Tailwind?
 - No reinventing of class names required.
 - crisp syntax and intuitive syntax.
 - Responsiveness: We can add different classes for different breakpoints on same element.
 - Seems like inline CSS only. Big No. These utility classes are well researched. Values, unit, preciseness we don't need to care much. 

 Setup:
 - Use Play CDN to play. Won't work in production.
 - mx-4 mx-2 cursor-pointer px-4 py-4 bg-purple-900 font-sans, pt means padding top.
  This is how we write classes inside elements and boom! CSS is applied. No need to remember anything. A secret extension will do this for us.
 - Remeber to use vite instead of using live server.

 - Commands to install and run tailwind properly
    - npm init -y skips all questions and directly generates an package.json file.
    - npm install -D tailwindcss postcss autoprefixer
    - npm install vite //to use tailwind in production.
    - "scripts": {"start": "vite"} in package.json
    - npx tailwindcss init to generate tailwind.config.js
    - npm tailwindcss init -p to generate postcss.config.js
    - Inside tailwind.config.js * in content:[] like this: content:["*"]
    - tailwind css intellisense extension in VS code.
    - npm run start will start website on local host.
    - Control + space bar if suggestion doesn't appear.

 - Search landing page templates to practice CSS or tailwind.

 - Even h1 tag results in small font-size. We need to use tailwind utility classes.

 - Popularly used classes:-
   - rounded-3xl to put border radius on image.
   - flex to make any div flexbox.
   - px-3 py-4 pt pb, pl, pr, pt to add padding, similary margin is added.
   - cursor-pointer.
   - bg-purple-400 //400 for level of darkness.
   - text-3xl is for font-size.
   - h-44 for height. 
   - w-10 for width.
   - text-white for color or font-color.
   - hover:text-black-400 for pseudo classes.
   - content-center is equal to align-content: center of flexbox.
   - justify-around for space-around
   - font-bold / font-extrabold.
   - border-purple-900
   - hr in css gives us a horizontal line.
   - font-serif, font-sans.
   - ### Protip: Search will css classes name in tailwind official site.
   - ### Margin Borders and Padding:
      - m-0 mx-0 my-0 mt mr ml mb, negative values are also allowed.
      - space-between; very important class, puts margin in all the child elements. Very helpful in case of navbar.
      - divide-width to put border in child elements.
   - ### Square bracket notation to give custom values.
      - 

