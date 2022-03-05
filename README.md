[![Actions](https://github.com/misabiko/GithubPagesURP/actions/workflows/main.yml/badge.svg)](https://github.com/misabiko/GithubPagesURP/actions/workflows/main.yml)
 
An empty project with "3D (URP)" to test deployment on Github Pages, using Unity 2021.2.8f1
 
WebGL build hosted on https://misabiko.github.io/GithubPagesURP/


Changes from template
- Added a cube to the scene
- Switched build platform to WebGL
- In Player Settings
  - Unchecked "Auto Graphics API"
  - Removed "WebGL 1 (Deprecated)" from Graphics APIs

Tried
- Checking "Decompression Fallback"
  - Internal-ErrorShader.shader is not found
- Not checking fallback but adding web.config to Build/
  - Looks like Github Pages doesn't load web.config, js.rs is still read as application/octet-stream
- Disabling compression all together
  - Internal-ErrorShader.shader is still not found
