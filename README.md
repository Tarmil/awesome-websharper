# Awesome WebSharper

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of WebSharper libraries, samples and resources.

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
## Table of Contents

- [Examples](#examples)
  - [Applications](#applications)
  - [Library demos](#library-demos)
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

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

## Examples

* <img width="20" alt="F#" src="fsharp.png"/> = Written in F#
* <img width="20" alt="C#" src="csharp.png"/> = Written in C#
* <img width="20" alt=".NET Core" src="netcore.png"/> = Written for .NET Core
* <img width="20" alt=".NET Framework" src="netfx.png"/> = Written for .NET Framework

### Applications

* [<img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Framework" src="netfx.png"/> 2048](https://github.com/intellifactory/2048) - The well-known game 2048 reimplemented in F#, with a few custom rule options.

* [<img width="20" alt="C#" src="csharp.png"/> <img width="20" alt=".NET Framework" src="netfx.png"/> BookCollection](https://github.com/websharper-samples/BookCollection) - A client-server CRUD application using remoting and a reactive client side, with [full tutorial](https://github.com/websharper-samples/BookCollection/blob/master/BookCollection.md).

* <a name="LoginWithBulma"></a>[<img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Core" src="netcore.png"/> LoginWithBulma](https://github.com/websharper-samples/LoginWithBulma) - A client-side login page using HTML templating, with full tutorial.

* [<img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Core" src="netcore.png"/> Counter](https://github.com/websharper-samples/Counter) - Follow-up to [LoginWithBulma](#LoginWithBulma): A client-side Model-View-Update-style counter, with full tutorial.

* [<img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Framework" src="netfx.png"/> REST API](https://github.com/intellifactory/rest-api.sample) - A simple CRUD REST API.

* [<img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Framework" src="netfx.png"/> MVU TodoMVC](https://github.com/dotnet-websharper/mvu/tree/master/WebSharper.Mvu.TodoMvc) - The classic TodoMVC app written with UI and [MVU](#mvu).

* [<img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Framework" src="netfx.png"/> TodoMVC](https://github.com/intellifactory/samples.todomvc) - The classic TodoMVC app written with UI.

### Library demos

* [<img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Framework" src="netfx.png"/> BabylonJs](https://github.com/intellifactory/websharper.babylonjs.samples) - simple 3D scenes.

* [<img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Framework" src="netfx.png"/> Google Visualization](https://github.com/intellifactory/websharper.googlevisualization.sample) - A simple bar chart with Google Visualization.

* [<img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Framework" src="netfx.png"/> HighCharts](https://github.com/intellifactory/websharper.highcharts.samples) - [Highcharts](#highcharts), Highmaps and Highstock graphs.

* [<img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Framework" src="netfx.png"/> MongoLab](https://github.com/intellifactory/websharper.mongolab.samples) - A [MongoLab](#mongolab)-backed notes application.

<!-- * [<img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Framework" src="netfx.png"/> PouchDb](https://github.com/intellifactory/websharper.pouchdb.samples) - (not working correctly?) -->

* [<img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Framework" src="netfx.png"/> ThreeJs](https://github.com/intellifactory/websharper.threejs.samples) - simple 3D scenes.

* [<img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Framework" src="netfx.png"/> UI Samples](https://github.com/intellifactory/websharper.ui.next.samples) - A set of samples to discover the UI reactive library.

* [<img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Framework" src="netfx.png"/> WebAudio](https://github.com/intellifactory/websharper.webaudio.samples) - Play and manipulate audio.

* [<img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Framework" src="netfx.png"/> WebRTC](https://github.com/intellifactory/websharper.webrtc.samples) - Record audio and video.

* [<img width="20" alt="F#" src="fsharp.png"/> <img width="20" alt=".NET Framework" src="netfx.png"/> WebSpeech](https://github.com/intellifactory/websharper.webspeech.samples) - Speech synthesis and recognition.


## Libraries

Libraries written with and for WebSharper.

### Reactive libraries

* <a name="ui"></a>[UI](https://github.com/dotnet-websharper/ui) (formerly known as UI.Next) - a library for constructing server-side and reactive client-side web pages in plain C#, F#, or with HTML templates.

    * <a name="forms"></a>[Forms](https://github.com/dotnet-websharper/forms) - an implementation of "Piglets" for UI. It provides a concise syntax to define forms and their validation with clear model vs rendering separation of concerns.
    
    * [Forms.Bootstrap](https://github.com/dotnet-websharper/forms.bootstrap) - Bootstrap-based widgets for [Forms](#forms).

    * [UI.Formlets](https://github.com/dotnet-websharper/ui.formlets) - a more concise, although less flexible, abstraction similar to [Forms](#forms).

    * [Charting](https://github.com/dotnet-websharper/charting) - An API for client-side charts similar to FSharp.Charting. Includes [ChartJs](#chartjs)-based rendering, but has back-end extensibility.
    
    * <a name="mvu"></a>[MVU](https://github.com/dotnet-websharper/mvu) - Model-View-Update (Elm-like) architecture for full client-side applications.

### Server-side hosting

* [Owin](https://github.com/dotnet-websharper/owin) - OWIN defines a standard interface between .NET web servers and web applications. This library allows hosting WebSharper applications on any OWIN-compliant host - ASP.NET, Katana, Suave, etc.

* [Owin.WebSocket](https://github.com/dotnet-websharper/owin.websocket) - Client-side and server-side WebSockets interface for OWIN-hosted applications, including automated serialization of messages.

* [ASP.NET Core](https://github.com/dotnet-websharper/aspnetcore) - Run WebSharper applications on ASP.NET Core.

* [ASP.NET MVC](https://github.com/dotnet-websharper/aspnetmvc) - Run WebSharper applications alongside ASP.NET MVC and include client-side controls in Razor pages.

* [Suave](https://github.com/dotnet-websharper/suave) - Run WebSharper applications as a Suave WebPart.

### Other libraries

* [Data](https://github.com/dotnet-websharper/data) - Proxy for [FSharp.Data](https://fsharp.github.io/FSharp.Data/) which allows using its JsonProvider and WorldBankProvider on the client side.

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

* [iioEngine](https://github.com/dotnet-websharper/iioengine) - A 2D engine based on HTML5 Canvas.

* [O3D](https://github.com/dotnet-websharper/o3d) - WebGL-based implementation of the (discontinued) O3D rendering and 3D math engine.

* [ThreeJs](https://github.com/dotnet-websharper/threejs) - Leading 3D engine based on WebGL.

    * [ThreeJs.FirstPersonControls](https://github.com/dotnet-websharper/threejs.firstpersoncontrols) - First-person camera controls for Three.js.

    * [ThreeJs.TrackballControls](https://github.com/dotnet-websharper/threejs.trackballcontrols) - Trackball-style camera controls for Three.js.

    * [ThreeJs.TransformControls](https://github.com/dotnet-websharper/threejs.transformcontrols) - Translate/rotate/scale control gizmo for Three.js.

#### Browser Capabilities

* [Modernizr](https://github.com/dotnet-websharper/modernizr) - Eaisily detect the browser's capabilities.

* [WebAudio](https://github.com/dotnet-websharper/webaudio) - Audio playback, recording and manipulation.

* [WebRTC](https://github.com/dotnet-websharper/webrtc) - Real-Time Communications: media recording and peer-to-peer connections.

* [WebSpeech](https://github.com/dotnet-websharper/webspeech) - Speech synthesis and recognition.

#### Charting and Graphs

* <a name="chartjs"></a>[ChartJs](https://github.com/dotnet-websharper/chartjs) - Simple yet flexible JavaScript charting for designers & developers.

* [Cytoscape](https://github.com/dotnet-websharper/cytoscape) - An open source software platform for visualizing complex networks and integrating these with any type of attribute data.

* [D3](https://github.com/dotnet-websharper/d3) - Data-Driven Documents: A low-level library for data visualization.

* [Google.Visualization](https://github.com/dotnet-websharper/google.visualization) - Interactive charts.

* <a name="highcharts"></a>[Highcharts](https://github.com/dotnet-websharper/highcharts) - Interactive charts. Includes Highstock for financial data and timeline charts, and Highmaps for interactive map charts.

* [JointJs](https://github.com/dotnet-websharper/jointjs) - Visualize and interact with diagrams and graphs.

* [Peity](https://github.com/dotnet-websharper/peity) - mini SVG pie, donut, line or bar charts.

* [Rickshaw](https://github.com/dotnet-websharper/peity) - JavaScript toolkit for creating interactive real-time graphs.

#### Code and text editing

* [Ace](https://github.com/dotnet-websharper/ace) - High-performance code editor for the web.

* [CodeMirror](https://github.com/dotnet-websharper/codemirror) - A versatile text editor implemented in JavaScript for the browser.

* [Google.CodePrettify](https://github.com/dotnet-websharper/google.codeprettify) - An embeddable script that makes source-code snippets in HTML prettier.

* [HighlightJs](https://github.com/dotnet-websharper/highlightjs) - Syntax highlighting for the Web.

* [JsPdf](https://github.com/dotnet-websharper/highlightjs) - HTML5 client library for generating PDFs.

* [MediumEditor](https://github.com/dotnet-websharper/mediumeditor) - Medium.com WYSIWYG editor clone.

* [Remarkable](https://github.com/dotnet-websharper/remarkable) - Markdown parser with Commonmark support, extensions, syntax plugins, high speed.

* [TinyMce](https://github.com/dotnet-websharper/tinymce) - WYSIWYG rich text editor.

#### Database

* <a name="mongolab"></a>[MongoLab](https://github.com/dotnet-websharper/mongolab) - Connect to online MongoDB instances.

* [PouchDb](https://github.com/dotnet-websharper/mongolab) - CouchDB-inspired in-browser database.

#### GUI and widgets

* [GoldenLayout](https://github.com/dotnet-websharper/goldenlayout) - A multi-screen layout manager for webapps.

* [IntroJs](https://github.com/dotnet-websharper/introjs) - Step-by-step guide and feature introduction for websites.

* <a name="jqueryui"></a>[JQueryUI](https://github.com/dotnet-websharper/introjs) - A collection of GUI widgets, animated visual effects, and themes implemented with jQuery.

* [MaterialUI](https://github.com/dotnet-websharper/materialui) - Material Design style widgets.

* [SlickGrid](https://github.com/dotnet-websharper/slickgrid) - A fully open-source, javascript, client-side grid control, based on jQuery and jQueryUI and compatible with Bootstrap.

* [SweetAlert](https://github.com/dotnet-websharper/sweetalert) - Customizable JavaScript popup messages.

* [JQuery.Terminal](https://github.com/dotnet-websharper/terminal) - A plugin for creating command line interpreters in your applications.

#### Maps

* [Bing.Maps](https://github.com/dotnet-websharper/bing.maps) - Embedded Microsoft Bing maps.

* [Google.Maps](https://github.com/dotnet-websharper/google.maps) - Embedded Google maps.

* [Google.Maps.MarkerClusterer](https://github.com/dotnet-websharper/google.maps.markerclusterer) - Automatically cluster Google Maps marker by proximity.

* [Leaflet](https://github.com/dotnet-websharper/google.maps.markerclusterer) - Embedded map library that can connect to providers like OpenStreetMap or MapBox.

#### Math

* [GlMatrix](https://github.com/dotnet-websharper/glmatrix) - 3D Math library: matrices, quaternions, etc.

* [MathJax](https://github.com/dotnet-websharper/mathjax) - A JavaScript display engine for mathematics that works in all browsers.

* [MathJs](https://github.com/dotnet-websharper/core/tree/master/src/stdlib/WebSharper.MathJS) - An extensive math library for JavaScript. Includes proxies for .NET types such as `Complex` and `decimal`.

* [Moment](https://github.com/dotnet-websharper/moment) - Parse, validate, manipulate, and display dates and times in JavaScript.

#### Mobile

* [JQueryMobile](https://github.com/dotnet-websharper/jquerymobile) - A Touch-Optimized Web Framework.

* [PhoneGap](https://github.com/dotnet-websharper/phonegap) - PhoneGap / Cordova bindings to native phone APIs.

* [PhoneJs](https://github.com/dotnet-websharper/phonejs) - Now known as DevExtreme Mobile - Native-looking mobile web applications.

* [Swiper](https://github.com/dotnet-websharper/swiper) - Mobile touch slider focused on performance.

* [HammerJs](https://github.com/dotnet-websharper/hammerjs) - An open-source library that can recognize gestures made by touch, mouse and pointerEvents.

#### Reactive libraries

* [KnockoutJs](https://github.com/dotnet-websharper/knockoutjs) - MVVM framework for reactive applications.

* [Facebook React](https://github.com/dotnet-websharper/react) - A JavaScript library for building user interfaces.

## Resources

TODO
