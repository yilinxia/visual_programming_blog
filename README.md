# Build a Makecode Platform and Customize Extensions
Aim to instruct people build a makecode platform and custormize their own blocks, the content on this page is based on the exsited document including microsoft official documnet on [Makecode](https://makecode.com/docs) and tutorials of serveral platforms. PS: There might be some differences from the original ones since some code did not work for me through the process.

## Makecode General Information
Microsoft Makecode is based on the open source project [Microsoft Programming Experience Toolkit(PXT)](https://github.com/Microsoft/pxt). Microsoft Makecode is the name in the user-facing editors (hereinafter called the 'platform'), ```PXT``` is used in all the GitHub sources.

![General Information of Makecode](https://github.com/YilinXia/Makecode/blob/master/General%20Information.png)

**1. Platform (User-Facing)** Composed of homepage, simulator, blocks console, and javascript console.User can use blocks or javascript to design their own code and workflow and the result will show within simulator area simultaneously</br></br>
Many platforms programmed by makecode have existed and each of them has its own tutorials. (Including the block features, applications in reality and examples)

| Platform Name          | Homepage                                          | Tutorial                                |Github
| -------------------    |:-------------                                     | :-----                                  |:-----
| Ada-fruit              | [Homepage](https://makecode.adafruit.com/)        | [Tutorial](https://makecode.adafruit.com/blocks)    |
| Microbit               | [Homepage](https://makecode.microbit.org/)        | [Tutorial](https://makecode.microbit.org/blocks)    |
| Minecraft              | [Homepage](https://minecraft.makecode.com/)       | [Tutorial](https://minecraft.makecode.com/blocks)   |
| Lego Education         | [Homepage](https://makecode.mindstorms.com/)      | [Tutorial](https://makecode.mindstorms.com/blocks)  |
| Chibi Chip             | [Homepage](https://makecode.chibitronics.com/)    | [Tutorial](https://makecode.chibitronics.com/about) |
| Seed Studio            | [Homepage](https://makecode.seeedstudio.com/)     | [Tutorial](https://makecode.seeedstudio.com/blocks) |
| Beat the traffic       | [Homepage](https://liolop.github.io/Coraffic/)     | NULL|
| Cornell Build your face| [Homepage](https://jcspec.github.io/BuildUFace/#)      | NULL|
| Arcadia    |[Homepage](https://laboratoryforplayfulcomputation.github.io/arcadia/)     |[Tutorial](https://laboratoryforplayfulcomputation.github.io/arcadia/docs/examples/piano.html)|
| Samuel Postcard Making    | [Homepage](https://samelhusseini.github.io/pxt-holidays/controller.html) | NULL|



**2. PXT (Developers-Oriented)** . PXT developers are group of people who can reorganize homescreen, build simulators and javascript console, customize blocks including naming attributes, defining new functions ect.

Some useful information for your reference
* Stack Overflow ```makecode``` tag
* Discord https://discordapp.com/invite/ypvQNWy (Highly Recommend)
* Email makecode@microsoft.com

## Existed Blocks
Certainly, blocks in the platform represent certain lines of code and by combining them, users can launch functions such as forloop, boolean statement and so on. After reviewing the existed platforms and the blocks they contain, blocks can be divided into groups and detailed information is shown as below.

## Build your own Platform (Target)
![Specific Information about Creating Target](https://github.com/YilinXia/Makecode/blob/master/Create%20Target.png)
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
### Step2: Update information 
Since you copy the sample source "pxt-adafruit" to directory pxt-adafruit in step1, so you can find important files as following in pxt-adafruit file
* ```/libs```Packages that define the APIs and they shld be exposed in blocks
* ```/sim```Typescript source for the in-browser simulator, if any
* ```docs``` markdown documentation pages
* ```pxtarget.json```  A PXT target is described by a  ```pxtarget.json```

#### Update information of ```pxtarget.json```
:question: change the ```id/ name/ title```reagarding the sample of ```pxtarget.json```

#### Update information of ```package.json```
:question: what is NPM / change your target id and repositories locations, etc.
```
Comments by makecode team on Discord: ignore this part
```

#### Update information of ```graphical assets```
Graphical assets are located under ```/docs/static```
* avatar.svg image used in talking heads
* loader.svg image used in loading overlay

### Step3: Customized Homescreen 
related files are ```pxtarget.json``` and ```targetconfig.json```


## Block Design And Build (Extensions)




### Update Feb.11th, 2019
