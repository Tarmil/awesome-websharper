# Awesome WebSharper

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of WebSharper libraries, samples and resources.

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
## Table of Contents

- [Examples](#examples)
  - [Applications](#applications)
- [Libraries](#libraries)
  - [Reactive libraries](#reactive-libraries)
  - [Server-side hosting](#server-side-hosting)
  - [Other libraries](#other-libraries)
  - [JavaScript library bindings](#javascript-library-bindings)
    - [3D and Game engines](#3d-and-game-engines)
    - [Browser Capabilities](#browser-capabilities)
    - [Charting and Graphs](#charting-and-graphs)
    - [Code and text editing](#code-and-text-editing)
    - [Database](#database)
    - [GUI and widgets](#gui-and-widgets)
    - [Maps](#maps)
    - [Math](#math)
    - [Mobile](#mobile)
    - [Reactive libraries](#reactive-libraries-1)
- [Resources](#resources)
  - [Blogs](#blogs)
  - [Sites](#sites)
  - [Academic publications](#academic-publications)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

## Examples

* <img width="20" alt="F#" src="fsharp.png"/> = Written in F#
* <img width="20" alt="C#" src="csharp.png"/> = Written in C#
* <img width="20" alt=".NET Core" src="netcore.png"/> = Written for .NET Core
* <img width="20" alt=".NET Framework" src="netfx.png"/> = Written for .NET Framework

### Applications

* [<img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Framework" src="netfx.png"/> 2048](https://github.com/websharper-samples/2048) - The well-known game 2048 reimplemented in F#, with a few custom rule options. [Running live](https://websharper-samples.github.io/2048/)

* [<img width="20" alt="C#" src="csharp.png"/> <img width="20" alt=".NET Framework" src="netfx.png"/> BookCollection](https://github.com/websharper-samples/BookCollection) - A client-server CRUD application using remoting and a reactive client side, with [full tutorial](https://github.com/websharper-samples/BookCollection/blob/master/BookCollection.md).

* <a name="LoginWithBulma"></a>[<img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Core" src="netcore.png"/> LoginWithBulma](https://github.com/websharper-samples/LoginWithBulma) - A client-side login page using HTML templating, with full tutorial.

* [<img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Core" src="netcore.png"/> Counter](https://github.com/websharper-samples/Counter) - Follow-up to [LoginWithBulma](#LoginWithBulma): A client-side Model-View-Update-style counter, with full tutorial.

* [<img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Framework" src="netfx.png"/> PeopleAPI](https://github.com/websharper-samples/PeopleAPI) - A simple CRUD REST API.

* [<img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Framework" src="netfx.png"/> MVU TodoMVC](https://github.com/dotnet-websharper/mvu/tree/master/WebSharper.Mvu.TodoMvc) - The classic TodoMVC app written with UI and [MVU](#mvu). [Running live](https://websharper-samples.github.io/Mvu)

* [<img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Framework" src="netfx.png"/> TodoMVC](https://github.com/websharper-samples/TodoMVC) - The classic TodoMVC app written with UI. [Running live](https://websharper-samples.github.io/TodoMVC/)


## Libraries

Libraries written with and for WebSharper.

### Reactive libraries

* <a name="ui"></a>[UI](https://github.com/dotnet-websharper/ui) (formerly known as UI.Next) - a library for constructing server-side and reactive client-side web pages in plain C#, F#, or with HTML templates.

    * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Framework" src="netfx.png"/> Examples: [Source](https://github.com/websharper-samples/ui) - [Running live](https://websharper-samples.github.io/ui/#/samples/SimpleTextBox)

    * <a name="forms"></a>[Forms](https://github.com/dotnet-websharper/forms) - an implementation of "Piglets" for UI. It provides a concise syntax to define forms and their validation with clear model vs rendering separation of concerns.
        * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Core" src="netcore.png"/> Example: [Source](https://github.com/websharper-samples/Forms) - [Running live](https://websharper-samples.github.io/Forms)
    
    * [Forms.Bootstrap](https://github.com/dotnet-websharper/forms.bootstrap) - Bootstrap-based widgets for [Forms](#forms).
        * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Core" src="netcore.png"/> Example: [Source](https://github.com/websharper-samples/Forms.Bootstrap) - [Running live](https://websharper-samples.github.io/Forms.Bootstrap)

    * [UI.Formlets](https://github.com/dotnet-websharper/ui.formlets) - a more concise, although less flexible, abstraction similar to [Forms](#forms).
        * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Core" src="netcore.png"/> Example: [Source](https://github.com/websharper-samples/UI.Formlets) - [Running live](https://websharper-samples.github.io/UI.Formlets)

    * [Charting](https://github.com/dotnet-websharper/charting) - An API for client-side charts similar to FSharp.Charting. Includes [ChartJs](#chartjs)-based rendering, but has back-end extensibility.
        * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Core" src="netcore.png"/> Example: [Source](https://github.com/websharper-samples/Charting) - [Running live](https://websharper-samples.github.io/Charting)
    
    * <a name="mvu"></a>[MVU](https://github.com/dotnet-websharper/mvu) - Model-View-Update (Elm-like) architecture for full client-side applications.
        * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Core" src="netcore.png"/> Example: [Source](https://github.com/websharper-samples/Mvu) - [Running live](https://websharper-samples.github.io/Mvu)

### Server-side hosting

* [Owin](https://github.com/dotnet-websharper/owin) - OWIN defines a standard interface between .NET web servers and web applications. This library allows hosting WebSharper applications on any OWIN-compliant host - ASP.NET, Katana, Suave, etc.

* [Owin.WebSocket](https://github.com/dotnet-websharper/owin.websocket) - Client-side and server-side WebSockets interface for OWIN-hosted applications, including automated serialization of messages.

* [ASP.NET Core](https://github.com/dotnet-websharper/aspnetcore) - Run WebSharper applications on ASP.NET Core.

* [ASP.NET MVC](https://github.com/dotnet-websharper/aspnetmvc) - Run WebSharper applications alongside ASP.NET MVC and include client-side controls in Razor pages.

* [Suave](https://github.com/dotnet-websharper/suave) - Run WebSharper applications as a Suave WebPart.

### Other libraries

* [Data](https://github.com/dotnet-websharper/data) - Proxy for [FSharp.Data](https://fsharp.github.io/FSharp.Data/) which allows using its JsonProvider and WorldBankProvider on the client side.
    * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Core" src="netcore.png"/> Example: [Source](https://github.com/websharper-samples/Data) - [Running live](https://websharper-samples.github.io/Data)

* <a name="html"></a>[WebSharper.Html](https://github.com/dotnet-websharper/html) - a library for constructing server-side and client-side web pages. Superceded by [UI](#ui).

    * <a name="piglets"></a>[Piglets](https://github.com/dotnet-websharper/piglets) - an implementation of "Piglets" for [WebSharper.Html](#html). It provides a concise syntax to define forms and their validation with clear model vs rendering separation of concerns.

    * <a name="formlets"></a>[Formlets](https://github.com/dotnet-websharper/formlets) - a more concise, although less flexible, abstraction similar to [Piglets](#piglets).
    
    * [Formlets.JQueryUI](https://github.com/dotnet-websharper/formlets.jqueryui) - [JQueryUI](#jqueryui) widgets for [Formlets](#formlets).
    
    * [Reactive](https://github.com/dotnet-websharper/reactive) - An imperative reactive programming library. Underlies [Piglets](#piglets) and [Formlets](#formlets).

* [OAuth](https://github.com/dotnet-websharper/oauth) - Authenticate users with external login providers with OAuth 1.0 or 2.0.

### JavaScript library bindings

Using libraries written in JavaScript from WebSharper.

#### 3D and Game engines

* [BabylonJs](https://github.com/dotnet-websharper/babylonjs) - A 3D engine based on WebGL and WebAudio.
    * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Framework" src="netfx.png"/> Example: simple 3D scenes - [Source](https://github.com/websharper-samples/BabylonJS) - [Running live](https://websharper-samples.github.io/BabylonJS/)

* [iioEngine](https://github.com/dotnet-websharper/iioengine) - A 2D engine based on HTML5 Canvas.

* [O3D](https://github.com/dotnet-websharper/o3d) - WebGL-based implementation of the (discontinued) O3D rendering and 3D math engine.
    * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Core" src="netcore.png"/> Example: pool game - [Source](https://github.com/websharper-samples/O3D) - [Running live](https://websharper-samples.github.io/O3D)

* [ThreeJs](https://github.com/dotnet-websharper/threejs) - Leading 3D engine based on WebGL.

    * [ThreeJs.FirstPersonControls](https://github.com/dotnet-websharper/threejs.firstpersoncontrols) - First-person camera controls for Three.js.

    * [ThreeJs.TrackballControls](https://github.com/dotnet-websharper/threejs.trackballcontrols) - Trackball-style camera controls for Three.js.

    * [ThreeJs.TransformControls](https://github.com/dotnet-websharper/threejs.transformcontrols) - Translate/rotate/scale control gizmo for Three.js.
    
    * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Framework" src="netfx.png"/> Example: simple 3D scenes - [Source](https://github.com/websharper-samples/ThreeJS) - [Running live](https://websharper-samples.github.io/ThreeJS/)

#### Browser Capabilities

* [Modernizr](https://github.com/dotnet-websharper/modernizr) - Eaisily detect the browser's capabilities.

* [WebAudio](https://github.com/dotnet-websharper/webaudio) - Audio playback, recording and manipulation.
    * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Framework" src="netfx.png"/> Examples: [Source](https://github.com/websharper-samples/WebAudio) - [Running live](https://websharper-samples.github.io/WebAudio/)

* [WebRTC](https://github.com/dotnet-websharper/webrtc) - Real-Time Communications: media recording and peer-to-peer connections.
    * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Framework" src="netfx.png"/> Examples: [Source](https://github.com/websharper-samples/WebRTC) - [Running live](https://websharper-samples.github.io/WebRTC/)

* [WebSpeech](https://github.com/dotnet-websharper/webspeech) - Speech synthesis and recognition.
    * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Framework" src="netfx.png"/> Examples: [Source](https://github.com/websharper-samples/WebSpeech) - [Running live](https://websharper-samples.github.io/WebSpeech/)

#### Charting and Graphs

* <a name="chartjs"></a>[ChartJs](https://github.com/dotnet-websharper/chartjs) - Simple yet flexible JavaScript charting for designers & developers.
    * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Core" src="netcore.png"/> Example: [Source](https://github.com/websharper-samples/ChartJS) - [Running live](https://websharper-samples.github.io/ChartJS)

* [Cytoscape](https://github.com/dotnet-websharper/cytoscape) - An open source software platform for visualizing complex networks and integrating these with any type of attribute data.
    * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Core" src="netcore.png"/> Example: [Source](https://github.com/websharper-samples/Cytoscape) - [Running live](https://websharper-samples.github.io/Cytoscape)

* [D3](https://github.com/dotnet-websharper/d3) - Data-Driven Documents: A low-level library for data visualization.
    * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Core" src="netcore.png"/> Example: World Tour - [Source](https://github.com/websharper-samples/D3) - [Running live](https://websharper-samples.github.io/D3)

* [Google.Visualization](https://github.com/dotnet-websharper/google.visualization) - Interactive charts.
    * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Framework" src="netfx.png"/> Example: a simple bar chart - [Source](https://github.com/websharper-samples/GoogleVisualization) - [Running live](https://websharper-samples.github.io/GoogleVisualization/)

* <a name="highcharts"></a>[Highcharts](https://github.com/dotnet-websharper/highcharts) - Interactive charts. Includes Highstock for financial data and timeline charts, and Highmaps for interactive map charts.
    * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Framework" src="netfx.png"/> Example: HighCharts, Highmaps and Highstock graphs - [Source](https://github.com/websharper-samples/HighCharts) - [Running live](http://websharper-samples.github.io/HighCharts/)

* [JointJs](https://github.com/dotnet-websharper/jointjs) - Visualize and interact with diagrams and graphs.

* [Peity](https://github.com/dotnet-websharper/peity) - mini SVG pie, donut, line or bar charts.
    * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Core" src="netcore.png"/> Example: [Source](https://github.com/websharper-samples/Peity) - [Running live](https://websharper-samples.github.io/Peity)

* [Rickshaw](https://github.com/dotnet-websharper/peity) - JavaScript toolkit for creating interactive real-time graphs.
    * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Core" src="netcore.png"/> Example: [Source](https://github.com/websharper-samples/Rickshaw) - [Running live](https://websharper-samples.github.io/Rickshaw)

#### Code and text editing

* [Ace](https://github.com/dotnet-websharper/ace) - High-performance code editor for the web.

* [CodeMirror](https://github.com/dotnet-websharper/codemirror) - A versatile text editor implemented in JavaScript for the browser.
    * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Core" src="netcore.png"/> Example: [Source](https://github.com/websharper-samples/CodeMirror) - [Running live](https://websharper-samples.github.io/CodeMirror)

* [Google.CodePrettify](https://github.com/dotnet-websharper/google.codeprettify) - An embeddable script that makes source-code snippets in HTML prettier.

* [HighlightJs](https://github.com/dotnet-websharper/highlightjs) - Syntax highlighting for the Web.
    * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Core" src="netcore.png"/> Example: [Source](https://github.com/websharper-samples/HighlightJS) - [Running live](https://websharper-samples.github.io/HighlightJS)

* [JsPdf](https://github.com/dotnet-websharper/highlightjs) - HTML5 client library for generating PDFs.
    * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Core" src="netcore.png"/> Example: [Source](https://github.com/websharper-samples/JsPDF) - [Running live](https://websharper-samples.github.io/JsPDF)

* [MediumEditor](https://github.com/dotnet-websharper/mediumeditor) - Medium.com WYSIWYG editor clone.
    * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Core" src="netcore.png"/> Example: [Source](https://github.com/websharper-samples/MediumEditor) - [Running live](https://websharper-samples.github.io/MediumEditor)

* [Remarkable](https://github.com/dotnet-websharper/remarkable) - Markdown parser with Commonmark support, extensions, syntax plugins, high speed.
    * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Core" src="netcore.png"/> Example: [Source](https://github.com/websharper-samples/Remarkable) - [Running live](https://websharper-samples.github.io/Remarkable)

* [TinyMce](https://github.com/dotnet-websharper/tinymce) - WYSIWYG rich text editor.
    * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Core" src="netcore.png"/> Example: [Source](https://github.com/websharper-samples/TinyMCE) - [Running live](https://websharper-samples.github.io/TinyMCE)

#### Database

* <a name="mongolab"></a>[MongoLab](https://github.com/dotnet-websharper/mongolab) - Connect to online MongoDB instances.
    * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Framework" src="netfx.png"/> Example: a MongoLab-backed notes application - [Source](https://github.com/websharper-samples/MongoLab) - [Running live](http://websharper-samples.github.io/MongoLab/)

* [PouchDb](https://github.com/dotnet-websharper/mongolab) - CouchDB-inspired in-browser database.

<!-- * [<img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Framework" src="netfx.png"/> PouchDb](https://github.com/websharper-samples/PouchDB) - (not working correctly?) -->

#### GUI and widgets

* [GoldenLayout](https://github.com/dotnet-websharper/goldenlayout) - A multi-screen layout manager for webapps.
    * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Core" src="netcore.png"/> Example: [Source](https://github.com/websharper-samples/GoldenLayout) - [Running live](https://websharper-samples.github.io/GoldenLayout)

* [IntroJs](https://github.com/dotnet-websharper/introjs) - Step-by-step guide and feature introduction for websites.
    * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Core" src="netcore.png"/> Example: [Source](https://github.com/websharper-samples/IntroJS) - [Running live](https://websharper-samples.github.io/IntroJS)

* <a name="jqueryui"></a>[JQueryUI](https://github.com/dotnet-websharper/introjs) - A collection of GUI widgets, animated visual effects, and themes implemented with jQuery.
    * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Core" src="netcore.png"/> Examples: [Source](https://github.com/websharper-samples/JQueryUI) - [Running live](https://websharper-samples.github.io/JQueryUI)

* [MaterialUI](https://github.com/dotnet-websharper/materialui) - Material Design style widgets.

* [SlickGrid](https://github.com/dotnet-websharper/slickgrid) - A fully open-source, javascript, client-side grid control, based on jQuery and jQueryUI and compatible with Bootstrap.

* [SweetAlert](https://github.com/dotnet-websharper/sweetalert) - Customizable JavaScript popup messages.
    * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Core" src="netcore.png"/> Example: [Source](https://github.com/websharper-samples/SweetAlert) - [Running live](https://websharper-samples.github.io/SweetAlert)

* [JQuery.Terminal](https://github.com/dotnet-websharper/terminal) - A plugin for creating command line interpreters in your applications.
    * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Core" src="netcore.png"/> Example: [Source](https://github.com/websharper-samples/JQueryTerminal) - [Running live](https://websharper-samples.github.io/JQueryTerminal)

#### Maps

* [Bing.Maps](https://github.com/dotnet-websharper/bing.maps) - Embedded Microsoft Bing maps.
    * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Core" src="netcore.png"/> Examples: [Source](https://github.com/websharper-samples/Bing.Maps) - [Running live](https://websharper-samples.github.io/Bing.Maps)

* [Google.Maps](https://github.com/dotnet-websharper/google.maps) - Embedded Google maps.
    * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Core" src="netcore.png"/> Examples: [Source](https://github.com/websharper-samples/Google.Maps) - [Running live](https://websharper-samples.github.io/Google.Maps)

* [Google.Maps.MarkerClusterer](https://github.com/dotnet-websharper/google.maps.markerclusterer) - Automatically cluster Google Maps marker by proximity.

* [Leaflet](https://github.com/dotnet-websharper/google.maps.markerclusterer) - Embedded map library that can connect to providers like OpenStreetMap or MapBox.
    * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Core" src="netcore.png"/> Example: [Source](https://github.com/websharper-samples/Leaflet) - [Running live](https://websharper-samples.github.io/Leaflet)

#### Math

* [GlMatrix](https://github.com/dotnet-websharper/glmatrix) - 3D Math library: matrices, quaternions, etc.
    * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Core" src="netcore.png"/> Examples with WebGL: [Source](https://github.com/websharper-samples/GLMatrix) - [Running live](https://websharper-samples.github.io/GLMatrix)

* [MathJax](https://github.com/dotnet-websharper/mathjax) - A JavaScript display engine for mathematics that works in all browsers.
    * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Core" src="netcore.png"/> Example: [Source](https://github.com/websharper-samples/MathJax) - [Running live](https://websharper-samples.github.io/MathJax)

* [MathJs](https://github.com/dotnet-websharper/core/tree/master/src/stdlib/WebSharper.MathJS) - An extensive math library for JavaScript. Includes proxies for .NET types such as `Complex` and `decimal`.
    * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Core" src="netcore.png"/> Example: [Source](https://github.com/websharper-samples/MathJS) - [Running live](https://websharper-samples.github.io/MathJS)

* [Moment](https://github.com/dotnet-websharper/moment) - Parse, validate, manipulate, and display dates and times in JavaScript.
    * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Core" src="netcore.png"/> Example: [Source](https://github.com/websharper-samples/Moment) - [Running live](https://websharper-samples.github.io/Moment)

#### Mobile

* [JQueryMobile](https://github.com/dotnet-websharper/jquerymobile) - A Touch-Optimized Web Framework.

* [PhoneGap](https://github.com/dotnet-websharper/phonegap) - PhoneGap / Cordova bindings to native phone APIs.

* [PhoneJs](https://github.com/dotnet-websharper/phonejs) - Now known as DevExtreme Mobile - Native-looking mobile web applications.

* [Swiper](https://github.com/dotnet-websharper/swiper) - Mobile touch slider focused on performance.
    * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Core" src="netcore.png"/> Example: [Source](https://github.com/websharper-samples/Swiper) - [Running live](https://websharper-samples.github.io/Swiper)

* [HammerJs](https://github.com/dotnet-websharper/hammerjs) - An open-source library that can recognize gestures made by touch, mouse and pointerEvents.
    * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Core" src="netcore.png"/> Example: [Source](https://github.com/websharper-samples/HammerJS) - [Running live](https://websharper-samples.github.io/HammerJS)

#### Reactive libraries

* [KnockoutJs](https://github.com/dotnet-websharper/knockoutjs) - MVVM framework for reactive applications.

* <a name="react"></a>[Facebook React](https://github.com/dotnet-websharper/react) - A JavaScript library for building user interfaces.
    * <img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Core" src="netcore.png"/> Example: a Tic-Tac-Toe game - [Source](https://github.com/dotnet-websharper/react/tree/master/WebSharper.React.Tests) - [Running live](https://dotnet-websharper.github.io/react/)

## Resources

### Blogs

* [The WebSharper team's blog](http://websharper.com/blog) - Official announcements, releases, tutorials.

* [Kimserey Lam's blog](https://kimsereyblog.blogspot.com/search/label/WebSharper)

* [Youenn Bouglouan's blog](http://www.ybouglouan.pl/)

### Sites

* [Try WebSharper](https://try.websharper.com) - Write client-side code in your browser and see it running immediately, in F# or C#.

* [Official documentation](https://developers.websharper.com)

### Academic publications

* Loic Denuziere, Adam Granicz. **Enabling modular persistence for reactive data models in F# client-server web applications**. In *Modularity*, Malaga, Spain, 2016. [ACM](https://dl.acm.org/citation.cfm?id=2892672)

* Adam Granicz, Loic Denuziere. **Functional, Reactive Web Programming in F#**. In *Central European Functional Programming School* (CEFP), Budapest, Hungary, 2015, pp. 137-160. [Springer](https://link.springer.com/chapter/10.1007/978-3-030-28346-9_5)

* Simon Fowler, Loic Denuziere, Adam Granicz. **Reactive Single-Page Applications with Dynamic Dataflow**. In *Practical Aspects of Declarative Languages* (PADL), Portland, OR, USA. 2015. [Springer](https://link.springer.com/chapter/10.1007/978-3-319-19686-2_5), **[PDF1](http://simonjf.com/writing/padl2015.pdf)**, [PDF2](https://www.researchgate.net/publication/300890501_Reactive_Single-Page_Applications_with_Dynamic_Dataflow)

* Loic Denuziere, Adam Granicz, Simon Fowler. **Reactive Abstractions for Functional Web Applications**. Submitted to *Implementation and Application of Functional Languages* (IFL), Koblenz, Germany, 2015. **[PDF](https://pdfs.semanticscholar.org/eb57/611ccb0c8c2ef4beeed2709cfa37444a068a.pdf)**

* Adam Granicz. **Functional Web and Mobile Development in F#**. In *Central European Functional Programming School* (CEFP), Budapest, Hungary, 2013, pp. 381-406. [Springer](https://link.springer.com/chapter/10.1007/978-3-319-15940-9_9)

* Loic Denuziere, Ernesto Rodriguez, Adam Granicz. **Piglets to the Rescue: Declarative User Interface Specification with Pluggable View Models**. In Symposium on Implementation and Application of Functional Languages (IFL), Nijmegen, The Netherlands, 2013. [ACM](https://dl.acm.org/citation.cfm?id=2620689), **[PDF](http://www.cs.ru.nl/P.Achten/IFL2013/symposium_proceedings_IFL2013/ifl2013_submission_29.pdf)**.

* Loic Denuziere, Adam Granicz, Anton Tayanovskyy. **Visualizing data on the web**. In *Data-driven Functional Programming* (DDFP), Rome, Italy, 2013, pp. 19-22. [ACM](https://dl.acm.org/citation.cfm?id=2429383)

* Joel Bjornson, Anton Tayanovskyy, Adam Granicz. **Composing Reactive GUIs in F# Using WebSharper**. In Symposium on Implementation and Application of Functional Languages (IFL), Alphen aan den Rijn, The Netherlands, 2010. pp. 203-216. [Springer](https://link.springer.com/chapter/10.1007/978-3-642-24276-2_13)

* Alex Peake, Adam Granicz. **The first substantial line of business application in F#**. In *Commercial Users of Functional Programming* (CUFP), Tokyo, Japan, 2009.
