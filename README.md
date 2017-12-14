# Mixed Reality Tools and Development Platforms

The following are platforms &  tools  [Mixed Reality for All](https://makersall.org/making-ar-more-accessible/)   may use for AR/VR development:

- [WebVR/WebXR](https://github.com/aschneiderman/mixed-reality-tools/#webvr)
- [Unity](https://github.com/aschneiderman/mixed-reality-tools/#unity)
- [Miscellaneous](https://github.com/aschneiderman/mixed-reality-tools/#miscellaneous-tools) tools

As you begin to learn about AR/VR development, write up a few notes about your experience:

- What was easy to learn, what was hard?
- Once you learn the basics, what insights, metaphors, etc. did you learn along the way that you wish you'd had at the beginning?
- If you had to train people in the community how to use a tool/platform, what changes do you think would make it easier to learn?

Before you get started, you might want to watch the short 2 videos that helped give me a better idea of what the less far out but still very useful day-to-day uses of VR/AR might look like:

- Re-envisioning what using a [word processor](https://www.youtube.com/watch?feature=youtu.be&v=LxviGskApcw&app=desktop) might look like in VR
-  Constructing a 3D object [using using other people's 3d components](https://mobile.twitter.com/zite00/status/938169740840787969) as you find them  on the web.  


## WebVR

[WebVR](https://webvr.info/) is a standard for a web-based version of VR; as of October, a new version called WebXR also includes AR. WebVR/WebXR is only a few years old, but it's taken off in the last year, with support from Mozilla, Google, Microsoft, Facebook, and Apple. It has several major advantages:

- Because it's built on Internet standards, WebXR pages are linkable and searchable, and you don't have to install it 
- It's designed to make it as easy as possible to develop AR/VR pages that work across VR/AR headsets, some smart phones, and desktop browsers.
- For coding, it uses a very popular programming language: JavaScript 
- It's open source, which means that we can create libraries & tools on top of it to hide its complexity or to customize it for particular types of work/industries

To see what WebVR can do, check out Google's [WebVR experiments](https://experiments.withgoogle.com/webvr) page. 

Here's how to use WebVR (more details on [their website]( https://webvr.info/)):

- Most people working on this project don't own a VR/AR headset, but if you do it's pretty easy to use WebVR. Today most VR/AR headsets cost between a couple hundred to a couple thousand dollars. That's going to change in the next 2 years: Oculus says in "early 2018" will start selling Oculus Go, which will [cost $199]( https://www.oculus.com/go/); in 2019 Microsoft is going to launch the consumer-priced version of their headset (their developer headset now costs $3000); and in 2020 Apple is probably coming out with their headset.
- [Google Cardboard](https://vr.google.com/cardboard/): a cheapo virtual reality headset that's either literally made out of cardboard or an inexpensive material and which is powered by a smartphone. Google Cardboard has good support for WebVR. Someone on the project will need to explore which smart phones work well with it; I think most Android phones do, but I read conflicting things about iPhones.
- Android: some of the newer Android smartphones have AR built into them; we need to research this
 - iOS: in general, iOS hasn't had good support for WebVR. But in December, Mozilla launched an experimental [WebXR Viewer app](https://itunes.apple.com/us/app/webxr-viewer/id1295998056?ls=1&mt=8) that should let you view both AR and VR on iOS; for more info, see this [blog post](https://blog.mozvr.com/experimenting-with-ar-and-the-web-on-ios/)
 - Desktop browsers: several desktop browsers will work with WebVR, and all of them are trying to build and support. They don't offer as much interactive support as VR/AR headsets, but many of them will allow you to do basic interactions. Again, something we need to research

NOTE: usually when someone does a tech project in the community, they  try to only use tech that virtually everyone will be able to use. Since the goal of Mixed Reality for All is to work on the bleeding edge so we get to influence this emerging tech before it gets set in stone, we will be working with tech that many people can't fully use now but almost everyone will be able to use in the next few years.

### Developing WebVR: Using A-Frame ###

Once you're ready to get your feet wet developing AR/VR, don't work with WebVR directly. Instead, do what a lot of folks are doing and use a library/platform that is been built on top of it. We will probably end up making heavy use of the most popular platform: [A-Frame](https://aframe.io/).

A-Frame looks like someone saw WebVR and said to themselves, why should I have to write all that JavaScript? Why can't I write in something like HTML? From taking an initial look at it, it looks like A-Frame is well-documented and has lots of examples to learn from; to get started, check out the A-Frame [website]( https://aframe.io/).

Mixed Reality for All believes that the best way of making tech development available to as many people as possible is to [create a continuum of tools](https://datachefs.org/goals/continuum/) and  [smooth the learning curve](https://datachefs.org/goals/smoothcurve/) among them. So, as you start getting comfortable with A-Frame, ask yourself, if I were trying to build something in AR in an area I know something about -- e.g., cooking -- what layer would I want on top of A-Frame to make my work easier? For example, what HTML-like tags would I want, especially if I wasn't  a developer but a "power user"? 



### Developing WebVR: Other Tools/Platforms ###

A-Frame should give you plenty to play with. But if you're feeling particularly adventurous, here are some of the other ways to work with WebVR you might take a quick glance at.

- [three.js]( https://threejs.org/),  [Canon.JS]( http://www.cannonjs.org/), etc.: Another way people go is to combine other JavaScript libraries with WebVR. One popular library is three.js. Some of these libraries allow you to add features to WebVR.  For example, WebVR doesn't include a "physics engine," which lets you easily treat objects in VR/AR as if they existed in a world where there's gravity, objects can collide with each other, etc.  But you can easily add one.  Here's a [cool example](https://mobile.twitter.com/Datatitian/status/932021670340124672)    of how you can simulate cloth by combining A-Frame and the physics engine cannonjs.
- [React VR](https://facebook.github.io/react-vr/): if you are a web developer and you use [React](https://facebook.github.io/react-vr/), you might want to check this out
- [AR.js](https://github.com/jeromeetienne/ar.js): very cool library for AR development that's built from a combination of WebVR, several of the libraries, and magic fairy dust. Definitely check out some of the amazing examples that he's created. FYI, AR.js also [works with A-Frame](https://aframe.io/blog/arjs/)



## Unity

[Unity](https://unity3d.com/)is a 3D gaming engine that Google, Microsoft, Apple, Facebook, and others support for designing VR and AR. Unity is very powerful, there are lots of tutorials and other support, and there are a lot of free or cheap "assets" -- e.g., 3D objects -- that are easily available. And Unity's development editor is pretty customizable. However, there are several drawbacks to using Unity:

- Deploying what you built on Unity can be a real pain in the butt. For example, to build an AR project for an iPhone, you need to have Xcode 9 running on your computer, and Xcode 9 only runs on MacOS.
- Unity is a proprietary system, and you have to pay for it if you start making a decent amount of money off of it. Given that WebVR/XR is open source, it's unclear how long the main tech players will invest in supporting it. And because it's proprietary, we can't easily build other libraries/tools on top of it.
-  Most Unity projects require coding, and Unity uses the programming language C#, which is much harder to learn than JavaScript.

If you are working on Mixed Reality for All, you need to know that Unity exists. But given its drawbacks, it's unlikely we'll invest much if any time on it.

## Miscellaneous Tools

- [Sketchfab](https://sketchfab.com/): a website that lets you "publish, share, and explore 3D content on web, mobile, VR, and AR." You have to purchase some of the content, but there's a lot of free content on the site. When you start messing around with AR/VR, definitely worth checking out.
- [Google Expeditions](https://edu.google.com/expeditions/): a tool by Google for creating immersive VR journeys, especially for educational purposes. Google is also working on an AR version called Expeditions AR.

