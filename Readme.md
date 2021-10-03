# Don't have an iPhone 13 ? How about making it with Tailwind ourselves?
This repo followed [Rebuilding iOS 15 with Tailwind CSS](https://www.youtube.com/watch?v=eSzNNYk7nVU&list=WL&index=1&t=144s) from [Tailwind Lab](https://www.youtube.com/channel/UCOe-8z68tgw9ioqVvYM4ddQ).

## Steps to setup dev environment:
1. Init a node frontend project in root folder. `-y` stands for "yes for all questions throughout the steps"  
   ```shell
   npm init -y
   ```  

2. Install dev-dependency packages. `vite` is a dev server to host our frontend at some port.
   ```shell
   npm install -D tailwindcss postcss autoprefixer vite
   ```
   We need also goto **package.json**, add `"dev":"vite"` for later usage.

3. Generate tailwind requisite config files. `-p` for "please create files for postcss framework". This generates **tailwind.config.js** and **postcss.config.js** files for us.
   ```shell
   npx tailwindcss init -p
   ```

4. Run vite to host our frontend under dev environment.
   ```shell
   npm run dev
   ```


