# RemoteCamera
通过USB-PTP协议，远程控制相机
# 说明
> [原项目地址](https://github.com/duwurensheng010/remoteyourcam-usb) 非常感谢前辈留下的资源！此项目仅做学习交流，不可直接商用。
- 由于原项目不是AndroidStudio创建的，这里是把原项目的代码提取出来。 实测可以通过USB进行远程拍摄、图片获取资源。
- 项目中所使用的指令，皆需和 [佳能](https://www.canon.com.cn/) 、 [尼康](https://www.nikon.com.cn/sc_CN/) 签署协议。
- 如有侵权相关问题，请联系作者。
# 注意
- 相册默认读取的是卡2的资源，如果出现打开崩溃情况，可以修改[GalleryFragment](https://github.com/NightRainDream/RemoteCamera/blob/master/app/src/main/java/com/remoteyourcam/usb/view/GalleryFragment.java)类中，`onAllStoragesFound()`方法中修改默认SD卡的的位置
- 项目中继承比较多，需要耐心看看，不是很复杂。
- 原图获取项目中做了缩放处理，注意 `GetObjectCommand` 类中的 `BitmapFactory.Options options` 参数。
# 特征
- 拍摄照片
- 查看您拍摄的照片
- 显示当前曝光模式
- 灯泡拍摄（仅限佳能）
  - 实时取景
  - 直方图（仅限佳能）
  - 驱动焦点
  - 在实时查看模式下可调整拍摄图片的持续时间
- 在活动实时视图中缩放和平移
- 具有全屏图片查看、缩放和平移功能的图库
- 图片流显示捕获的图片
- 控制以下属性：
  - 白平衡
  - 快门速度
  - 等灵敏度
  - 光圈优先
  - 色温
  - 自动对焦测光模式（仅限尼康）
  - 设置对焦点（仅限尼康）
  - 在实时取景中设置对焦矩形（仅限尼康）
  - 曝光补偿
# 友情连接
- [佳能](https://www.canon.com.cn/supports/sdk/icp/)
- [尼康](https://www.nikon.com.cn/sc_CN/)
