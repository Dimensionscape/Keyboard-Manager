# Keyboard Manager
 Lightweight Manager for keyboard control in openfl applications

Usage:
```haxe
KeyboardManager.start(stage);

function onXPressed(){
  trace("X Key Pressed");
}

KeyboardManager.setKeyDownCallback(X, onXPressed);

//output: X Key Pressed
```

```haxe
KeyboardManager.start(stage);

function onEnterFrame(e:Event){
 trace(KeyboardManager.isKeyDown(X));
}

addEventListener(Event.ENTER_FRAME, onEnterFrame);

//output: false
```
