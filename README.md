# Build a Makecode Platform and Customize Extensions
Aim to instruct people build a makecode platform and custormize their own blocks, the content on this page is based on the exsited document including microsoft official documnet on [Makecode](https://makecode.com/docs) and tutorials of serveral platforms. PS: There might be some differences from the original ones since some code did not work for me through the process.

## Makecode General Information
Microsoft Makecode is based on the open source project [Microsoft Programming Experience Toolkit(PXT)](https://github.com/Microsoft/pxt). Microsoft Makecode is the name in the user-facing editors (hereinafter called the 'platform' or 'target'), ```PXT``` is used in all the GitHub sources.

![General Information of Makecode](https://github.com/YilinXia/Makecode/blob/master/Picture/General%20Information.png)

**1. Platform (User-Facing)** Composed of homepage, simulator, blocks console, and javascript console.User can use blocks or javascript to design their own code and workflow and the result will show within simulator area simultaneously.</br></br>
Many platforms programmed by makecode have existed and each of them has its own tutorials. (Including the block features, applications in reality and examples).

| Platform Name          |Description       | Homepage                                          | Tutorial              |Github
| -------------------    |:-------------    |:-------------                                     | :-----                |:-----
| Ada-fruit              | You can run your code using the Adafruit Circuit Playground Express simulator, all within the confines of a web browser. The simulator has support for the LED screen, buttons, as well as compass, accelerometer, and digital I/O pins.                 | [Homepage](https://makecode.adafruit.com/)        | [Tutorial](https://makecode.adafruit.com/blocks)    |[Github](https://github.com/Microsoft/pxt-adafruit)
| Microbit               | The micro:bit provides an easy and fun introduction to programming and making – switch on, program it to do something fun – wear it, customize it. Just like Arduino, the micro:bit can be connected to and interact with sensors, displays, and other devices.| [Homepage](https://makecode.microbit.org/)        | [Tutorial](https://makecode.microbit.org/blocks)    |[Github](https://github.com/Microsoft/pxt-microbit)
| Minecraft              |MakeCode for Minecraft is a code editor to build fun mods and programs for Minecraft. | [Homepage](https://minecraft.makecode.com/)       | [Tutorial](https://minecraft.makecode.com/blocks)   |NULL
| Lego Education         |You can run your code using the LEGO® MINDSTORMS® Education EV3 simulator, all inside the same browser window. The simulator has support for the EV3 Brick screen, buttons, sensors, and motors. | [Homepage](https://makecode.mindstorms.com/)      | [Tutorial](https://makecode.mindstorms.com/blocks)  |NULL
| Chibi Chip             |The Love to Code Creative Coding Kit is a fun, new way to learn circuits and coding. | [Homepage](https://makecode.chibitronics.com/)    | [Tutorial](https://makecode.chibitronics.com/about) | [Github](https://github.com/Microsoft/pxt-chibitronics)
| Seed Studio            |When you have your code ready, you connect your Grove Zero Main Board to a computer via a USB cable then press the reset button twice so it appears as a mounted drive（Grove Zero）.| [Homepage](https://makecode.seeedstudio.com/)     | [Tutorial](https://makecode.seeedstudio.com/blocks) | [Github](https://github.com/Seeed-Studio/pxt-grove-zero-for-microbit)
| Beat the traffic       |By setting values, simulator could calculate the efficiency of the road| [Homepage](https://liolop.github.io/Coraffic/)     | NULL| NULL
| Cornell Build your face|An editor for personalizing mask on your face captured by camera  | [Homepage](https://jcspec.github.io/BuildUFace/#)      | NULL|NULL
| Arcadia    |An editor for Marker-based Augmented Reality|[Homepage](https://laboratoryforplayfulcomputation.github.io/arcadia/)     |[Tutorial](https://laboratoryforplayfulcomputation.github.io/arcadia/docs/examples/piano.html)| NULL
| Samuel Postcard Making    |A Blocks / JavaScript code editor for the holidays powered by Microsoft MakeCode| [Homepage](https://samelhusseini.github.io/pxt-holidays/controller.html) | NULL| [Github](https://github.com/samelhusseini/pxt-holidays)



**2. PXT (Developers-Oriented)** . PXT developers are group of people who can reorganize homescreen, build simulators and javascript console, customize blocks including naming attributes, defining new functions ect.

Some useful information for your reference
* Stack Overflow ```makecode``` tag
* Discord https://discordapp.com/invite/ypvQNWy (Highly Recommend)
* Email makecode@microsoft.com

## Existed Blocks
Certainly, blocks in the platform represent certain lines of code and by combining them, users can launch functions such as forloop, boolean statement and so on. After reviewing the existed platforms and the blocks they contain, blocks can be divided into groups and detailed information is shown below.

<img src="https://github.com/YilinXia/Makecode/blob/master/Picture/Blocks.png" width="60%" height="40%">

### Basic Blocks
| Types                  |Name              | Function                    | Looks like            
| -------------------    |:-------------    |:----------                  | :-----              
| Loops                  |on start          |An event that runs when the program starts | <img src="https://github.com/YilinXia/Makecode/blob/master/Picture/Onstart.png" width="40%" height="30%">      
|                        |for               |Repeat code for a given number of times using an index | <img src="https://github.com/YilinXia/Makecode/blob/master/Picture/for.png" width="40%" height="30%">               
|                        |while             |Repeat code while a condition is true  | <img src="https://github.com/YilinXia/Makecode/blob/master/Picture/While.png" width="30%" height="30%">  
|                        |repeat            |Repeat code for a given number of times  | <img src="https://github.com/YilinXia/Makecode/blob/master/Picture/Repeat.png" width="30%" height="30%"> 
|                        |for of            |Repeat code for each item in a list  | <img src="https://github.com/YilinXia/Makecode/blob/master/Picture/For of.png" width="40%" height="30%"> 
|                        |forever            |Repeat code for a given number of times  | <img src="https://github.com/YilinXia/Makecode/blob/master/Picture/Forever.png" width="30%" height="30%"> 
|                        |pause              |Pause for the specified time in milliseconds  | <img src="https://github.com/YilinXia/Makecode/blob/master/Picture/Pause.png" width="30%" height="30%"> 
|                        |runInBackground    |Run this code in parallel with the current code  | <img src="https://github.com/YilinXia/Makecode/blob/master/Picture/runinbackgroud.png" width="30%" height="30%"> 
| Logic                  |if               |Conditional statement | <img src="https://github.com/YilinXia/Makecode/blob/master/Picture/if.png" width="30%" height="30%"> 
|                        |boolean          |True or false values | <img src="https://github.com/YilinXia/Makecode/blob/master/Picture/Boolean.png" width="30%" height="30%">
|                        |comparison       |Compare two values, usually locate as the condition of if | <img src="https://github.com/YilinXia/Makecode/blob/master/Picture/Comparison.png" width="30%" height="30%">
| Variable               |assign             |Assign(set) a variable's value | <img src="https://github.com/YilinXia/Makecode/blob/master/Picture/Assign.png" width="30%" height="30%"> 
|                        |change             |change a variable's value | <img src="https://github.com/YilinXia/Makecode/blob/master/Picture/Change.png" width="30%" height="30%"> 

### Basic build-in objects
| Type                   | Functions                                      | Achieved operation             
| -------------------    |:----------                                     | :-----   
| Math                   |using math, math operators and math functions   |integer/float/ binary operation/ remainder/ Exponent / Square root/ Absolute value/ minimum and maxmum / random value / constrain
| Text                   |Functions to combine, split, and search text strings   |return the character at the specified index/ compare order of two strings/ return substring of the current string/ convert string to number/ convert string to integer
| Arrays                  |Add,remove, and replace items in lists         |return the index of the first occurence of a value in an array/ append a new element to an array/ remove element from an array and return it/ add element to an array and return the new length / insert the value at a particular index / remove the element at a certain index

## Build your own Target
![Specific Information about Creating Target](https://github.com/YilinXia/Makecode/blob/master/Picture/Create%20Target.png)

<br>Reference:[Target-Creation](https://makecode.com/target-creation) 

### Software & System Information
System: Mac V10.13.6<br>
Version: <br>
Node v10.13.0 <br>
NPM v6.7.0

### Step1: Copy one sample to local 
* Install node.js 8+ Go to https://nodejs.org/en/download/  download the appropriate version and then install<br>
* Install Node.JS and the PXT command line
```
sudo npm install -g pxt
sudo npm install -g install
```
* Get a copy of the sample target sources, here the sample used is https://github.com/microsoft/pxt-adafruit
   * clone
   ```
   git clone https://github.com/Microsoft/pxt-adafruit  pxt-adafruit
   ```
   * run npm install (under the pxt-adafruit folder)
   ```
   cd pxt-adafruitnpm install
   ```
   * run the serve (under the pxt-adafruit folder)
   ```
   npm run serve
   ```
### Step2: Update information & Customized Homescreen 
Since you copy the sample source "pxt-adafruit" to directory pxt-adafruit in step1, so you can find important files as following in pxt-adafruit file
* ```/libs```Packages that define the APIs and they shld be exposed in blocks
* ```/sim```Typescript source for the in-browser simulator, if any
* ```docs``` markdown documentation pages
* ```pxtarget.json```  Where a PXT target is described  [pxtarget.json](https://makecode.com/targets/pxtarget)
* ```targetconfig.json``` change the structure of home screen  [targetconfig.json](https://makecode.com/targets/home-screen)
* ```package.json``` all PXT target also must supply an this JSON file [package.json](https://docs.npmjs.com/files/package.json)
* ```graphical assets```  where storing pictures and icons of editor homepage and located under ```/docs/static```

#### Relationship between attributes of ```pxtarget.json``` &```package.json``` & ```targetconfig.json```
Based on the three files of PXT-adafruit & [pxt-holidays/pxtarget.json](https://github.com/samelhusseini/pxt-holidays/blob/master/pxtarget.json) , then figure out the relationship among these attributes and associate them with corresponding part of editor homepage.

#### Update information of ```pxtarget.json```
:question: change the ```id/ name/ title```reagarding the sample of ```pxtarget.json```<br>

#### Update information of ```package.json```
:question: what is NPM / change your target id and repositories locations, etc. <br>

```Comments by makecode team on Discord: ignore this part```

#### Customized structure of homescreen```targetconfig.json```
related files are ```pxtarget.json``` and ```targetconfig.json```

#### Beautify your editor```graphical assets```
* avatar.svg image used in talking heads
* loader.svg image used in loading overlay


## Block Design And Build (Extensions)



<br>
<br>

### Update Mar.4th, 2019
