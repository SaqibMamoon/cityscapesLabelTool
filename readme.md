# 图片标注工具使用说明及标注规范
1. 标注工具提供两个版本，Windows版和Linux版
2. 标注工具 **一定必须放在英文路径，英文路径，英文路径** 下哦，并且 **不要修改文件名，不要修改文件名**，否则它会耍赖。

## 一、标注工具使用说明
 Windows版和Linux版的使用方法是一样的。主要的不同点在于：  
 1. Windows用户可直接双击 **`cityscapesLabelTool.exe`** 运行   
 2. Linux用户需要通过以下两种方式运行：    
 >   A、切换到 **`cityscapesLabelTool.py`**脚本所在目录，在终端运行：```python cityscapesLabelTool.py``` [enter]   
 >   B、使用IDE打开脚本，点击运行即可。     

### 打开文件
> 有两种方式，程序启动时和程序运行时    

#### 1. 启动程序会弹出文件选择对话框，选择图片所在的目录（Linux用户还可以设置环境变量 *CITYSCAPES_DATASET* ，必须是包含png图片的目录，否则会出错）
#### 2. 程序运行时，点击左上角的打开文件按钮（Windows用户的‘打开’），然后弹出文件夹选择框。如下图，我的图片放在**testImgDir**目录下：
![打开文件夹](https://i.imgur.com/HgEF5pq.png)

### 标注图片
标注图片分为以下几步：     
#### 1. 选择区域
  > 当选择了图片所在的文件夹后，程序自动加载该文件夹下的所有png图片。使用鼠标点击图片会绘制一个锚点，当形成一个闭环时，点击从左到右第8个图标或者**快捷键 N**会弹出标签选择框，有三种标签（static，sidewalk，road），根据实际道路类型，打上 **sidewalk**或 **road**标签，然后点击ok就为这块区域打上标签啦，可以看到颜色也会有变化。      
  
  ![](https://i.imgur.com/JSiINvg.png)

#### 2. 修改区域
  > 当选择的区域不当时，可以通过拖动 **锚点** 来修改区域，在绘制过程中，若不小心打错了锚点，可按快捷键 **回退** 取消上一步操作。    
  > 若要清除当前的形状，可使用快捷键 **ESC** （已经打上标签的不会被清除）。

### 保存
1. 所有区域都正确标记之后，可使用快捷键 **S**保存或者鼠标点击工具栏的保存图标（Windows用户是‘保存’按钮）。    
2. 保存之后，可使用键盘上的左右键切换图片，也可以点击工具栏的左右图标。 

----------

## 二、图片标注规范
### 1. 图片标注目前只有两类标签：**sidewalk**和 **road**，对于每一个区域都要打上正确的标签。  
 > road：能走车的道路统一归为 road    
 >sidewalk：除了road之外能走人的道路都归为 sidewalk，注意在标注是不要把台阶囊括进可行区域中。     
 
### 2. 天桥、楼梯等，人虽然能走，但不需要标记。
### 3. 马路的花坛、路肩标记在内侧（详见样例1）。
### 4. 如果有多个区域不连续的，需要将所有区域都标记并打上正确的标签。
### 5.标注完成之后，千万记得要保存，要保存，保存。

##### 样例1、边缘的标记：     
![](https://i.imgur.com/HSMF4XU.png)
##### 样例2：标注后结果
![](https://i.imgur.com/JaEZIyt.gif)
 
##### 标注示例：    
![](https://i.imgur.com/E8Emaq6.gif)

## 三、实习要求及津贴支付方式
### 1、实习要求
1. 以实习生身份，通过QQ群（唯一指定群号：643262482）领取当日标注任务，根据标注要求进行图片标注。
2. 标注结果需要相应人员检验，验收通过的图片按计量方式支付相应津贴（0.5元人民币/张）

### 2、津贴支付方式
1. 津贴的支付方式为：通过QQ红包派发


##### 若有任何疑问，欢迎随时在群里提出，我们会及时解决。