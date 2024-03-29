---
title: "Understanding Tiling Window Managers"
excerpt: ""
---
TOS by default uses what is called a tiling window manager. What it does is rather simple.
Lets first understand what a window manager is.
A window manager is exactly what it says. It manages windows or in other words applications. It handles opening, closing, resizing and moving of applications. For exaple you can open a browser (an application) and open for example a pdf viewer. The window manager will then manage those 2 windows. Usually they are stacked ontop of eachother (the pdf viewer is ontop of the browser).
A tiling window manager is a specific way of handeling windows. When you for example open a browser it will start in fullscreen mode. When we then open up a pdf viewer the browser will be scaled to only take up half of the screen. Whilst the pdf viewer will take up the other half. Lets take a look at the difference using pictures.
[block:api-header]
{
  "title": "Normal Window Manager"
}
[/block]
Here we show the example of the browser and pdf viewer using a normal window manager
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/84be730-Window-manager.png",
        "Window-manager.png",
        1920,
        1080,
        "#666c76"
      ]
    }
  ]
}
[/block]

[block:api-header]
{
  "title": "Tiling window manager"
}
[/block]
Here we show the example of the browser and pdf viewer using a tiling window manager
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/d113f3b-Tiling-Window-Manager.png",
        "Tiling-Window-Manager.png",
        1920,
        1080,
        "#6f747d"
      ]
    }
  ]
}
[/block]
Notice that if we open up a second window the first one resized to let the second one take up the extra space.