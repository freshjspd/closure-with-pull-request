Client:
- совместимость браузеров: new node v => babel => old node v  - babel
- разрешение импортов (нестандартных)      - webpack loader (npm i -D css-loader style-loader, ...)
- транспайлинг js (babel)                  - webpack loader (npm i -D babel-loader)
- + сборка и минификация                   - webpack
- горячая перезагрузка                     - webpack plugin (webpack-dev-server)
- + автосоздание html и подвязка к нему js - webpack plugin (html-webpack-plugin)
  
1. npm install webpack webpack-cli --save-dev  
loader (babel, scc, images) - резолв импорта и преобразование файлов
plugin (hot reload, ... )   - различные другие задачи