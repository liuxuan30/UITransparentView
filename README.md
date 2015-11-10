# UITransparentView

This is a very useful UIView when you want to make it transparent, and other views beneath it can still get touch events.

If this tranparent view has sub views, it will not ignore touch events, instead, it will capture it.

Be noted, if the view.alpha is set to 0, the event will never be dispatched to the view. The transparent view's purpose is just to make it as if its alpha = 0 while still being able to capture touch events.

There are plenty of ways to make use of it, as long as you get the point how `pointInSide` is implemented.

Implemented by John Stephen, for more details, check http://stackoverflow.com/questions/3046813/how-can-i-click-a-button-behind-a-transparent-uiview

I just cannot stop sharing it for such a great piece of code.

# 3D Touch on iOS 9 attention:
seems 3D Touch had different implementation, be careful if you enable allowMoving, the gesture won't ended, still under investigation.
