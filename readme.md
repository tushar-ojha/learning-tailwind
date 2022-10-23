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
    - npm install vite //to open page on live server.
    - "scripts": {"start": "vite"} in package.json
    - npx tailwindcss init to generate tailwind.config.js
    - npx tailwindcss init -p to generate postcss.config.js
    - Create input.css file, link it into HTML file.
      - Write @tailwind base; @tailwind components; @tailwind utilities;
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
      - divide-width; to put border in child elements.
   - ### Square bracket notation to give custom values.
      - my-[67px] pd-[44rem]
   - ### Responsiveness
      - sm md lg 2xl xl:bg-blue-200 boom! Work done!
      - text-base default font size.
      - MOST IMPORTANT THING: Follow mobile-first approach. We need to think in this way. Smallest screen will use default classes, then I will keep increasing size of screen and keep on overriding my classes.
      - class="hidden" is display: none. block to take it back.
   - ### Hover, focus and other states:
      - hover:bg-purple-700
      - focus: when element is selected to receive input while active when it is activated by user. Stack overflow has beutiful answer for this.

   - @apply directive. 
      - .btn { @apply ...tailwind classes... }; giving short name, sort of variable to large lines of CSS.

   - Specificity in style.css. If we want our CSS to be fetched first then we put it before @tailwind utilites. We generally keep our CSS before @tailwind utilities. We should handle this based on our requirement.

   - @layer components {....css classes and properties.....} will add CSS afer component layer. We mention the layer after which we want to add our CSS.

   - @layer utilities  {....css classes and properties.....}; classes in this will be considered as utility classes. 
   - ### layering in tailwind needs more attention of mine.
      - @layer directive comes with some cost, so we should use it only if it is really important. Cost is we need to go multiple times to CSS file in case of debugging.
   - ## npx tailwindss init tushar 
      - --full will generate a full configuration file. This will act as a reference file to edit tailwind.config.js. We can know where we have add our custom changes.

   - Build breaks when we don't have relative URL.
   - Deploying on production
      - Inside scripts of package.json "build": "vite build" then npm run build/ output is the production build.


   

