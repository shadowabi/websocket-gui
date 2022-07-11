# websocket-gui
websocket客户端的gui，以及云函数版本



## Usage

websocket.html版本，双击打开即可使用，若出现socket连接失败，则有可能是由于本地打开，导致http发送请求时header中的origin为null所引起的，此时可搭建http服务，将websocket.html以web网站的方式访问即可

基于此，可采用云函数的方式搭建，即使用websocketSCF.py：新建云函数，选择空白函数-python3.7（3.6），将scf文件内容全部粘贴进去，函数勾选集成响应即可
