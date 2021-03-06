# 智能毕业纪念相册    

| 发布日期        | 2019/12/10    |     
| --------   | -----:  | 
| 项目名称        | 智能毕业相册     |
| 项目现状        | 进行中       |
| 项目所有者        | 余杭宏      |
| 项目设计师        | 余杭宏      |
| 项目开发者        | 余杭宏      |
| 项目测试者        | 余杭宏      |


##  背景
-  学生毕业时都会留有一本毕业纪念册，但纸质版的毕业纪念册并不能持续更新，毕业生们可能多年之后留在毕业纪念册上的信息都会有所变更，导致无法联系上老同学，而且目前相册类应用的功能多以存储、分类、加密、分享为主，无法实现与现状信息相同步更新。

##  产品介绍-加值宣言
-  智能毕业纪念册APP采用阿里云API的人脸识别，提取图像中的人脸五官关键点，输出关键点位置信息，可毫秒级识别人脸105个关键点定位。在APP中输入一张照片，即识别的主体，基于图像或视频输入进行检测，与注册库比对，输出识别主体用户自身所输入更新的信息。

##  核心价值宣言  
-  毕业纪念相册APP的核心价值是解决用户无从得知老同学当前现状的联系方式，不再让毕业纪念相册只是徒留念想的作用。

##  目标用户  
-  各阶段的毕业生
-  老师、辅导员

##  用户痛点
-  当看回毕业纪念相册时无法得知现在的联系方式
-  想寻找关于某个人的全部照片，但照片较多的话可能会有所遗漏   




##  AI概率性考量

-  人脸识别API：     
1.人脸检测定位：识别图像中是否有人脸并给出人脸区域，进行人脸检测后返回检测到的人脸矩形框坐标，可支持最多上千个人脸的同时检测，支持平面360度旋转人脸检测，支持左右最大90度侧面人脸检测。      
2.人脸特征定位：提取图像中的人脸五官关键点，输出关键点位置信息。可毫秒级识别人脸105个关键点定位(眉毛24点，眼睛32点，鼻子6点，嘴巴34点，外轮廓9点)。    
应用场景：可为人脸美化/美妆、人脸认证、检索、3D人脸等功能提供基础信息。    
3.人脸属性识别：在人脸检测基础上，识别各个检测人脸的性别（男/女）、年龄、表情（笑/不笑）、眼镜（戴/不戴）四种属性；同时可返回人脸的1024维深度学习特征，基于这个特征并按照我们给出的特征比较规则，用户可实现高性能的人脸识别。    
4.人脸查找：基于图像或视频输入进行检测，与注册库比对，实现1：N的人脸识别。    

-  可能发生的问题
1.图片过于模糊无法识别人脸     
2.所输入的图像人脸过多，输出过多的用户导致混乱    

###  需求优先级
| 用户        | 使用场景    | 用户需求    | 重要程度     |
| --------   | -----:  | :----: | :----: |
| 毕业生        | 联系老同学聚会      |  寻找老同学的联系方式     | 重要    |
| 毕业生或老师       | 回忆照片    | 想要观看其他同学的毕业纪念照片    | 次重要     |

##  产品框架图   

![架构图](https://images.gitee.com/uploads/images/2019/1224/154109_404239ec_1648172.png "屏幕截图.png")


