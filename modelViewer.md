Adding 3D elements to your website sounds daunting, requiring highly creative thinking and potentially adding layers of difficulty to your workload.
Typically, you would need to understand something like Three.JS along with GLSL to create the viewer and the scene in WebGL, maybe Blender for creating the asset, and then a bundler to secure the codebase ready for deployment. 

This is a lot....and maybe you don't have the time to invest in learning all that, or the budget to employ someone who does.

But with [Model Viewer](https://modelviewer.dev/), the Open-source, easy-to-implement, and well-optimised HTML Web component 🎇🎇, we can add these elements and create some excellent wow factor to your site.

## Enter `<model-viewer>`

Just look at how smooth this operates in my browser (Google Chrome):

<img src="https://i.gyazo.com/092c9ce55a1c105f7410dc03090ed07a.gif" width=35% height=35% />

Source: _Gif recording of the example on https://modelviewer.dev/_


It's been over two years, and I'm still telling people about this awesome web component. Used it first in a Hackathon for Breast Cancer to showcase human anatomy. The brief we wanted to accomplish was briding the gap of breat cancer and technology using current tech available. 3D in the browser was not a new thing, but it was emerging, and we wanted to show that in our project.

Fun fact, it was the first time meeting [Kera Cudmore](https://github.com/kera-cudmore) as we were on the same team together. Time really does fly! 🤜

But what I'm really raving about, is how ridiculously easy it is to actually get this working.
* Have a 3D asset with an applicable file type
* Import the Web Component, `<model-viewer>` using the script module import in your HTML. (Yes, HTML)
* Use the `<model-viewer>` element in your HTML like any other HTML element.

And that's it. Well not exactly, but that is the basis for everything, you still need to save the 3D asset in your file directory, and then link it in the `src` attribute of the web component.

```html
<model-viewer
    auto-rotate
    loading="eager"
    field-of-view="30deg"
    alt="meaningful alternative text"
    src="3dAsset.gltf">
</model-viewer>
```
👆 Such a handy little snippet of HTML, and all because we imported the web component into the page for use. This code, will show a viewer element, where the user can zoom, pan, and move through 3D space with mouse/touch gestures. Awesome 👏!

_By the way_, did I mention this can just be deployed to Github Pages or Vercel without the need to bundle your codebase? Well you can!

#### Want to see it in action? Check out these projects:

* [Bust It: Cancer without Borders](https://vanessacleary.github.io/W-I-T-IT-LAB-Breast-Cancer-Awareness/) - Breast Cancer awareness Hackathon project 2021 highlighting Transgender Communities. Utilises Model-Viewer to show 3D human anatomy forms.
* [Save Earth](https://hashim222.github.io/save-earth/) - Earth Day 2022 Hackathon project. Utilises Model-Viewer to enable interactive planet scaling of Earth and Mars...and a Death Star!
* [ZTM Canvaz Hacktoberfest 2021](https://zero-to-mastery.github.io/Canvaz/art/auxfuse-modelSwitcher/index.html) - Hacktoberfest submission 2021 to the Zero to Mastery Community Project. Utilises Model-Viewer to switch between different GLTF 3D models in a viewer.

### Where to find assets:

I did promise I would show you where to get the assets from.

* [Market](https://market.pmnd.rs/) - Lots and lots of free Models/Textures/HDRIs
* [Sketchfab](https://sketchfab.com/features/gltf) - Over 800K models available under Creative Commons licensing, from hi-res to low-poly
* [Smithsonian](https://3d.si.edu/) - Educational website offering open access to GLTF models

There is plenty more available, you might just need to do a bit of digging, and of course please be mindful when downloading files from sources you may not have complete faith in. 🔐

### Documentation

`<model-viewer>` has an incredible team of people behind it. It is a Google project, open-source, and the documentation and examples of using it are excellent.

The [website](https://modelviewer.dev/) has some excellent getting-started steps, and the documentation for use cases of the web component are expertly crafted. The Quick Start guide is located on the homepage of the site itself...no fuss, no mess.

The web component itself uses Three.JS under the hood for rendering, and is now a Google hosted library. And of course it's free and easy to implement, as easy as just adding the Script link to the HTML file linked to the CDN source!

### Try it out with a starter project?

Let's quickly bash something up together. How about looking at a Cut chibi dog on a webpage, complete with deployment?

Repo here: 

Or just follow these steps:

* Let's start by getting the Dog GLTF Model shall we? Go to [Market](https://market.pmnd.rs/model/dogue) and download the model of this Dog.🐶
* Open up your favorite editor, in my case I'm using vsCode and create a new project.
* Put the `model.gltf` file in the file directory of your newly created project. It most likely went to your "Downloads" folder, so you can just drag it across or cut/paste etc.✂
* Create an `index.html` page with the following code. This includes the Script link to the Google model-viewer Library Hosting CDN.

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Model Viewer Demonstration</title>
    </head>
    <body>

        <h1>Model viewer demonstration</h1>
        <p>
            This is a code demonstration of the
            <a href="https://modelviewer.dev/" target="_blank">
            Google Model-viewer</a> 3D web component.
        </p>
        
        <!-- Import the component -->
        <script type="module" src="https://ajax.googleapis.com/ajax/libs/model-viewer/3.0.1/model-viewer.min.js"></script>
    </body>
</html>
```
* At this stage you should have the model, and the HTML both sitting in the root of your project. Why the root? Well this is a basic demonstration, and it will be easy to link the two files when we get to that stage.😅

<img src="" alt="Model-Viewer Demo File Directory screenshot" width=50% height=50% />