Hand Gesture Control System.
Overview.
A touch-free computer interaction system that uses hand gestures to control your computer's mouse, volume, and screen brightness through your webcam.

Features.
Mouse Control: Move cursor with hand movements.
Click Gestures: Perform left/right clicks.
Scroll: Vertical and horizontal scrolling.
System Controls: Adjust volume and screen brightness.
Zoom: Pinch to zoom in/out.
Drag & Drop: Intuitive drag and drop functionality.
Prerequisites.
Python 3.6+.
Webcam.
Windows OS (for system volume/brightness controls).
Installation.
Install required packages:
pip install opencv-python mediapipe pyautogui pycaw screen-brightness-control numpy comtypes.
How to Use.
Run the application:
python gesture_control2.py.
Position yourself 1-2 meters from the webcam.
Use these gestures:
Gesture Controls.
V_GEST (Victory Sign).
Function: Mouse Movement.
How to use: Show a "V" sign with your index and middle fingers.
The cursor will follow your hand movement.
This is the base gesture for many other actions.
FIST (Closed Hand).
Function: Drag and Drop.
How to use: Close all fingers into a fist.
Must hold for 1 second to activate.
Click and hold to drag items.
Release to drop.
INDEX (Index Finger Up).
Function: Right Click.
How to use: Point only your index finger up, keep other fingers down.
Only works after showing V_GEST first.
Performs a right-click action.
MID (Middle Finger Up).
Function: Left Click.
How to use: Point only your middle finger up, keep other fingers down.
Only works after showing V_GEST first.
Performs a left-click action.
TWO_FINGER_CLOSED.
Function: Double Click.
How to use: Show index and middle fingers close together.
Only works after showing V_GEST first.
Performs a double-click action.
PINCH_MAJOR (Dominant Hand Pinch).
Function: Volume and Brightness Control.
How to use: Pinch thumb and index finger on your dominant hand.
While pinching:
Move up/down to control volume.
Move left/right to control screen brightness.
The more you move, the more it changes.
PINCH_MINOR (Non-dominant Hand Pinch).
Function: Scroll Control.
How to use: Pinch thumb and index finger on your non-dominant hand.
While pinching:
Move up/down to scroll vertically.
Move left/right to scroll horizontally.
The more you move, the more it scrolls.
INDEX (without V_GEST).
Function: Quick Scroll.
How to use: Point only your index finger up.
Move your finger up/down to scroll.
More responsive than pinch scrolling.
THUMBS_UP.
Function: Volume Up.
How to use: Show thumbs up gesture.
Increases system volume.
THUMBS_DOWN.
Function: Volume Down.
How to use: Show thumbs down gesture.
Decreases system volume.
Important Notes.
Some gestures require the V_GEST first (like right-click, left-click, double-click).
The system has a 0.5-second cooldown between gestures.
FIST gesture requires a 1-second hold to activate.
PINCH gestures are more precise but slower than direct gestures.
The system uses your dominant hand (right by default) for major controls and non-dominant hand for minor controls.
Troubleshooting.
Ensure good lighting.
Keep background simple.
Make gestures clearly and deliberately.
Check webcam permissions.
Demo.
See the demo/ folder for example videos of all features.

Note.
For best results, use against a plain background with good lighting. The system works best with one hand at a time.
