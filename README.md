# mofa-nft-rendering-in-hdrp

This is the rendering project for the MOFA project, primarily responsible for creating and outputting visual content for MOFA NFTs. In this project, there are 9 early versions(Version 0.1) of NFT visual content and 4(Version 0.2) created during the 2023 Flow Hackathon, located in the scenes 'Assets->Nft0.1->Scene.1' and 'Assets->Nft0.2->Scenes->Scene'.

## Demo
### Version 0.1
#### Mystic


<img src="Documentation~/images/mystic.avif" width="480" />


#### Thunder


<img src="Documentation~/images/thunder.avif" width="480" />



#### HP


<img src="Documentation~/images/hp.avif" width="480" />



#### Feather


<img src="Documentation~/images/feather.avif" width="480" />



#### Duck


<img src="Documentation~/images/duck.avif" width="480" />



#### Fire


<img src="Documentation~/images/fire.avif" width="480" />



#### Electric


<img src="Documentation~/images/lightning.avif" width="480" />



#### Water


<img src="Documentation~/images/water.avif" width="480" />



#### TimeStone


<img src="Documentation~/images/time.avif" width="480" />




### Version0.2
#### Myctic


<img src="Documentation~/images/mystic-2.avif" width="480" />



#### Thunder



<img src="Documentation~/images/thunder-2.avif" width="480" />



#### HP


<img src="Documentation~/images/hp-2.avif" width="480" />


### Feather

<img src="Documentation~/images/feather-2.avif" width="480" />

## System requirements
1. Unity: 2023.3.12f1

## How to try it
Among all nfgt game objects in a version of 0.1, they are generally composed of two parts: the weapon visuals("Weapon" GameObject) and the surrounding force field visuals("Field" GameObject). The visual aspects of all NFT objects are primarily handled by the Visual Effect Graph.

<img src="Documentation~/images/01.png" width="480" />


In the force field objects, there is a set of properties controlling the basic content of a particle system, such as the lifespan, particle count, size, color, etc., which are easy to understand, and you can adjust parameters to observe changes. 

<img src="Documentation~/images/02.png" width="480" />


In addition, the force field utilizes two SDFs to control the direction and magnitude of forces in the field. Here, we can modify properties like size, rotation, scale of SDFs to adjust the force field effects.

<img src="Documentation~/images/03.png" width="480" />


Here we provide some SDF Textures under path: Assets->Textures->Field SDFs. Try it out by yourself.

In the weapon obejcts, the main shape controled by a SDF texture.

<img src="Documentation~/images/04.png" width="480" />



There is a set of properties controlling the basic content of a particle system, such as the lifespan, particle count, size, color, etc., which are easy to understand, and you can adjust parameters to observe changes. 

<img src="Documentation~/images/05.png" width="480" />



Nft objects in a version of 0.2 got a set of properties related to "Level", in our design, those nft objects grows along the level, shape and brightness changes during the process. Addtionally, Nft objects in a version of 0.2 have Animator component to diaplay the process of growth. Select object, open animator window and press "Space" to play the animation.

<img src="Documentation~/images/06.png" width="480" />



Animation Window:

<img src="Documentation~/images/07.png" width="480" />


## Create you own visuals

Using Unity SDF Bake Tool is the fastest way to create your own sdf textures for "Weapon":

1. Create or download a 3d model
2. Import to Unity.
3. Open SDF Bake Tool, drag the mesh to it and bake.
For more information about how to use SDF Bake Tool: https://docs.unity3d.com/Packages/com.unity.visualeffectgraph@15.0/manual/sdf-bake-tool.html#:~:text=The%20SDF%20Bake%20Tool%20is,use%20in%20a%20visual%20effect.


Using external tools to vreate your sdf textures for "Field"

1. There are some sdf textures under: "NFT"->"Weapons Resources"->"SDFTextures", you can drag them into "Field" objedct to try it out. 
2. If you got your own sdf textures, import to Unity and drag to "Field".
3. Recommended Tools：
  vectoraygen: https://jangafx.com/software/vectoraygen/



## Reference

1. https://github.com/keijiro/SdfVfxSamples
2. https://github.com/keijiro/SushiVfx
