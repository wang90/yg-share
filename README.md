## 阳光志愿者数据统计年度总结h5分享页面

利用 Discuz数据统计参与活动链接shengchengapi  

#### 前端：jquery + html2canvas.js
实现方式   
通过html2canvas生成图片    
网站http://html2canvas.hertzen.com/    

``````
// 主要功能

html2canvas(document.querySelector("#showShare"),{
    useCORS: true,
    height: $("#showShare").outerHeight()
  }).then(canvas => {
    canvas.setAttribute('id','canvas');
    document.body.appendChild(canvas);
    getImg();
});

``````
