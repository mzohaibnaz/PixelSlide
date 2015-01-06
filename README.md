PixelSlide jQuery Slider Plugin
================================
PixelSlide is very simple but useful jquery slide plugin.
its work in vertical direction as well as horizontal.

Why we use PixelSlide?
======================
PixelSlide is simple to use with key of many options to control your slider.
You can use PixelSlide as many time on your site with both directions (vertical/horizontal).

Lets see how PixelSlide works
=====================================================
First download the source code from GitHub
and extract files you will get folder with name PixelSlide

i also included demos in this package too see how PixelSlide will work.


=====================================================
PixelSlide HTML Structure
=====================================================
> <div class="pixelSlide_Container">
>    <span><img src="thumb03.jpg" /></span>
>    <span><img src="thumb04.jpg" /></span>
>    <span><img src="thumb05.jpg" /></span>
>    ....
> </div>

I added (pixelSlide_Container) class on div you can use any name as you like for use in jquery.

you and also and optional html structure as you like for next/prev/start/pause buttons - Example
- note these htmls are options if you don't mention PixelSlide will generate automatically.
- But the Start/Pause button is conditional if you run PixelSlide as auto slide mode then html will be generated.

> <div class="main_container">

>    <a href="#" class="prev">Prev</a>
>    <a href="#" class="next">Next</a>
>    <a href="#" class="start">Start</a>
>    <a href="#" class="Pause">Pause</a>
    
>    <div class="pixelSlide_Container">
>        <span><img src="thumb03.jpg" /></span>
>        <span><img src="thumb04.jpg" /></span>
>        <span><img src="thumb05.jpg" /></span>
>        ....
>    </div>
> </div>

i added for links with class to control slider and we will use these classed on jquery lets move on jquery

=====================================================
How to Use PixelSlide in jQuery
=====================================================

first you need to include jQuery and PixelSlide files on document head tag - Example

> <html>
>    <head>
>        <script type="text/javascript" src="js/jquery-1.11.0.min.js"></script>
>        <script type="text/javascript" src="js/pixelSlide.min.js"></script>
>    </head>
>    <body>
>        ....
>    </body>
> </html>

now you just need to call PixelSlide plugin now lets take look on all code.

><html>
>    <head>
>        <script type="text/javascript" src="js/jquery-1.11.0.min.js"></script>
>        <script type="text/javascript" src="js/pixelSlide.min.js"></script>
>        <script type="text/javascript">
>            $(document).ready(function(){
>                // here call pixelSlide
>                $(".scroller_contents").pixelSlide({
>                    width: 300,
>                    nextBtn: ".next",
>                    prevBtn: ".prev",
>                    speed: 500,
>                    margin: 14,
>                    mode: "horizontal",
>                    auto: true
>                });
>            });
>        </script>
>    </head>
>    <body>
>        <div class="main_container">
>            <a href="#" class="prev">Prev</a>
>            <a href="#" class="next">Next</a>
>            <a href="#" class="start">Start</a>
>            <a href="#" class="Pause">Pause</a>
            
>            <div class="pixelSlide_Container">
>                <span><img src="thumb03.jpg" /></span>
>                <span><img src="thumb04.jpg" /></span>
>                <span><img src="thumb05.jpg" /></span>
>                ....
>            </div>
>        </div>
>    </body>
></html>


-------------------------------------------
Parameters of PixelSlide Plugin
-------------------------------------------
      // These are the defaults.
      width: 260,           // lets PixelSlide to know how much width of your each span or item to slider horizontal perfectally
      height: 190,          // lets PixelSlide to know how much width of your each span or item to slider vertical perfectally
      items: 3,             // lets PixelSlide to know how much items you want to slide each time or how much item is displaying
      nextBtn: false,       // provide id or class for next slide - default is .next
      prevBtn: false,       // provide id or class for previous slide - default is .prev
      pauseBtn: false,      // provide id or class for Pause Slider - default is .pauseBtn
      startBtn: false,      // provide id or class for Start Slider - default is .next
      mode: "horizontal",   // set to run PixelSlide run (vertical/horizontal)
      margin: 10,           // lets PixelSlide to know how much margin is between items to slide in perfect position
      speed: 1000,          // enter time to how much milliseconds time takes by each slide
      auto: false,          // run slider auto without click on next or previous buttons
      autoSpeed: 2000,      // how much speed for run auto
      toggleClass: false    // add class for toggle . it will be added on next/prev/start/pause buttons when its hide . if its false then slider will automatically hide buttons

And Thats All.

Thank you!
Follow me @Facebook: https://www.facebook.com/zebi.rajpot