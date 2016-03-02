## Building your very own iOS Calculator App

#### Introduction:
This tutorial is aimed for anyone who wants to learn how to build an iOS Application. This tutorial will guide users on how to build a calculator application for iPhone in order to teach the basic building blocks of mobile application development. 

#### Necessary Equipment:
- Mac Computer with Xcode installed
+ Xcode can be found in the Mac App store.
- Internet Connection   
- Basic skills on how to user a computer (i.e. how to use a mouse / keyboard)

### Step 1: Creating a new Project and Getting familiar with Xcode
In this section you will create the Xcode project and get yourself familiar with the development environment.

1. Open Xcode<br /><br />
2. Select "Create a new Xcode Project" <br /><br />
<img src="https://raw.githubusercontent.com/fnk0/iOS-Calculator-Tutorial/master/Calculator/images/fig1.png" alt="Figure 1" style="width: 600px;"/> <br />
_Figure 1_ <br /><br /><br /><br /><br /><br /><br />
3. Select "Single View Application" and click "Next" <br /><br />
<img src="https://raw.githubusercontent.com/fnk0/iOS-Calculator-Tutorial/master/Calculator/images/fig2.png" alt="Figure 2" style="width: 600px;"/> <br />
_Figure 2_ <br /><br />
4. Give the App (i.e. Product Name) a name and a organization identifier. <br />
**Note:** _The organization is usually a company's domain name in reverse, but for our purposes we will justbe using **com.last name**. In my case it will be **com.gabilheri**_ <br /><br />
5. Select the language to be Swift<br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />
6. Select iPhone in the devices Dropdown. You should now have something similar to Figure 3. <br /><br />
<img src="https://raw.githubusercontent.com/fnk0/iOS-Calculator-Tutorial/master/Calculator/images/fig3.png" alt="Figure 3" style="width: 600px;"/> <br />
_Figure 3_ <br /><br /><br />
7. Click **next** to select where to save and then **create** to create the project. Depending on the speed of your computer this might take a couple of minutes.
<br /><br />
8. After the project has been created, Xcode will open the project and you should see something like Figure 4. <br /><br />
<br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />
<img src="https://raw.githubusercontent.com/fnk0/iOS-Calculator-Tutorial/master/Calculator/images/fig4.png" alt="Figure 4" style="width: 600px;"/> <br />
_Figure 4_ <br /><br />
9. In the second section of that screen where it says "Deployment Info" uncheck the boxes that says "Landscape Left" and "Landscape Right". We only want to support portrait orientantion in this calculator. See figure 5.
<img src="https://raw.githubusercontent.com/fnk0/iOS-Calculator-Tutorial/master/Calculator/images/fig5.png" alt="Figure 5" style="width: 600px;"/> <br />
_Figure 5_ <br /><br />

10. Now let's proceed to build the user interface for our calculator. On the **Navigator Area** select the file ```Main.storyboard```

<br /><br /><br /><br /><br /><br /><br /><br />

### Step 2: Building the User Interface
In this step we will be adding the buttons and the placeholder text for our calculator app. <br />
You should now have something similar to figure 6. <br />
<img src="https://raw.githubusercontent.com/fnk0/iOS-Calculator-Tutorial/master/Calculator/images/fig6.png" alt="Figure 6" style="width: 600px;"/> <br />
_Figure 6_ <br /><br />

I know that XCode might look intimidating at first glance. So let's take a second to understand what each section of the program does:

- Navigator Area
+ A tree view of the files in your project. The .swift files is where our code will live. The .storyboard file is where the user interface for our app will be located.
- Outline View
+ The ouline view will show an outline and a hierarchy of the user interface in the storyboard.
- Toolbar
+ The buttons on the right are used to hide or show different sections of Xcode. 
+ The buttons on the left are used to "Run" or stop the application. You can also select which device you want to run the app on. For the purposes of this tutorial we will only be using the iPhone 6.
+ The central area of the toolbar will display information about the current status of the project and progress bar for any ongoing operation by Xcode.
- Canvas Area
+ The canvas area in the .storyboard files represents the area on which we will build the user interface for our applications
+ For the .swift files the canvas will be replaced with a text editor where we will write the code for the app.
- Attribute Selector
+ The attributes selector allow us to navigate in between diferent properties of our user interface application
<br /><br /><br /><br /><br /><br />
- Attributes Area
+ Displays the attributes for the current selected attribute selector.
+ Atrributes can vary depending on the object selected in the canvas.
- Object Library
+ The object library is where we will select the different components to build the user interface.

