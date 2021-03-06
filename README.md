YISwipeShiftCaret
=================

Swipe-to-shift text input caret for iOS (no private APIs)

<img src="https://github.com/downloads/inamiy/YISwipeShiftCaret/screenshot.png" alt="ScreenShot1" width="225px" style="width:225px;" />

Above screenshot is from [WordBook App](https://itunes.apple.com/jp/app/id495453330?mt=8) using [YIPopupTextView](https://github.com/inamiy/YIPopupTextView/commit/28a85245691076121ff85d1698ca455683437a5a).

This project is based on this [commit](https://github.com/inamiy/YIPopupTextView/commit/28a85245691076121ff85d1698ca455683437a5a).

How to use
----------
```
- (BOOL)application:(UIApplication *)application didFinishLaunchingWithOptions:(NSDictionary *)launchOptions
{
    // add swipe-shift-caret gestures to all of UITextField/UITextView
    [YISwipeShiftCaret install];
    
    //
    // or, you can implement gestures manually as follows, adding to non-textInput (wider parent) view:
    //
    // YISwipeShiftCaretGestureRecognizer* gesture = [[YISwipeShiftCaretGestureRecognizer alloc] initWithTextInput:self.textField];
    // [self.window addGestureRecognizer:gesture];
    
    return YES;
}

```

License
-------
YISwipeShiftCaret is available under the Beerware license.