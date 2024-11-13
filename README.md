# 9103-01-final
I use my work to do an iPad prototype.
Interactive iPad Interface with Lock Screen and Img Screens
This project simulates an iPad-like interface prototype with multiple interactive features, including a lock screen, password input, image screens and adaptive resizing. The display can switch between two images screens (img1 and img2) and includes a simulated lock screen that requires password input to unlock.

Features
Image Screens: Click the return (white circle ) button on the right side of the silver border to shift between two images, img1 and img2.
Lock Screen: Click the gray rectangle "lock screen button" (positioned slightly above the center) to activate a lock screen that covers the current display with a black overlay.
Password Input: On the lock screen, enter any numeric input as the password, and the display will unlock to show img2.
Responsive Design: All elements, including the images, borders, buttons, and lock screen inputs, resize based on the window dimensions for a consistent user experience.

Code Breakdown
Main Components
Image Screens and Lock Screen Button:
The white circle acts as a return button to switch between the main images (img1 and img2).
The gray rectangle at the left of the silver border functions as a lock screen button.
Lock Screen and Password Input:
When the lock screen is active, a black overlay covers the image area, and an input field appears for password entry.
Any numeric input is accepted as a correct password, unlocking the screen and displaying img2.
Resizable Elements:
The images and interactive elements scale with the screen size to maintain proportions.

Code Functions
drawImageWithSegments(): Displays segmented parts of img1 or img2 within the image area.
checkPassword(): Verifies the input password; any numeric input unlocks the display and shows img2.
mousePressed(): Handles click events, including toggling between images and activating the lock screen.
windowResized(): Ensures the canvas resizes when the window dimensions change, maintaining responsive elements.
External Reference
This project includes a password demo functionality adapted from Mahdadbor's "password demo" on p5.js:

Mahdadbor, "password demo," available at https://editor.p5js.org/mahdadbor/sketches/cEwKTI5m3, accessed on [2024.11.13].

Usage
Initial View: The canvas initially displays img1 or img2.
Toggle Images: Click the white circle on the right side of the silver border to switch between img1 and img2.
Activate Lock Screen: Click the gray rectangle (lock screen button) to activate the black screen.
Enter Password: Type any numeric value in the password input field. Correct passwords will display img2.