1. In the attribute selector click on the leftmost icon. The icon looks like a file<br /><br />
2. In the attributes area unchek the box that says _"Use size classes"_.<br /><br />
3. When promped with a message to keep the data for iPhone or iPads. Select iPhone and click on "Disable Size Classes". See figure 7.
<br />
<img src="https://raw.githubusercontent.com/fnk0/iOS-Calculator-Tutorial/master/Calculator/images/fig7.png" alt="Figure 7" style="width: 600px;"/> <br />
_Figure 7_ <br /><br /><br />
4. On the attributes selector click on the 4th icon from left to right
5. On the outline view click on **"ViewController"**
6. In the Attributes area where it says Size, change it to iPhone 4.7 inch
7. In the object selector find the ```Label``` component and drag into the canvas.<br /><br />
8. Resize the label to occupy the full width of the screen, but leaving a small margin on the sides. Xcode should display some guiding margins when you get close to the edge of the screen.<br /><br />
9. On the attributes selector click on 4th icon from left to right. <br /><br /><br />
10. On the attributes area aligh the text of the label to be right. You should now have something similar to Figure 8. <br /><br /><br /><br /><br />
11. Increase the font size of the label to 22. Feel free to explore the Attributes panel and change anything else, such as font, color, etc. 
<br />
<img src="https://raw.githubusercontent.com/fnk0/iOS-Calculator-Tutorial/master/Calculator/images/fig8.png" alt="Figure 8" style="width: 600px;"/> <br />
_Figure 8_ <br /><br />
12. From the object library drag 16 buttons to the canvas.<br /><br />
13. Arrange the buttons into 4 rows of 4 buttons each.<br /><br />
<br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />
14. Double click on each button to change it's text and change the text inside a button to mirror a calculator layout. You should now have something similar to Figure 9. 
<br />
<img src="https://raw.githubusercontent.com/fnk0/iOS-Calculator-Tutorial/master/Calculator/images/fig9.png" alt="Figure 9" style="width: 600px;"/> <br />
_Figure 9_ <br /><br />
15. Double click the label and change the text to 0<br /><br />
16. Using your mouse or trackpad select all numeric buttons of the calculator. You can also hold shift and click each button individually to keep the selection.<br /><br />
17. On the attributes Area change the background color of the buttons to any color you want.<br /><br />
18. Change the text color of the button to anything you want as well.<br />
_**hint**: You can change the text color of a button by changing the **Tint** property, right below the **Background** property. _<br /><br />
19. Select the Group with the different operators and the **"."** symbol.<br /><br />
20. Do the same that you did for the numbers but with a different color.<br /><br />
21. Change the background and text color of the **"="** button. <br /><br />
<br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />
22. You should now have something similar to Figure 10. 
<br />
<img src="https://raw.githubusercontent.com/fnk0/iOS-Calculator-Tutorial/master/Calculator/images/fig10.png" alt="Figure 10" style="width: 600px;"/> <br />
_Figure 10_ <br /><br />
You may have noticed that our calculator is not using all the space available in the screen and our buttons are very small.  <br /><br />
23. Resize the buttons by dragging from it's edges to fill up more space on the screen. This step is optional and just for asthetics purposes.<br /><br />
24. Change the background color of the Window. To change the background colorof the window in the Outline View click on the Item that says **"View"**.<br /><br />
25. Change the font size of all the buttons and label<br /><br />
26. Click on where says **iPhone 6s plus** and change it to **iPhone 6s**<br /><br />
<br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />
27. Click the **Play** button in the toolbar to run the app. See figure 11.<br /><br />
<img src="https://raw.githubusercontent.com/fnk0/iOS-Calculator-Tutorial/master/Calculator/images/fig10.png" alt="Figure 11" style="width: 600px;"/> <br />
_Figure 11_ <br /><br />
28. You should now see a simulator window with the calculator app running! See figure 12. Click on the buttons of the calculator. <br />
<img src="https://raw.githubusercontent.com/fnk0/iOS-Calculator-Tutorial/master/Calculator/images/fig12.png" alt="Figure 12" style="width: 600px;"/> <br />
_Figure 12_ <br /><br />

