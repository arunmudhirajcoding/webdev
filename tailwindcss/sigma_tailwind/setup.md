## How to setup Tailwind CSS v3

Step 1: Run the following commands

``` 
npm install -D tailwindcss@3.4.17 postcss autoprefixer vite (-D for dev dependecies)
npx tailwindcss init -p (for postcss config)
```

Step 2: Update tailwind.conf.js file to include this line:
```
content: ["*.html"], (to watch all html files in current folder)
```

tip when using react put
```
 content: ["./src/**/*.{html,js}"],
```

Step 3: create src/input.css or just main.css in root directory to include:
```
@tailwind base;
@tailwind components;
@tailwind utilities;
```

Step 4: Include the src/output.css file to your html

Step 5: Run the following command:
```
npx tailwindcss -i ./src/input.css -o ./src/output.css --watch
```

step 6: add script in package.json

```
"scripts": {
    "start": "vite"
  }, (for normal configuration)
```


## how to setup tailwindcss v4

step 1: run the following commands in terminal 
```
npm create vite@latest
```

step 2: follow the tailwindcss official installation doc