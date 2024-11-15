# Deprecation notice

This plugin is not further developed and it might break with upcoming Cumulocity releases. Use it at your own risk.
The repository is archived but feel free to fork & adapt it to your needs in a new repo.

# Cumulocity Demo Widget Plugin [<img width="35" src="https://user-images.githubusercontent.com/67993842/97668428-f360cc80-1aa7-11eb-8801-da578bda4334.png"/>](https://github.com/Cumulocity-IoT/cumulocity-demo-widget-plugin/releases/download/1.0.6/c8y-pkg-demo-runtime-widget-1.0.6.zip)

This Demo Widget is the Cumulocity module federation plugin created using c8ycli. This plugin can be used in Application Builder or Cockpit. It fetches Inventory data based on the device id and displays the same in a widget.

### Please choose Demo Widget release based on Cumulocity/Application builder version:

|APPLICATION BUILDER | CUMULOCITY | DEMO WIDGET PLUGIN  |
|--------------------|------------|---------------------|
| 2.0.x              | >= 1018.x.x| 1.x.x               |


## Prerequisites:
   Cumulocity c8ycli >=1018.x.x
   
## Installation

  
### Runtime Deployment?

* This widget support runtime deployment. Download [Runtime Binary](https://github.com/Cumulocity-IoT/cumulocity-demo-widget-plugin/releases/download/1.0.6/c8y-pkg-demo-runtime-widget-1.0.6.zip) and install via Administrations(Beta mode) --> Ecosystems --> Applications --> Packages 

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

This tool is provided as-is and without warranty or support. They do not constitute part of the Cumulocity product suite. Users are free to use, fork and modify them, subject to the license agreement. While Cumulocity GmbH welcomes contributions, we cannot guarantee to include every contribution in the master project.

_____________________

