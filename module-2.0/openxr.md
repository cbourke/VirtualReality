

Hello everyone! I decided to not use steam vr for module 2 and it went absolutely fantastic so I'm here to convince you to try out OpenXR if you are having issues with SteamVR!

I decided to switch to open xr because it seemed like there were more tutorials for it on youtube. Trying to search for "how to make xyz in steam vr" always turned up incorrect results for me and I got pretty frustrated trying to deviate from steam VR's sample project. Steam VR is easy to set up and get rolling but if you want to do anything beyond your basic grab or interaction implementing custom logic can be tricky. This was also another reason why I decided to use OpenXR.

To get going with open xr I watched this video: https://www.youtube.com/watch?v=DQAwRnGAHoU
Make sure you create a new project that does not have steam vr already set up inside of it as you can run into issues. The nice thing about this video is there's also a repo you can clone to just get the project. Initially xr didn't work for me but that's because he was using an index. In order to get this to work with our vives go to edit > project settings > openXR > features > "check htc vive controller profile"

You will have to spend some time setting up the open xr player but in my opinion it's worth it because it cuts out on a lot of complicated pieces steam vr utilizes. You will start with blocks for hands but simple tutorials exist for adding hand/body support instead of just cubes -https://www.youtube.com/watch?v=VdT0zMcggTQ&list=PLrk7hDwk64-a_gf7mBBduQb3PEBYnG4fU&index=4

Once you have this project setup you're good to go! Please note these tutorials are a bit old so READ THE COMMENTS!! Scripts like "XR Rig" are now called "XR Origin". Remember if something is missing or not the same as the guy in the video just check the comments!

Once you get the basic controller setup refer to this tutorial series for additional content: https://www.youtube.com/watch?v=gGYtahQjmWQ&list=PLrk7hDwk64-a_gf7mBBduQb3PEBYnG4fU


You can also use OpenXR without a headset: https://www.youtube.com/watch?v=UlqdHrfXppo&t=41s

something else to note: the interaction toolkit used in the first setup video will not show up. You have to add it by name: com.unity.xr.interaction.toolkit