<br />
As you can see when we click on the buttons of the calculator nothing happens. Don't worry in the next section we will make everything work!
<br /><br /><br /><br /><br /><br /><br /><br /><br /><br />
### Step 3: Making it work!

1. In the navigator area click on the **ViewController.swift**. The canvas area is replaced with the Text editor area. You should see something similar to figure 13. (The colors of the editor will probably be different).
<img src="https://raw.githubusercontent.com/fnk0/iOS-Calculator-Tutorial/master/Calculator/images/fig13.png" alt="Figure 13" style="width: 600px;"/> <br />
_Figure 13_ <br /><br />
2. In the navigator area select the **Main.storyboard** file again.<br /><br />
3. On the right side of the **Toolbar** click on the icon that are 2 circles. You should now see the Canvas editor on the left and the text editor on the right. <br /><br />
<img src="https://raw.githubusercontent.com/fnk0/iOS-Calculator-Tutorial/master/Calculator/images/fig14.png" alt="Figure 14" style="width: 600px;"/> <br />
_Figure 14_ <br /><br />
<br /><br />
4. Select one of the buttons in the canvas area.
5. Hold control and drag a line from the canvas area to the text editor area right below the code that says:

```swift
override func didReceiveMemoryWarning() {
super.didReceiveMemoryWarning()
// Dispose of any resources that can be recreated.
}
// Here is where we will drag
```
See figure 15.
<img src="https://raw.githubusercontent.com/fnk0/iOS-Calculator-Tutorial/master/Calculator/images/fig15.png" alt="Figure 15" style="width: 600px;"/> <br />
_Figure 15_ <br /><br />

6. After you release the mouse you should get a pop-up window with different options. Make it look like figure 16. <br />
<img src="https://raw.githubusercontent.com/fnk0/iOS-Calculator-Tutorial/master/Calculator/images/fig16.png" alt="Figure 16" style="width: 600px;"/> <br />
_Figure 16_ <br /><br /><br /><br /><br /><br />

7. You should now see a new function in your code that says:
```swift
@IBAction func handleButtonPress(sender: UIButton) {
}
```
To the right of that function there is tiny filled circle. Drag from the circle each one of the buttons with the exception of the first one. See figure 17. <br />
<img src="https://raw.githubusercontent.com/fnk0/iOS-Calculator-Tutorial/master/Calculator/images/fig17.png" alt="Figure 17" style="width: 600px;"/> <br />
_Figure 17_ <br /><br />

8. Now drag the **Label** to the space in between ```ViewController``` and ```ViewDidLoad```. See figure 18.
<img src="https://raw.githubusercontent.com/fnk0/iOS-Calculator-Tutorial/master/Calculator/images/fig18.png" alt="Figure 18" style="width: 600px;"/> <br />
_Figure 18_ <br /><br />

9. Make the items in the pop-up window that appeard look like Figure 19.
<img src="https://raw.githubusercontent.com/fnk0/iOS-Calculator-Tutorial/master/Calculator/images/fig19.png" alt="Figure 19" style="width: 600px;"/> <br />
_Figure 19_ <br /><br />

10. Xcode should have generate the following code for you:
```swift
@IBOutlet weak var resultLabel: UILabel!
```
Right below that code add the following code to declare the variables we will use.

```swift
var firstNumberText = ""
var secondNumberText = ""
var op = ""
var isFirstNumber = true
var hasOp = false
var canClear = true
```
<br />
11. Now below the method says ```handleButtonpress(sender: UIButton) ``` add the following code:
```swift
func calculate() -> Double {
let firstNumber = Double(firstNumberText)!
let secondNumber = Double(secondNumberText)!
firstNumberText = ""
secondNumberText = ""
switch op {
case "+":
return firstNumber + secondNumber
case "-":
return firstNumber - secondNumber
case "*":
return firstNumber * secondNumber
case "/":
return firstNumber / secondNumber
default:
return 0
}
```

