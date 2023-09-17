new node v => babel => old node v  
  
old node v:    
  nvm install 12  
  
1. npm install --save-dev @babel/core @babel/cli  
npx babel src -d build => equel map

2. configure babel  
plugin
preset = many plugins
babel.config.json:
{
  "presets": ["@babel/preset-env"]
}

"build": "babel src -d build",
npm install --save-dev @babel/preset-env  

3. for server:
npm i -D @babel/node
"babel-node": "babel-node --presets=@babel/preset-env",
"start": "nodemon --exec npm run babel-node -- ./src/index.js"
