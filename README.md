# Build a Platform Based on Makecode
Aim to instruct people build a makecode platform and custormize their own blocks, the content on this page is based on the exsited document including microsoft official documnet on [Makecode](https://makecode.com/docs). PS: There might be some difference from the original ones since some code did not work for me through the process.

## Makecode General Information
Microsoft Makecode is based on the open source project [Microsoft Programming Experience Toolkit(PXT)](https://github.com/Microsoft/pxt). Microsoft is the name in the user-facing editors (hereinafter called the 'platform'), ```PXT``` is used in all the GitHub sources

![General Information of Makecode](https://github.com/YilinXia/Makecode/blob/master/General%20Information%20of%20Makecode.png)

**1. Platform** Focus on user-facing. User can use blocks or javascript to design their own code and workflow. </br></br>
Many platforms programmed by makecode already exist and each of them has its own tutorials. (Including the block features, applications in reality and examples)
* Circuits: **Editor Ada-fruit:** https://makecode.adafruit.com/  **Tutorial:** https://makecode.adafruit.com/blocks. 
* Microbit: **Editor micro-bit:** https://makecode.microbit.org/  **Tutorial:** https://makecode.microbit.org/blocks
* Minecraft:**Editor Minecraft:** https://minecraft.makecode.com/ **Tutorial:** https://minecraft.makecode.com/blocks
* Lego Education: https://makecode.mindstorms.com/blocks
* Chibi Chip: https://makecode.chibitronics.com/about
* Seed Studio: https://makecode.seeedstudio.com/blocks
* Beat the traffic: https://liolop.github.io/Coraffic/
* Cornell Build your face: https://jcspec.github.io/BuildUFace/
* Arcadia https://laboratoryforplayfulcomputation.github.io/arcadia/docs/about.html
* Samuel Postcard Making https://samelhusseini.github.io/pxt-holidays/controller.html


**2. PXT** For developers. PXT developers are group of people who can change the block totally including changing the block shape, block attribute, block color ect., not like users can only change certain part of the block.

Some useful information for your reference
* Stack Overflow ```makecode``` tag
* Discord https://discordapp.com/invite/ypvQNWy (Highly Recommend)
* Email makecode@microsoft.com

## Block
Certainly, blocks in the platform represent certain lines of code and by combining them, users can launch functions such as forloop, boolean statement and so on. After reviewing the existed platforms and the blocks they contain, blocks can be divided into groups and detailed information is shown as below.

## Build your own Platform
### Step1: Build local platform (Named "target" in the official document)
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
Since you copy the sample source "pxt-adafruit" to directory pxt-adafruit in step1, so you can find those important files in this file especially pxtarget.json

## Block Design And Build
