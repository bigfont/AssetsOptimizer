AssetsOptimizer
===============

Compiles lesscss, minifies javascript, resizes and compresses images in one powershell script.

Prerequisites
===============

1 Install node.js (for the lesscss compiling)
2 Setup your assets folder structure. It should look something like this:

websiteRoot
  assets-00
    site
      css
      img
      js
      less

Instructions
===============

1 Copy the entire <assetOptimizer-Process-v00000000-0> directory (you can delete the v00000000-0 part).
2 Paste the directory as a sibling of your sites assets-00 directory. EG:

websiteRoot
  assets-00
  assetsOptimizer-Process

3 Open process.ps1 and edit the #user preferences# section.
4 Run assetOptimizer-Process\process.ps1 in PowerShell.

Results
===============

Compiles and minifies LESS. Saves the results as .min.css in a sibling /css directory.
Minifies JAVASCRIPT. Saves the results as .min.js in the existing /js directory
Strips, compresses, and resizes IMAGES for responsive layouts. Saves results in a child /resized directory.
