# 毕业纪念手册的需求文档
Target release|2019年12月30日
-|-|
Epic	|智能毕业纪念册
Document status|已开始
Designer	|黄雨婷
Developer|黄雨婷
## 价值主张设计
### 产品定位
本产品作为一个以分享照片、视频为主的平台，为准毕业生提供往年毕业季的热门拍照地点，为不懂拍照和不懂摆姿势的准毕业生提供热门毕业照作为拍照灵感，为已毕业并打算重返母校的用户找到老照片中的地点。
### 加值宣言
1. （核心）百度图像识别api：
- 通过百度图像识别，设定定制化识图，将校园地标信息收集整理，集成于该识图小程序中。用户不需要到处打听，只需要输入带有校园地标的照片，便可得知照片中的拍摄地点。用户不知道在哪里拍毕业照时，该平台通过地标识别给用户上传的照片进行自动标记、分类而整理排序出热门地标排行榜，为用户解决了“不知道去哪里拍毕业照”的烦恼，同时，用户可以轻松地了解拍毕业照时与校内热门地标的合照姿势，拍出好看不僵硬的照片

2. （辅助）高德路径规划api：
- 为用户规划一条距离目的地最近的路线，用户可以轻松地找到照片中地标的所在位置

### 核心价值
识别用户上传的照片的校内景物，并按地标进行分类，为用户展示校内各个地标范围内校友们留下的照片。

### 用户痛点
- 用户不知道校内哪个地方适合拍毕业照，哪个地方必须打卡
- 用户面对镜头时肢体表情都很僵硬，不知摆何姿势
- 用户对某地标所在位置、到达路线不熟悉，用户需要打听才可得知路线

### AI概率性考量
![](https://upload-images.jianshu.io/upload_images/9457515-9be26c9ff59d329d.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
虽能识别中山大学，但未能实现更进一步的地标识别——“铜像”，需要进行定制化识图

### 需求列表与人工智能API加值
用户案例 | 重要性 |  笔记  | 技术
-|-|-|-
户不知道校内那个地方适合拍毕业照，哪个地方必须打卡 | 非常重要 | 核心功能，要求对照片内地标识别的准确性 | 百度AI图片识别api
某地标不属于用户的活动区域，用户需要打听才可得知路线 | 重要 | 辅助功能，为用户提供到达目的地的线路 | 高德路径规划api |

### 一句话版本价值主张
本产品作为一个以分享校园照片为主的平台，对用户上传的照片进行地标识别并标记分类，便利用户查看校园内热门打卡地点及照片。并且，用户只需上传带有地标照片，就可以通过地标识别，返回地标信息，还可以用路径规划，给用户带路。

### 一分钟版本价值主张
本产品通过百度图像识别，设定定制化识图，将校园地标信息收集整理，集成于该识图小程序中。用户不需要到处打听，只需要输入带有校园地标的照片，便可得知照片中的拍摄地点，并通过路径规划，找到定位所在位置到目标地标的最佳路径。用户不知道在哪里拍毕业照时，该平台通过地标识别给用户上传的照片进行自动标记、分类而整理排序出热门地标排行榜，为用户解决了“不知道去哪里拍毕业照”的烦恼，并且，用户可以在平台内查看经过图片识别而自动精确分组好的地标相册，轻松地了解其他校友拍毕业照时与校内热门地标的合照姿势，为用户提供拍照灵感，拍出好看不僵硬的照片。
