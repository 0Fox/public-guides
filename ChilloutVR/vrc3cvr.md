# Requirements
1. Unity 2019.4.31f
1. [VRCSDK for Unity 2019.4.31f](https://vrchat.com/download/sdk3-avatars)
1. [CCK for Unity 2019.4.31f](https://files.abidata.io/static_web/ChilloutVR%20CCK%20v3.3%20RELEASE.unitypackage)
1. [Dynamic Bones which you definitely bought](https://www.google.com/search?q=dynamic+bones+unitypackage)
1. [VRC3CVR Converter](https://github.com/imagitama/vrc3cvr/releases)
1. [PhysBone2DynamicBone](https://booth.pm/en/items/4032295) _(if the avatar has VRC's PhysBones)_


## 1-a. If you're importing an avatar that is intended for VRChat:
* Create a new 3D core project in Unity hub.
* Import VRCSDK.
* Import the avatar and everything it requires.

## 1-b. If you have a project with your VRChat avatar:
* __**MAKE A BACKUP** (Create an archive or a copy of the folder)__.
* Update your Unity to 2019.4.31f if it's older.

## 2. Importing stuff:
* Import Dynamic Bones.
* Import PhysBone2DynamicBone (needed only if the avatar has VRC's PhysBones).
* Import CCK.
* Import VRC3CVR

## 3. Converting Phys Bones to Dynamic Bones (**only if the avatar has VRC's PhysBones**)
* Moyuer -> PhysBone2DynamicBone
* Drag and drop in your avatar from Hierarchy:

![image](https://user-images.githubusercontent.com/24230448/181514243-bcf09b16-2b2a-449f-a78f-11ff984332db.png)
* Press Apply. This will create a dupe of the avatar with Dynamic Bones, use the dupe in the next steps

## 4. Converting VRC Scripts and Gestures to CVR
* PeanutTools -> VRC3CVR
* Drag and drop in your avatar from Hierarchy
* Press Convert
* Click on the avatar in Hierarchy, find the component "CVR Asset Info", click on "Detach asset unique identifier" if you can

![image](https://user-images.githubusercontent.com/24230448/181520625-b04a305c-2059-481c-b529-f91164b55a80.png)


## 5. Uploading
* Alpha Blend Interactive -> Control Panel
* Log in using your login and CCK API Key (that you can find [here](https://hub.abinteractive.net/my?cat=edit))
* Select the avatar in the Control Panel and upload it following the instructions in CCK.

## 6. Done
### You might wanna adjust some things after converting everything. Like.. The latest Rex has a floor trigger/collider & headpat animation that won't work with Dynamic Bones, so you probably want to yeet them. Also Voice position is currently in your view position, because VRC doesn't have that at all, so maybe move it where your mouth is.
