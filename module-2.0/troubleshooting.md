

**Input System Issues**

If you get an error about the input system, you may need to go to

`Edit > Project Settings > Player > Other > Active Input Handling`

and change it to “Both”

**Some Objects are Purple**

When importing materials from a non-URP project to a URP one, go to

`Edit > Render Pipepline > Universal Render Pipeline > Upgrade Project Materials`

For newer versions of Unity, this has been moved; see:

https://www.youtube.com/watch?v=zQIosR0P-RE

**Teleport 2-D fallback mode not working**

NOTE: this *may* break teleporting in the actual VR/headset so pick your poison
and revert this before you go to a VR station; otherwise don't worry about and
just use WASD to move around while developing.  

In order to cut down on all the teleport errors, you will need to go into
`Hand.cs` and comment out the code in the `TriggerHapticPulse` functions

Also, go into `SteamVR_Action_Vibration.cs` and comment out the code in the
`Execute` function.

Finally, in the `FallbackHand gameobject`, assign `Left` or `Right` hand
to the `Hand` setting.
