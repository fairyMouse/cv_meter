# cv_meter
canvas表盘组件
demo演示地址：https://fairymouse.github.io/cv_meter/cv_meter.html

可传参数：

  1.percent：初始动画过渡到的位置，范围0到1，默认0.6
  
  2.start_color：动画起始位置的渐变色，十六进制颜色，默认#FFA933
  
  3.end_color：动画结束位置的渐变色，十六进制颜色，默认#FF4B31
  
  4.r：表盘内圆的半径，单位px，默认200；canvas的大小是根据r的大小变化的
  
  5.degree：总刻度，默认100
  
  6.segment：表盘分段数，默认为4
  
  
对外方法：
  
  1.cv_meter.setValue(刻度值)：改变动画过渡的目标点，范围在0-总刻度之间
  2.这样写配置
  var cv_meter = sg.Component.CvMeter($('#app'), {
    percent:0.4 ,
    start_color:'#FFA933',
    end_color:'#FF4B31',
    r:200,
    degree:1000,
    segment:4,
  });
