# User Manual





## Standard Render Pipeline

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
<img src=".\Images\Usage\urp_usage1.png" align="middle" width="50%"  />

2. After creating and loading, you will be at "SampleScene" by default. If not then find it at "Assets/Scenes/SampleScene.scene" and open.

3. Import URP unitypackage. There are two ways:
  - Click through "Assets > Import Package > Custom Package..." and select package to import.
  - Or directly drag the package into project window.
4. Open demo scene at "Assets/Z-PostProcessing/Demo/DemoScene.unity".



#### Getting Started (2019.4.X or above)

1. Find and click "Assets/Settings/ForwardRenderer" file in project then view it at Inspector window.
<img src=".\Images\Usage\urp_usage2.png" align="middle" width="50%"  />

2. Click “Add Renderer Feature” button at bottom. You can select the effects you want in the pop-up menu and add it. Then you will see some cool effect in the Scene and Game window. Run your game to view real-time effects.

3. Take “Bokeh Blur” for example, you will see this component after you add this feature. Except for "Shader" and "Render Pass Event", each parameter is configurable as you wish.
<img src=".\Images\Usage\urp_usage3.png" align="middle" width="50%"  />



#### Getting Started (2019.3.X)

1. Find and click "Assets/Settings/ForwardRenderer" file in project then view it at Inspector window.
<img src=".\Images\Usage\urp_usage2_2019_3.png" align="middle" width="50%"  />

2. Click “+” button at bottom. You can select the effects you want in the pop-up menu and add it. Then you will see some cool effect in the Scene and Game window. Run your game to view real-time effects.

3. Take “Glitch RGB Split” for example, you will see this component after you add this feature. Except for "Shader" and "Render Pass Event", each parameter is configurable as you wish.
<img src=".\Images\Usage\urp_usage3_2019_3.png" align="middle" width="50%"  />







## High Definition Render Pipeline (HDRP)

#### Installation & Getting Started

1. Create a new HDRP project
<img src=".\Images\Usage\hd_usage1.png" align="middle" width="50%"  />
2. After creating and loading, you will be at "SampleScene" by default. If not then find it at "Assets/Scenes/SampleScene.scene" and open.
3. Import URP unitypackage. There are two ways:

  - Click through "Assets > Import Package > Custom Package..." and select package to import.
  - Or directly drag the package into project window.

4. Open "Project Settings" window through "Edit > Project Settings".
<img src=".\Images\Usage\hd_usage2.png" align="middle" width="50%"  />
5. Open "HDRP Default Settings". Find "+" button below "Before Post Process" or "After Post Process" and click it to add all Z Post-processing effects.
<img src=".\Images\Usage\hd_usage3.png" align="middle" width="50%"  />
6. Find and click “Post Process Volume” in sample scene.
<img src=".\Images\Usage\hd_usage4.png" align="middle" width="50%"  />
7. Click "Add Override" button at bottom and select one effect of Z post-processing you want.
<img src=".\Images\Usage\hd_usage5.png" align="middle" width="50%"  />
8. Take "Glitch Analog Noise" for example, you will see this component after adding. You can tune parameter to get the effect you need. (Note: the feature you add will not take effect immediately. You need adjust at least one parameter then run your game to preview the effect.)
<img src=".\Images\Usage\hd_usage6.png" align="middle" width="50%"  />



If you want to know more about post-processing stack in HDRP, please refer to:

[Post-processing in the High Definition Render Pipeline](https://docs.unity3d.com/Packages/com.unity.render-pipelines.high-definition@6.9/manual/Post-Processing-Main.html)



Enjoy it. :D









































