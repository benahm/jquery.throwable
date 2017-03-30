JQuery.throwable
================

JQuery plugin to make HTML elements throwable 

Create physical-like HTML objects in your browser

## Code example
```javascript
$(".box2d").throwable({
                        containment:[0,0,500,500],
                        drag:true,
                        gravity:{x:0,y:0},
                        impulse:{
                            f:52,
                            p:{x:1,y:1}
                        },
                        shape:"circle",
                        autostart:false,
                        bounce:0.5,
                        damping:100,
                        areaDetection:[[0,0,300,300]],
                        collisionDetection: true
                    });
```
## Options 
```javascript
* gravity: object {x:valueX,y:valueY} 
* container: define the limits where the object can be thrown 
                   "window" is the default
                   "parent" the object will be contained inside the parent
                   you can specify custom a container by giving array [x1,y1,x2,y2]
* shape: defines the shape of the object, by default is "box" and you can specify "circle"
* autostart: by default the effects start at mouse move 
* drag: boolean to specify if the object will be draggable or not, by default it is set to true
* impulse: you can specify an impluse to apply on the object by giving an object 
                   {
                        f: forceValue, // define the energy of the impluse (number)
                        p: pointDirection //define the direction on the impluse object like the gravity option
                   }
* bounce: defines the bounce effect of the body (value between 0 and 1) default 0, no bounce
* damping: defines the damping(*) effect value from 0 to infini, default 0 
* areaDetection: specify an array of areas, that when an objet enter those areas the event inarea is fired 
                 and outarea event fired when exiting
* collisionDectection : bool to activate or desactivate the collision detection 
```
(*) : [damping](http://en.wikipedia.org/wiki/Damping)

## Events & Callbacks
```javascript
* inarea : fired when an object enter and area specified in the option areaDetection
* outarea : fired when an object exit and area specified in the option areaDetection
* collision : fired when a collision happened between two objects 
* nocollision : fired when there is no collision 
```
## Requirements
    * JQuery (of course it's a jquery plugin)


## Demos
* Check out this simple demo here [Octocats Demo](http://benahm.github.com/jquery.throwable/octocats.html)<br>
* Applying gravity per selection of elements [Gravity per element](http://benahm.github.com/jquery.throwable/gravityperelement.html)
* Another demo [Slider demo](http://benahm.github.com/jquery.throwable/slider.html)<br>
* Demo of collision detection and area detection [here](http://benahm.github.com/jquery.throwable/demoevents.html)
* Billard js [Play Billard](http://benahm.github.io/jquery.throwable/billardjs.html)

## Credits
* Mr. Doobs : http://mrdoob.com/92/Google_Gravity
* Alex Arnell's inheritance.js : http://code.google.com/p/inheritance/
* Box2Djs : http://box2d-js.sourceforge.net/
* JQuery-ui draggable : http://api.jqueryui.com/draggable/

## How to use it!
You can test it by including this js link to your page
```html
<script src="http://benahm.github.io/jquery.throwable/javascripts/jquery.throwable.js" type="text/javascript"></script> 
```
Or download the <a href="http://benahm.github.io/jquery.throwable/javascripts/jquery.throwable.js">js file</a>


