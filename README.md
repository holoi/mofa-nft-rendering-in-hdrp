# mofa-nft-rendering-in-hdrp

This is the rendering project for the MOFA project, primarily responsible for creating and outputting visual content for MOFA NFTs. In this project, there are 9 early versions(Version 0.1) of NFT visual content and 4(Version 0.2) created during the 2023 Flow Hackathon, located in the scenes 'Assets->Nft0.1->Scene.1' and 'Assets->Nft0.2->Scenes->Scene'.

## Demo
### Version 0.1
#### Mystic


https://github.com/holoi/mofa-nft-rendering-in-hdrp/assets/52849063/b7ce66bd-8f67-4225-a539-1ae610b1e59f


#### Thunder


https://github.com/holoi/mofa-nft-rendering-in-hdrp/assets/52849063/da666ab3-299b-4ab8-8cd1-3fe620319847


#### HP


https://github.com/holoi/mofa-nft-rendering-in-hdrp/assets/52849063/4320448c-fd91-4356-9dea-181166960acc


#### Feather


https://github.com/holoi/mofa-nft-rendering-in-hdrp/assets/52849063/41a57de3-a1b6-41a7-af15-b2bc9a077e81


#### Duck


https://github.com/holoi/mofa-nft-rendering-in-hdrp/assets/52849063/8cceed22-be3e-43e8-9ab0-30658270da57


#### Fire


https://github.com/holoi/mofa-nft-rendering-in-hdrp/assets/52849063/bd757cbb-3be9-4c5f-b14c-aed049a5f84b


#### Electric


https://github.com/holoi/mofa-nft-rendering-in-hdrp/assets/52849063/b6838a9c-0faa-47b2-ac6d-0cb38bc15f69


#### Water


https://github.com/holoi/mofa-nft-rendering-in-hdrp/assets/52849063/256f1983-dc44-46fa-bb36-a9bd74fa8c32


#### TimeStone


https://github.com/holoi/mofa-nft-rendering-in-hdrp/assets/52849063/ccebbe8c-bb32-49c0-a4e2-d087bed9030d



### Version0.2
#### Myctic


https://github.com/holoi/mofa-nft-rendering-in-hdrp/assets/52849063/aa871cb3-587e-408b-8da5-d9451acb96a2


#### Thunder



https://github.com/holoi/mofa-nft-rendering-in-hdrp/assets/52849063/2e4ac5e6-aa35-4d50-914c-0395b481f0e0


#### HP


https://github.com/holoi/mofa-nft-rendering-in-hdrp/assets/52849063/aceab8e7-7487-4954-a2a9-493ba88444a6

### Feather



https://github.com/holoi/mofa-nft-rendering-in-hdrp/assets/52849063/a086fd8d-3c63-4e52-ae06-797772e768b1

## System requirements
Unity: 2023.3.12f1 and above.

## How to try it
Among all nfgt game objects in a version of 0.1, they are generally composed of two parts: the weapon visuals("Weapon" GameObject) and the surrounding force field visuals("Field" GameObject). The visual aspects of all NFT objects are primarily handled by the Visual Effect Graph.

<img width="286" alt="image" src="https://github.com/holoi/mofa-nft-rendering-in-hdrp/assets/52849063/789478da-00ee-42c1-91c4-a5bf6e0d2bbc">

In the force field objects, there is a set of properties controlling the basic content of a particle system, such as the lifespan, particle count, size, color, etc., which are easy to understand, and you can adjust parameters to observe changes. 

![image](https://github.com/holoi/mofa-nft-rendering-in-hdrp/assets/52849063/bfdb1b09-a493-433a-a7ed-5e3dfa617c5b)


In addition, the force field utilizes two SDFs to control the direction and magnitude of forces in the field. Here, we can modify properties like size, rotation, scale of SDFs to adjust the force field effects.

![image](https://github.com/holoi/mofa-nft-rendering-in-hdrp/assets/52849063/7aaa1ccf-0206-4a9b-b3bf-03bcb5160ca4)

Here we provide some SDF Textures under path: Assets->Textures->Field SDFs. Try it out by yourself.

In the weapon obejcts, the main shape controled by a SDF texture.

![image](https://github.com/holoi/mofa-nft-rendering-in-hdrp/assets/52849063/e3d81860-de8e-4132-8ab2-ae7480ae1bd0)

There is a set of properties controlling the basic content of a particle system, such as the lifespan, particle count, size, color, etc., which are easy to understand, and you can adjust parameters to observe changes. 

![image](https://github.com/holoi/mofa-nft-rendering-in-hdrp/assets/52849063/80eb1552-173f-4269-81fc-d69f7cd798ff)

Nft objects in a version of 0.2 got a set of properties related to "Level", in our design, those nft objects grows along the level, shape and brightness changes during the process. Addtionally, Nft objects in a version of 0.2 have Animator component to diaplay the process of growth. Select object, open animator window and press "Space" to play the animation.

![image](https://github.com/holoi/mofa-nft-rendering-in-hdrp/assets/52849063/348d84bc-1822-4b8a-8402-97fb618ca073)

Animation Window:

<img width="649" alt="image" src="https://github.com/holoi/mofa-nft-rendering-in-hdrp/assets/52849063/b5009fda-2f47-4034-a45f-6c93c75e06df">

