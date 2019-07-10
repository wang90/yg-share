# ygShare
h5 分享页面
通过html2canvas生成图片
网站http://html2canvas.hertzen.com/

``````
html2canvas(document.querySelector("#showShare"),{
    useCORS: true,
    height: $("#showShare").outerHeight()
  }).then(canvas => {
    canvas.setAttribute('id','canvas');
    document.body.appendChild(canvas);
    getImg();
});
``````
