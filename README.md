# UE VR Locomotion GripToMoveRotate
Unreal Engine Virtual Reality Grip/Grab Locomotion. Grab to Move / Rotate (Scale not quite working).

Functionality also seen in Unreal Engine's built in VR Editor / TiltBrush (unity) / Demeo (unity) / and other experiences. Oculus also has a version of this in their locomotion samples [GrabAndDrag](https://developer.oculus.com/documentation/unreal/unreal-samples/) though it runs on tick and doesn't handle rotation.


Dependencies *to avoid additional tweaking*:
 - Unreal Engine 4.27.2
 - default VR Template project
 - Enhanced Input
 - Quest HMD (1/2)


**Setup:**
1. Edit > Plugins > Enable "Enhanced Input" Plugin
2. Restart Now
3. Edit > Project Settings >
	- Change the Default Player Input Class to "Enhanced"
	- Change the Default Input Component Class to "Enhanced"
4. Close your project
5. Copy the "VRGripMovement" folder into your project's Content directory
6. Open Project
7. Open VRTemplateMap > World Settings > Override Default Pawn with included "VRPawn_Duplicate"


Play in VR preview or Build to HMD. Use either controller grips to move your VRPawn around the scene. Use both grips to rotate your VRPawn around.

Scale is partially implemented but the BP nodes are disconnected. I haven't yet figured out how to get it to work without being super jittery.
If you know what needs to be done please let me know.

The VRPawn_Duplicate has two sections of added code, commented in hard to miss Purple, should be pretty easy to follow.
If you have any questions reach out.


Some insight was gained from this forums thread, though much of the og post has missing images the conversation was useful:
https://forums.unrealengine.com/t/using-controllers-to-scale-rotate-re-position-world/74892/12
