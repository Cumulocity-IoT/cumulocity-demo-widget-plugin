# Cumulocity Demo Widget Plugin [<img width="35" src="https://user-images.githubusercontent.com/67993842/97668428-f360cc80-1aa7-11eb-8801-da578bda4334.png"/>](https://github.com/SoftwareAG/cumulocity-demo-widget-plugin/releases/download/1.0.0-beta/cumulocity-demo-widget-plugin-1.0.1-beta.zip)

This Demo Widget is the Cumulocity module federation plugin created using c8ycli. This plugin can be used in Application Builder or Cockpit. It fetches Inventory data based on the device id and displays the same in a widget.

### Please note that this plugin is in currently under BETA mode.

### Please choose Demo Widget release based on Cumulocity/Application builder version:

|APPLICATION BUILDER | CUMULOCITY | DEMO WIDGET PLUGIN  |
|--------------------|------------|---------------------|
| 1.4.x(coming soon)| >= 1015.x.x| 1.x.x               |


## Prerequisites:
   Cumulocity c8ycli >=1014.x.x
   
## Installation

  
### Runtime Deployment?

* This widget support runtime deployment. Download [Runtime Binary](https://github.com/SoftwareAG/cumulocity-demo-widget-plugin/releases/download/1.0.0-beta/cumulocity-demo-widget-plugin-1.0.1-beta.zip) and install via Administrations(Beta mode) --> Ecosystems --> Applications --> Packages 

### Local Development?

**Requirements:**
* Git
* NodeJS (release builds are currently built with `v14.18.0`)
* NPM (Included with NodeJS)

**Instructions**
1. Clone the repository: 
```
git clone https://github.com/SoftwareAG/cumulocity-demo-widget-plugin.git
```
2. Change directory: 
```
cd cumulocity-demo-widget-plugin
```
3. Install the dependencies: 
```
npm install
```
4. (Optional) Local development server: 
```
npm start -- --shell cockpit
```
5. Build the app: 
```
npm run build
```
6. Deploy the app: 
```
npm run deploy
```


------------------------------

These tools are provided as-is and without warranty or support. They do not constitute part of the Software AG product suite. Users are free to use, fork and modify them, subject to the license agreement. While Software AG welcomes contributions, we cannot guarantee to include every contribution in the master project.
_____________________
For more information you can Ask a Question in the [TECH Community Forums](https://tech.forums.softwareag.com/tag/Cumulocity-IoT).
