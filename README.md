# Mixed Reality Tools and Development Platforms

 What platforms &  tools could  [Mixed Reality for All](https://makersall.org/making-ar-more-accessible/)   use for developing AR and VR?

- [WebVR/WebXR](https://github.com/aschneiderman/mixed-reality-tools/#webvr)
- [Unity](https://github.com/aschneiderman/mixed-reality-tools/#unity)
- [Miscellaneous](https://github.com/aschneiderman/mixed-reality-tools/#miscellaneous-tools) tools


## WebVR

[WebVR](https://webvr.info/) is

(Make sure this section isn't  too overwhelming)
Advantages:

- Don't have to download a separate app
- Eventually, can create seamless transition between web and VR/AR experience
- Large, robust community
- All open source
- Designed to encourage
- Linkable, searchable, etc.
- For coding, uses JavaScript
- Doesn't require access to the Internet; it's all JavaScript plus web GL, so you can run it off of a USB stick

Doesn't include AR just yet, but coming in the near future
(explain change in name)

(How to use it for desktop, mobile)

 - iOS:  Mozilla has an experimental [WebXR Viewer app](https://itunes.apple.com/us/app/webxr-viewer/id1295998056?ls=1&mt=8) that should let you view both AR and VR; for more info, see this [blog post](https://blog.mozvr.com/experimenting-with-ar-and-the-web-on-ios/)
 

[A-Frame](https://aframe.io/)


- React VR

[AR.js](https://github.com/jeromeetienne/ar.js)

It [works with A-Frame](https://aframe.io/blog/arjs/)

- [WebVR experiments](https://experiments.withgoogle.com/webvr): the latest experiments using WebVR, with links to each experiment's code

Great example of what doing real work in AR/VR might look like: [constructing something  using other people's 3d components](https://mobile.twitter.com/zite00/status/938169740840787969) as you find them  on the web.  FYI, this isn't a mockup,  he's actually doing it; it's powered by  Google's [Poly API](https://developers.google.com/poly/), an API designed to let you "discover, view, and download thousands of free 3D assets directly in your AR and VR apps"

Unlike tools like Unity, WebVR/WebXR doesn't come "with batteries included." For example, WebVR doesn't include a "physics engine," which lets you easily treat objects in VR/AR as if they existed in a world where there's gravity, objects can collide with each other, etc.  But you can easily add one.  Here's a [cool example](https://mobile.twitter.com/Datatitian/status/932021670340124672)    of how you can simulate cloth by combining  A Frame and the physics engine cannonjs.


## Miscellaneous Tools

- Expeditions VR (Does it include Expeditions AR yet?)
- Sketchfab: create and share 3D models


## Unity

[Unity](https://unity3d.com/)is a 3D gaming engine that Google, Microsoft, Apple, Facebook, and others support for designing VR and AR. Unity is very powerful, there are lots of tutorials and other support, and there are a lot of free or cheap "assets" -- e.g., 3D objects -- that are easily available. And Unity's development editor is very customizable. However, there are several drawbacks to using Unity:

- Unity is a proprietary system -- and it's a pretty complex system
-  Most Unity projects require coding, and Unity uses the programming language C#. C# has a pretty steep learning curve.
- Deploying what you built on Unity can be a real pain in the butt. For example, to build an AR project for an iPhone, you need to have Xcode 9 running on your computer, and Xcode 9 only runs on MacOS.
