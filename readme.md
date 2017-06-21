# Vive Stereo Rendering Prototypes
Copyright (c) 2016-2017 HTC Corporation. All Rights Reserved.

## Introduction

- Vive Stereo Rendering Toolkit provides drag-and-drop components for developers to create 
  stereoscopic rendering effects in a few minutes. 

- With this toolkit, effects such as mirrors or portal doors can be easily achieved in your 
  VR application.

- For tutorial and API reference, please see the attached Developer's Guide.

## System Requirements

- Unity 5.3.5 or higher.
  This toolkit is compatible with native VR rendering introduced in Unity 5.4.

- SteamVR Unity plugin, version 1.2.0 or higher

## Known Issues

- Shadow rendering is wrong when using single-pass Stereo in Unity 5.4.x
  (this is caused by Unity issue #686520)

## Change log

v1.0.9
 - fix wrong rendering under single-pass stereo rendering for Unity 5.6.0

v1.0.8
 - new icon :)

v1.0.7
 - fix compatiblity for SteamVR plugin v1.2.1
 - bug fix: cannot build project due to SerializedProperty not exist outside of Unity Editor 

v1.0.6
 - Each StereoRenderer can have different "ignore object list"
   (for existing project, need to add proper layers to Unity "Tags and Layers Manager" manually)

v1.0.5
 - [Backward Compatibility Break Change!] 
   Minimal supported SteamVR plugin version changed to v1.2.0
 - fix compatibility issue for SteamVR plugin v1.2.0

v1.0.4
 - support double-sided StereoRenderer
 - bug fix: fix right-eye rendering of mirrors (for Unity 5.4+)

v1.0.3
 - Unity 5.5 compatibility
 - enable creation of StereoRenderer at runtime
 - add parameter for tweaking resolution of rendertextures
 - bug fix: fix "drifting" when entering portals (for Unity 5.4)
 - bug fix: fix rendering of near-anchor objects (for Unity 5.4+)

v1.0.2
 - bug fix: fix wrong shadow in canvases when using directional light (for Unity 5.4)

v1.0.1
 - add functions to query the up, forward and right vectors of canvas origin
 - support moving or rotating mirrors at run time
 - support mirrors of arbitrary orientation
 - bug fix: only remove StereoRenderers from manager when their host object is destroyed

## Contributing guidelines:

1. Read the CLA.
2. Create an issue for the work you want to contribute.
3. Fork this project on GitHub.
4. Create a new branch (based on master branch) for your work on your fork.
5. After you finish your work
    - Make sure all files start with `//========= Copyright 2016-2017, HTC Corporation. All rights reserved. ===========`
    - Try leaving [good commit message](https://chris.beams.io/posts/git-commit/) and [keeping commit histories clean](https://www.notion.so/Keeping-Commit-Histories-Clean-0f717c4e802c4a0ebd852cf9337ce5d2).
6. Submit a pull request from your new branch to our develop branch.
