<h1> git clone 後</h1>
  移動到 node_modules
  啟動 node index.js  然後開啟http://localhost:3000 可以發現簡易聊天室
<h2> 伺服器部分寫在 Socket.io/node_modules/index.js </h2>
  伺服器寫在 index.js，應用到HTTP伺服器、Socket.io應用(用於通訊)
<h2> 客戶端寫在 Socket.io/node_modules/views/index.html </h2>
  用到CSS布置介面，基本HTML標籤，js socket.io 客戶端的應用
  主要是有連到伺服器才會啟用js的函數
<h3> node.js 安裝的套件 </h3>
  npm install -S express socket.io
  express  建立HTTP伺服器
  socket.io 加入socket.io在 server上
<h3> 注意事項 客戶端js 第81行可以改用CDN的socket.io URL </h3>
https://cdnjs.cloudflare.com/ajax/libs/socket.io/2.2.0/socket.io.js
<h3> 啟動伺服器後 </h3>
可以連接的URL為 http://localhost:3000 預設為3000埠號和
http://192.168.1.103:3000 (IPV4+埠號) 這個是內部網路的人也可以連到，只要打上IPV4+埠號
以上都可連到聊天室
