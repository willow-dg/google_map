# 2025年12月15日

## API教程
- today，尝试googleMap的一些实例调用API 
## 地图基础
- begin,很显然手动编写会造成一些不易发现的贫血错误，
- In addition，尝试使用googleMap的API，但是没有成功，
- A case in point is that,成功了，尝试内地网络-不可以；
- As a matter of fact,我尝试可google地图的四种类型。
## 地图叠加层
1. 添加标记
- 我发现一个Marker对象只能添加到一个地图对象中，不能添加到多个地图对象中。
2. 跳动的标记
- 是的，调用API的时候又有拼写错误BOUCE(BOUNCE)跳动的标记
3. 自定义标记
- AND SO ON，又发现一个自定义标记，只能选择网络图标，不能选择本地图标
4. 添加路径
- 创建路径(Polyline)坐标点,赋值符号"=";而不是":",适用于标签语句
5. 添加多边形
6. 添加圆
7. 添加信息窗口
## 地图事件
1. 点击标记缩放地图
- 添加不了事件?又是拼写错误addListener
- 还有就是addListener已经弃用了,还是能用的.也许随时就停用了
2. 重置标记
- I am understanding.就是返回中心点center,当然缩放级别不会变回来
- good,没为题
3. 点击时打开信息窗口
- 将infowindow.open(地图实例,锚点对象)移入点击事件中，就可以实现点击时打开信息窗口了
4. 设置标记及打开每个标记的信息窗口
- addListener(对象实例、事件名称、出发事件调用函数)
- 又是一个调用函数拼写错误，var可以重复声明
## 地图控件集
1. 默认控件集设置
- Zoom显示一个滑动条来控制map的Zoom级别
- PPan地图上显示的是一个平底碗样的控件，点击4个按钮，可以平移地图
- MapType允许用户在map types(roadmap和satellite)之间切换
2. 更多控件集
- Scale显示地图比例尺
- Rotate显示一个小的圆周坐标，可以转动地图
- verview Map从广域视角俯视地图
> 这些控件集可以通过setOptions(控件集名称,true)改变。
3. 地图关闭默认控件集
- disableDefaultUI:true
- 我又懂了，添加属性时，应该注意分割“,”否则加载不出来。
4. 开所有控件集
- 有些控件集似乎不能打开
5. 修改控件集
- 有些控件集也用不了
# 一些基础知识：
- API “应用程序编程接口（Application Programming Interface）”
- API 也就是操作系统留给应用程序调用执行功能的接口