# User Manual





## Build-in Render Pipeline (BRP)

#### Step 1. Create or open a Unity Project

<img src=".\Images\Usage\usage1.png" align="middle" width="50%"  />

#### Step 2. Install PPv2

Z Post-processing requires Unity PPv2 package. So make sure you install the PPv2 package in the Package Manager before you import this one. If you do not know how to install PPv2, please refer to [Post-processing stack v2 - Installation](https://docs.unity3d.com/Packages/com.unity.postprocessing@3.1/manual/Installation.html)

#### Step 3. Import this package and open the demo scene

The location of the demo scene: Assets/Z-PostProcessing/Demo/DemoScene.unity

The usage of Z Post-processing in build-in pipeline is the same as the Unity PPv2 (Post-processing stack v2). If you do not know how to use it, please refer to [Getting started with post-processing](https://docs.unity3d.com/Packages/com.unity.postprocessing@3.1/manual/Quick-start.html)









## Universal Render Pipeline (URP)



#### Installation


1. Create a new URP project
<img src=".\Images\Usage\usage1.png" align="middle" width="50%"  />

2. After creating and loading, you will be at "SampleScene" by default. If not then find it at "Assets/Scenes/SampleScene.scene" and open.

3. Import URP unitypackage. There are two ways:
  - Click through "Assets > Import Package > Custom Package..." and select package to import.
  - Or directly drag the package into project window.
4. Open demo scene at "Assets/Z-PostProcessing/Demo/DemoScene.unity".



#### Getting Started (2019.4.X or above)

1. Find and click "Assets/Settings/ForwardRenderer" file in project then view it at Inspector window.
<img src=".\Images\Usage\usage2.png" align="middle" width="50%"  />

2. Click “Add Renderer Feature” button at bottom. You can select the effects you want in the pop-up menu and add it. Then you will see some cool effect in the Scene and Game window. Run your game to view real-time effects.

3. Take “Bokeh Blur” for example, you will see this component after you add this feature. Except for "Shader" and "Render Pass Event", each parameter is configurable as you wish.
<img src=".\Images\Usage\usage3.png" align="middle" width="50%"  />



#### Getting Started (2019.3.X)

1. Find and click "Assets/Settings/ForwardRenderer" file in project then view it at Inspector window.
<img src=".\Images\Usage\usage2_2019_3.png" align="middle" width="50%"  />

2. Click “+” button at bottom. You can select the effects you want in the pop-up menu and add it. Then you will see some cool effect in the Scene and Game window. Run your game to view real-time effects.

3. Take “Glitch RGB Split” for example, you will see this component after you add this feature. Except for "Shader" and "Render Pass Event", each parameter is configurable as you wish.
<img src=".\Images\Usage\usage3_2019_3.png" align="middle" width="50%"  />







## High Definition Render Pipeline (HDRP)

1. 新建一个HDRP项目
<img src=".\Images\Usage\hd_usage1.png" align="middle" width="50%"  />

2. 等新建好项目后应该就默认在SampleScene了，如果不在的话在Project窗口中找到Assets > Scenes > SampleScene并打开

3. 导入Z-PostprocessingHDRP的unitypackage，有两种导入方法

  - 点击菜单Assets > Import Package > Custom Package... 选择package并导入
  - 或者，直接将package文件拖入到Project窗口中导入

4. 打开Project Settings窗口 Edit > Project Settings
<img src=".\Images\Usage\hd_usage2.png" align="middle" width="50%"  />
5. 点击"HDRP Default Settings"，在此页面最下方的“Before Post Process”或“After Post Process”通过点击加号“+”按钮添加Z-PostProcessing的所有效果
<img src=".\Images\Usage\hd_usage3.png" align="middle" width="50%"  />
6. 在SampleScene的“Hierarchy”界面找到“Post Process Volume”并点击
<img src=".\Images\Usage\hd_usage4.png" align="middle" width="50%"  />
7. 点击“Inspector”界面最下方的“Add Override”按钮，在菜单中选择“Z-PostProcessing”的选项添加所需的效果
<img src=".\Images\Usage\hd_usage5.png" align="middle" width="50%"  />
8. 以“Glitch Analog Noise”效果为例，添加后会出现这样的组件，调节属性达到你想要的效果（注：添加后效果并不会立即生效，需要先调节默认开启的属性并运行游戏来预览效果）
<img src=".\Images\Usage\hd_usage6.png" align="middle" width="50%"  />



关于HDRP中的后处理栈介绍：

[Post-processing in the High Definition Render Pipeline](https://docs.unity3d.com/Packages/com.unity.render-pipelines.high-definition@6.9/manual/Post-Processing-Main.html)













































