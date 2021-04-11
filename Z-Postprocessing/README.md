# User Manual

**CONTENT**

- Guide (Standard RP)
- Guide (URP)
- Guide (HDRP)
- Glitch Effects



## Guide (Standard RP)

#### Step 1. Create or open a Unity Project

<img src=".\Images\Usage\usage1.png" align="middle" width="50%"  />

#### Step 2. Install PPv2

Z Post-processing requires Unity PPv2 package. So make sure you install the PPv2 package in the Package Manager before you import this one. If you do not know how to install PPv2, please refer to [Post-processing stack v2 - Installation](https://docs.unity3d.com/Packages/com.unity.postprocessing@3.1/manual/Installation.html)

#### Step 3. Import "Z Glitch Effects" unitypackage and open the demo scene

The location of the demo scene: Assets/Z-PostProcessing/Demo/DemoScene.unity

The usage of Z Post-processing in build-in pipeline is the same as the Unity PPv2 (Post-processing stack v2). If you do not know how to use it, please refer to [Getting started with post-processing](https://docs.unity3d.com/Packages/com.unity.postprocessing@3.1/manual/Quick-start.html)









## Guide (URP)



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







## Guide (HDRP)

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



## Glitch Effects

### Glitch Analog Noise



<img src="https://raw.githubusercontent.com/Mirage-Game-Studio/PublicRepository/main/Z-Postprocessing/Images/Glitch/GlitchAnalogNoise.png"  align="middle" style="zoom:80%;" />

| Property                   | Description                                                  |
| -------------------------- | ------------------------------------------------------------ |
| Noise Speed                | Determine how fast the noise flickering, in a range from 0 to 1. |
| Noise Fading               | The fade amount to blend between normal and noise image, in a range from 0 to 1. |
| Luminance Jitter Threshold | Only the pixels which luminance above this threshold will jitter, in a range from 0 to 1. |




### Glitch Digital Stripe



<img src="https://raw.githubusercontent.com/Mirage-Game-Studio/PublicRepository/main/Z-Postprocessing/Images/Glitch/GlitchDigitalStripe.png"  align="middle" style="zoom:80%;" />

| Property                      | Description                                                  |
| ----------------------------- | ------------------------------------------------------------ |
| Intensity                     | Larger intensity will bring more jittering stripes, in a range from 0 to 1. |
| Frequency                     | The frequency of digital stripes, in a range from 1 to 10.   |
| Stripe Length                 | The Length of digital stripes, in a range from 0 to 0.99.    |
| Need Stripe Color Adjust      | If you need adjust color of stripes, turn it on.             |
| Stripe Color Adjust Color     | The adjustment color of stripes.                             |
| Stripe Color Adjust Intensity | The intensity of the stripe color, in a range from 0 to 10.  |
| Noise Texture Width           | The width of the noise texture, in a range from 8 to 256.    |
| Noise Texture Height          | The height of the noise texture, in a range from 8 to 256.   |




### Glitch Image Block



<img src="https://raw.githubusercontent.com/Mirage-Game-Studio/PublicRepository/main/Z-Postprocessing/Images/Glitch/GlitchImageBlock.png"  align="middle" style="zoom:80%;" />

| Property                | Description                                                  |
| ----------------------- | ------------------------------------------------------------ |
| Fade                    | The fade amount to blend between normal and noise image, in a range from 0 to 1. |
| Speed                   | Determine how fast the noise blocks flickering, in a range from 0 to 1. |
| Amount                  | The amount of the noise blocks, in a range from 0 to 10.     |
| Block Layer 1_U         | The U (horizontal) factor to adjust generated noise blocks of the first layer, in a range from 0 to 50. |
| Block Layer 1_V         | The V (vertical) factor to adjust generated noise blocks of the first layer, in a range from 0 to 50. |
| Block Layer 2_U         | The U (horizontal) factor to adjust generated noise blocks of the second layer, in a range from 0 to 50. |
| Block Layer 2_V         | The V (vertical) factor to adjust generated noise blocks of the second layer, in a range from 0 to 50. |
| Block Layer 1_Intensity | The intensity factor of the first block layer, the larger the weaker, in a range from 0 to 50. |
| Block Layer 2_Intensity | The intensity factor of the second block layer, the larger the weaker, in a range from 0 to 50. |
| RGB Split Intensity     | The splitting strength of the RGB three color channels, in a range from 0 to 50. |
| Block Visualize Debug   | The toggle to visualize the generated noise blocks.          |




### Glitch Image Block V2



<img src="https://raw.githubusercontent.com/Mirage-Game-Studio/PublicRepository/main/Z-Postprocessing/Images/Glitch/GlitchImageBlockV2.png"  align="middle" style="zoom:80%;" />

| Property                | Description                                                  |
| ----------------------- | ------------------------------------------------------------ |
| Fade                    | The fade amount to blend between normal and noise image, in a range from 0 to 1. |
| Speed                   | Determine how fast the noise blocks flickering, in a range from 0 to 1. |
| Amount                  | The amount of the noise blocks, in a range from 0 to 10.     |
| Block Layer 1_U         | The U (horizontal) factor to adjust generated noise blocks of the first layer, in a range from 0 to 50. |
| Block Layer 1_V         | The V (vertical) factor to adjust generated noise blocks of the first layer, in a range from 0 to 50. |
| Block Layer 1_Intensity | The intensity factor of the first block layer, the larger the weaker, in a range from 0 to 50. |
| RGB Split Intensity     | The splitting strength of the RGB three color channels, in a range from 0 to 50. |
| Block Visualize Debug   | The toggle to visualize the generated noise blocks.          |


### Glitch Image Block V3



<img src="https://raw.githubusercontent.com/Mirage-Game-Studio/PublicRepository/main/Z-Postprocessing/Images/Glitch/GlitchImageBlockV3.png"  align="middle" style="zoom:80%;" />

| Property   | Description                                                  |
| ---------- | ------------------------------------------------------------ |
| Speed      | Determine how fast the noise blocks flickering, in a range from 0 to 50. |
| Block Size | The property to adjust the block size, the larger the smaller, in a range from 0 to 50. |


### Glitch Image Block V4



<img src="https://raw.githubusercontent.com/Mirage-Game-Studio/PublicRepository/main/Z-Postprocessing/Images/Glitch/GlitchImageBlockV4.png"  align="middle" style="zoom:80%;" />

| Property        | Description                                                  |
| --------------- | ------------------------------------------------------------ |
| Speed           | Determine how fast the noise blocks flickering, in a range from 0 to 50. |
| Block Size      | The property to adjust the block size, the larger the smaller, in a range from 0 to 50. |
| Max RGB Split X | The max splitting amount of RGB colors in horizontal direction. |
| Max RGB Split Y | The max splitting amount of RGB colors in vertical direction. |


### Glitch Line Block



<img src="https://raw.githubusercontent.com/Mirage-Game-Studio/PublicRepository/main/Z-Postprocessing/Images/Glitch/GlitchLineBlock.png"  align="middle" style="zoom:80%;" />

| Property        | Description                                                  |
| --------------- | ------------------------------------------------------------ |
| Block Direction | The property to determine the direction that blocks will fickering on, Horizontal or Vertical. |
| Interval Type   | The interval mode that line blocks will appear. Infinite, Periodic or Random. |
| Frequency       | The frequency of the line blocks, in a range from 0 to 25.   |
| Amount          | The amount of the line blocks, in a range from 0 to 1.       |
| Lines Width     | The width of the blocky lines, in a range from 0.1 to 10.    |
| Speed           | Determine how fast the line blocks flickering, in a range from 0 to 50. |
| Offset          | The offset of the glitchy blocks from the normal position, in a range from 0 to 13. |
| Alpha           | The alpha or fading amount of the glitchy blocks, in a range from 0 to 1. |


### Glitch RGB Split



<img src="https://raw.githubusercontent.com/Mirage-Game-Studio/PublicRepository/main/Z-Postprocessing/Images/Glitch/GlitchRGBSplit.png"  align="middle" style="zoom:80%;" />

| Property        | Description                                                  |
| --------------- | ------------------------------------------------------------ |
| Split Direction | The RGB splitting direction: Horizontal, Vectical or Horizontal_Vertical (aka Diagonal). |
| Amount          | The offset amount of the RGB splitting, in a range from 0 to 5. |
| Speed           | The animation speed of the RGB splitting, in a range from 0 to 10. |
| Fading          | The fading amount of the RGB splitting, in a range from 0 to 1. |
| Center Fading   | The fading amount to control the RGB splitting in the center of screen, in a range from 0 to 1. |
| Amount R        | The offset amount of the splitting for only red color.       |
| Amount B        | The offset amount of the splitting for only blue color.      |


### Glitch RGB Split V2



<img src="https://raw.githubusercontent.com/Mirage-Game-Studio/PublicRepository/main/Z-Postprocessing/Images/Glitch/GlitchRGBSplitV2.png"  align="middle" style="zoom:80%;" />

| Property        | Description                                                  |
| --------------- | ------------------------------------------------------------ |
| Split Direction | The RGB splitting direction: Horizontal, Vectical or Horizontal_Vertical (aka Diagonal). |
| Amount          | The offset amount of the RGB splitting, in a range from 0 to 1. |
| Amplitude       | The amplitude of the RGB splitting, in a range from 1 to 6.  |
| Speed           | The animation speed of the RGB splitting, in a range from 0 to 2. |


### Glitch RGB Split V3



<img src="https://raw.githubusercontent.com/Mirage-Game-Studio/PublicRepository/main/Z-Postprocessing/Images/Glitch/GlitchRGBSplitV3.png"  align="middle" style="zoom:80%;" />

| Property        | Description                                                  |
| --------------- | ------------------------------------------------------------ |
| Split Direction | The RGB splitting direction: Horizontal, Vectical or Horizontal_Vertical (aka Diagonal). |
| Interval Type   | The interval mode that the splitting will occur. Infinite, Periodic or Random. |
| Frequency       | The frequency of the RGB splitting, in a range from 0.1 to 25. |
| Amount          | The offset amount of the RGB splitting, in a range from 0 to 200. |
| Speed           | The animation speed of the RGB splitting, in a range from 0 to 20. |


### Glitch RGB Split V4



<img src="https://raw.githubusercontent.com/Mirage-Game-Studio/PublicRepository/main/Z-Postprocessing/Images/Glitch/GlitchRGBSplitV4.png"  align="middle" style="zoom:80%;" />

| Property        | Description                                                  |
| --------------- | ------------------------------------------------------------ |
| Split Direction | The RGB splitting direction: Horizontal, Vectical or Horizontal_Vertical (aka Diagonal). |
| Intensity       | The strength of the RGB splitting, can be negative, in a range from -1 to 1. |
| Speed           | The animation speed of the RGB splitting, in a range from 0 to 100. |


### Glitch RGB Split V5



<img src="https://raw.githubusercontent.com/Mirage-Game-Studio/PublicRepository/main/Z-Postprocessing/Images/Glitch/GlitchRGBSplitV5.png"  align="middle" style="zoom:80%;" />

| Property  | Description                                                  |
| --------- | ------------------------------------------------------------ |
| Noise Tex | The noise texture is used to adjust the splitting amount.    |
| Amplitude | The amplitude of the RGB splitting, in a range from 0 to 5.  |
| Speed     | The animation speed of the RGB splitting, in a range from 0 to 1. |


### Glitch Scan Line Jitter



<img src="https://raw.githubusercontent.com/Mirage-Game-Studio/PublicRepository/main/Z-Postprocessing/Images/Glitch/GlitchScanLineJitter.png"  align="middle" style="zoom:80%;" />

| Property         | Description                                                  |
| ---------------- | ------------------------------------------------------------ |
| Jitter Direction | The direction of the shaking lines, Horizontal or Vertical.  |
| Jitter Intensity | The strength of the jittering, in a range from 0 to 1.       |
| Interval Type    | The interval mode that shaking lines will appear. Infinite, Periodic or Random. |
| Frequency        | Using this property to tune the frequency of jittering if you select Periodic or Random, in a range from 0 to 25. |


### Glitch Screen Jump



<img src="https://raw.githubusercontent.com/Mirage-Game-Studio/PublicRepository/main/Z-Postprocessing/Images/Glitch/GlitchScreenJump.png"  align="middle" style="zoom:80%;" />

| Property              | Description                                               |
| --------------------- | --------------------------------------------------------- |
| Screen Jump Direction | The direction of the screen jump, Horizontal or Vertical. |
| Screen Jump Intensity | The intensity of the screen jump, in a range from 0 to 1. |

### Glitch Screen Shake



<img src="https://raw.githubusercontent.com/Mirage-Game-Studio/PublicRepository/main/Z-Postprocessing/Images/Glitch/GlitchScreenShake.png"  align="middle" style="zoom:80%;" />

| Property               | Description                                                |
| ---------------------- | ---------------------------------------------------------- |
| Screen Shake Direction | The direction of the screen shake, Horizontal or Vertical. |
| Screen Shake Intensity | The intensity of the screen shake, in a range from 0 to 1. |

### Glitch Tile Jitter



<img src="https://raw.githubusercontent.com/Mirage-Game-Studio/PublicRepository/main/Z-Postprocessing/Images/Glitch/GlitchTileJitter.png"  align="middle" style="zoom:80%;" />

| Property            | Description                                                  |
| ------------------- | ------------------------------------------------------------ |
| Splitting Direction | The splitting direction of the glitchy tiles, Horizontal or Vertical. |
| Splitting Number    | The number of the splitting tiles, in a range from 0 to 50.  |
| Interval Type       | The interval mode that glitchy tiles will jitter. Infinite, Periodic or Random. |
| Frequency           | Using this property to tune the frequency of jittering if you select Periodic or Random for Interval Type, in a range from 0 to 25. |
| Jitter Direction    | The jitter direction of splitting tiles, Horizontal or Vertical. |
| Amount              | The offset amount of jittering tiles, in a range from 0 to 100. |
| Speed               | The animation speed of the jitter, in a range from 0 to 1.   |

### Glitch Wave Jitter



<img src="https://raw.githubusercontent.com/Mirage-Game-Studio/PublicRepository/main/Z-Postprocessing/Images/Glitch/GlitchWaveJitter.png"  align="middle" style="zoom:80%;" />

| Property          | Description                                                  |
| ----------------- | ------------------------------------------------------------ |
| Jitter Direction  | The jitter direction of splitting tiles, Horizontal or Vertical. |
| Interval Type     | The interval mode that glitchy tiles will jitter. Infinite, Periodic or Random. |
| Frequency         | Using this property to tune the frequency of jittering if you select Periodic or Random for Interval Type, in a range from 0 to 25. |
| RGB Split         | The offset amount of RGB colors splitting, in a range from 0 to 50. |
| Speed             | The animation speed of the wave jitter, in a range from 0 to 1. |
| Amount            | The offset amount of the wave jitter, in a range from 0 to 2. |
| Custom Resolution | If you want to specify the resolution of the wave jitter, toggle it on. |
| Resolution        | The custom resolution for the wave jitter. Use it to adjust the density of the wave jitter. |





































