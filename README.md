# father
父亲节海报活动
在 http://www.cnblogs.com/strick/p/5593166.html 有具体介绍

当前代码存在BUG，最简单的解决方案index.html中屏蔽hidpi-canvas.js 引入，并且build index.buldle.js中255优化  
canvas.width = $frame.width() * window.devicePixelRatio;//$frame.width();
canvas.height = $frame.height() * window.devicePixelRatio;//$frame.height();

344行新增：var pr = pr * window.devicePixelRatio;  以解决屏幕像素问题和清晰度，目前测试6s、8均正常清晰
