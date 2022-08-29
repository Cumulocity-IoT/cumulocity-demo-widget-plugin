# Cumulocity Demo Widget Plugin [<img width="35" src="https://user-images.githubusercontent.com/67993842/97668428-f360cc80-1aa7-11eb-8801-da578bda4334.png"/>](https://github.com/SoftwareAG/cumulocity-demo-widget/releases/download/2.0.0/demo-runtime-widget-2.0.0.zip)

This Demo Widget is the Cumulocity module federation plugin created using c8ycli. This plugin can be used in Application Builder or Cockpit. It fetches Inventory data based on the device id and displays the same in a widget.

### Please choose Demo Widget release based on Cumulocity/Application builder version:

|APPLICATION BUILDER | CUMULOCITY | DEMO WIDGET PLUGIN  |
|--------------------|------------|---------------------|
| 1.4.x              | >= 1014.x.x| 1.x.x               |


## Prerequisites:
   Cumulocity c8ycli >=1014.x.x
   
## Installation

  
### Runtime Deployment?

* This widget support runtime deployment. Download [Runtime Binary](https://github.com/SoftwareAG/cumulocity-smart-map-widget/releases/download/2.0.0/smartmap-runtime-widget-2.0.0.zip) and install via Administrations(Beta mode) --> Ecosystems --> Applications --> Packages 

### Local Development?


   
## Create Cumculocity Widget Plugin
This is the Cumulocity module federation plugin. Plugins can be developed like any Cumulocity application, but can be used at runtime by other applications. Therefore, they export an Angular module which can then be imported by any other application. The exports are defined in `package.json`:

```
"exports": [
  {
     "name": "Example widget plugin",
     "module": "WidgetPluginModule",
     "path": "./widget/widget-plugin.module.ts",
     "description": "Adds custom widget"
  }
]
```

**How to start**
Run the command below to scaffold a `widget` plugin.

```
c8ycli new <yourPluginName> widget-plugin
```

As the app.module is a typical Cumuloctiy application, any new plugin can be tested via the CLI:

```
npm start -- --shell cockpit
```

In the Module Federation terminology, `widget` plugin is called `remote` and the `cokpit` is called `shell`. Modules provided by this `widget` will be loaded by the `cockpit` application at the runtime. This plugin provides a basic custom widget that can be accessed through the `Add widget` menu.

> Note that the `--shell` flag creates a proxy to the cockpit application and provides` WidgetPluginModule` as an `remote` via URL options.

Also deploying needs no special handling and can be simply done via `npm run deploy`. As soon as the application has exports it will be uploaded as a plugin.
