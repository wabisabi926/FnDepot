<p>✉️一个基于Node.js + Redis构建的现代化、高颜值、重隐私的智能挪车通知系统。</p><p>⭐使用说明：安装后打开进入/admin管理后台，添加车主信息和配置通知推送，可参考<a href="https://github.com/nbbk/MoveCar-Docker-NB" target="_blank">官方文档</a></p>
系统部署成功并绑定域名后，不同身份的访问入口如下：

    🔒 管理后台：https://你的域名/admin (输入授权码登录，管理全局配置和车主)
    📱 呼叫车主页 (扫码端)：https://你的域名/?u=用户标识
    👨‍✈️ 车主处理页 (接单端)：https://你的域名/owner-confirm?u=用户标识
    🖨️ 挪车海报生成页：https://你的域名/qr?u=用户标识 (手机端左右滑动挑选样式并保存)

