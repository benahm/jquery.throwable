jquery.throwable
================

JQuery plugin to make html element throwable <br>

Create physical-like html object in your browser
## Code exemple

    $(".box2d").throwable({
                            containment:[0,0,500,500],
                            drag:true,
                            gravity:{x:0,y:0},
                            impulse:{
                                f:52,
                                p:{x:1,y:1}
                            },
                            shape:"circle"
                        });

## Options 
    * gravity: object {x:valueX,y:valueY} 
    * containment: define the limits where the object can be dragged
                   default window 
                   you can specify custom containment by giving array [x1,y1,x2,y2]
    * shape: define the shape of the object by default "box" and you can specify "circle"
    * drag: boolean to specify if the object will be draggable or not, by default true
    * impulse: you can specify un impluse to apply on the object by giving an object 
                   {f: define the energy of the impluse (number)
                   p: define the direction on the impluse object like the gravity option
    
## Events
    * no events, Work in progress

## Requirements
    * JQuery (of course it's a jquery plugin)


##Demos
* Check out this simple demo here [Octocats Demo](http://benahm.github.com/jquery.throwable/octocats.html)<br>
* Applying gravity per selection of elements [Gravity per element](http://benahm.github.com/jquery.throwable/gravityperelement.html)
* An other demo [Slider demo](http://benahm.github.com/jquery.throwable/slider.html)<br>

## Credits
* Mr. Doobs :: http://mrdoob.com/92/Google_Gravity
* Alex Arnell's inheritance.js :: http://code.google.com/p/inheritance/
* Box2Djs :: http://box2d-js.sourceforge.net/

You can find the documentation about the plugin at [JQuery.throwable page](http://benahm.github.com/jquery.throwable/)
