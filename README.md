# htmlChangePic
a part of html can be translated to a picture
# preview
you should run this project in the service, or you can not see what you expect
# changeLog
## To update the latest version of html2canvas
If you use HTML that contain the CSS （overflow:hidden），it can‘t screenshot the outside of view. The best way is using the latest version of html2canvas.
There's two demo with the latter one and the older one.
若需要截图的部分含有overflow：hidden，或者结构复杂，优选最新版本的html2canvas
## question
* 图片无法显示（pictures not display）
  - 图片是否跨域picture Cross domain?（solved：useCORS: true）
  - 前后是否使用了overflow包裹 use "overflow:hidden"（solved：使用新版本use new version）
* 生成图片的比例小于正常比例（The proportion of the generated pictures is less than the normal proportion）
  - 查看设备像素window.devicePixelRatio是否为1
  - window.devicePixelRatio = window.devicePixelRatio > 1 ? 1 : 1;