This function is the one we will use to calculate the result of the operations.
<br /><br />
12. Now lets add the code to deal what happens when a button is pressed. Inside the ```handleButtonpress(sender: UIButton) ``` add the following code:
```swift
@IBAction func handleButtonPress(sender: UIButton) {
if canClear {
resultLabel.text = ""
canClear = false
}
let currentText = resultLabel.text!
let textLabel = sender.titleLabel?.text
if let text = textLabel {
switch text {
case "+", "*", "/", "-":
if hasOp {
return
}
op = text
isFirstNumber = false
hasOp = true
resultLabel.text = "\(currentText) \(op) "
break
case "=":
isFirstNumber = true
hasOp = false
canClear = true
let result = calculate()
resultLabel.text = "\(result)"
break
default:
if isFirstNumber {
firstNumberText = "\(firstNumberText)\(text)"
} else {
secondNumberText = "\(secondNumberText)\(text)"
}
resultLabel.text = "\(currentText)\(text)"
break;
}
}
}
```
<br />
Your code should look something like this:
```swift
import UIKit

class ViewController: UIViewController {

@IBOutlet weak var resultLabel: UILabel!

var firstNumberText = ""
var secondNumberText = ""
var op = ""
var isFirstNumber = true
var hasOp = false
var canClear = true

override func viewDidLoad() {
super.viewDidLoad()
// Do any additional setup after loading the view, typically from a nib.
}

override func didReceiveMemoryWarning() {
super.didReceiveMemoryWarning()
// Dispose of any resources that can be recreated.
}


@IBAction func handleButtonPress(sender: UIButton) {
if canClear {
resultLabel.text = ""
canClear = false
}
let currentText = resultLabel.text!
let textLabel = sender.titleLabel?.text
if let text = textLabel {
switch text {
case "+", "*", "/", "-":
if hasOp {
return
}
op = text
isFirstNumber = false
hasOp = true
resultLabel.text = "\(currentText) \(op) "
break
case "=":
isFirstNumber = true
hasOp = false
canClear = true
let result = calculate()
resultLabel.text = "\(result)"
break
default:
if isFirstNumber {
firstNumberText = "\(firstNumberText)\(text)"
} else {
secondNumberText = "\(secondNumberText)\(text)"
}
resultLabel.text = "\(currentText)\(text)"
break;
}
}
}


func calculate() -> Double {
let firstNumber = Double(firstNumberText)!
let secondNumber = Double(secondNumberText)!
firstNumberText = ""
secondNumberText = ""
switch op {
case "+":
return firstNumber + secondNumber
case "-":
return firstNumber - secondNumber
case "*":
return firstNumber * secondNumber
case "/":
return firstNumber / secondNumber
default:
return 0
}
}

}

```

<br />
13. In the toolbar press the **Play** button to run the app. Play around with the calculator and make sure everything is working!

### Conclusion:

Congratulations! You just built your first app!! Where to go from here? Keep exploring and adding functionality to the calculator! You probably have noticed that the calculator does not handle negative numbers and it's also missing a **clear** and a **delete** button. There is also a really big problem in this calculator! If somebody tries to divide by zero the app will crash. I will live fixing that problem as an exercise for you. So go ahead and keep exploring! You can download the full code for the project from my [Github page](https://github.com/fnk0/iOS-Calculator-Tutorial).


An excelent place to find more iOS tutorials is [Ray Wanderlich](http://www.raywenderlich.com/)


### Troubleshooting:

- The buttons and label have a different size on the screen when I run the emulator?
+ Option 1: Make sure that in the Attributes area you have specified your storyboard to be iPhone 4.7"
+ Option 2: You are using a Simulator for the iPhone 6+ or for the iPhone 5. In the toolbar next to the **Play** button make sure to select iPhone 6 or iPhone 6s.
- When I press a specific button nothing happens.
+ Make sure to connect the function ```func handleButtonPress(sender: UIButton)``` to the button in the .storyboard file by dragging from the circle in the left side of the function.










