# PyINPUT

## PyINPUT_RECORD Object

Interface to the INPUT_RECORD struct used with console IO functions.  Create using PyINPUT_RECORDType(EventType)

#### Comments
Only attributes that apply to each particular EventType can be accessed:
KEY_EVENT: KeyDown, RepeatCount, VirtualKeyCode, VirtualScanCode, ControlKeyState
MOUSE_EVENT: MousePosition, ButtonState, ControlKeyState, EventFlags
WINDOW_BUFFER_SIZE_EVENT: Size
FOCUS_EVENT: SetFocus
MENU_EVENT: CommandId


#### Properties

  -  __int EventType__ 
    One of KEY_EVENT, MOUSE_EVENT, WINDOW_BUFFER_SIZE_EVENT, MENU_EVENT, FOCUS_EVENT. Cannot be changed after object is created

  -  __boolean KeyDown__ 
    True for a key press, False for key release

  -  __int RepeatCount__ 
    Nbr of repeats generated (key was held down if &gt1)

  -  __int VirtualKeyCode__ 
    Device-independent key code, win32con.VK_*

  -  __int VirtualScanCode__ 
    Device-dependent scan code generated by keyboard

  -  __[PyUnicode](#pyunicode)Char__ 
    Single unicode character generated by the keypress

  -  __int ControlKeyState__ 
    State of modifier keys, combination of CAPSLOCK_ON, ENHANCED_KEY, LEFT_ALT_PRESSED, 

LEFT_CTRL_PRESSED, NUMLOCK_ON, RIGHT_ALT_PRESSED, RIGHT_CTRL_PRESSED, SCROLLLOCK_ON, SHIFT_PRESSED

  -  __int ButtonState__ 
    Bitmask representing which mouse buttons were pressed.

  -  __int EventFlags__ 
    DOUBLE_CLICK, MOUSE_MOVED or MOUSE_WHEELED, or 0.  If 0, indicates a mouse button press

  -  __[PyCOORD](#pycoord)MousePosition__ 
    Position in character coordinates

  -  __[PyCOORD](#pycoord)Size__ 
    New size of screen buffer in character rows/columns

  -  __boolean SetFocus__ 
    Reserved - Used only with type FOCUS_EVENT.  This event is Reserved, and should be ignored.

  -  __int CommandId__ 
    Used only with event type MENU_EVENT, which is reserved and should not be used