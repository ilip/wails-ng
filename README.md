<p align="center">
 <img src="./banner.png"/>
</p>

# Introduction
A template for [Wails v2.9.0](https://wails.io) with Angular 18.2.3. (TypeScript + Less + Tailwind + Preline)

Current Versions:
 - Angular 18.2.3
 - Wails v2.9.0 or newer
 - Tailwind 3.4.14
 - Preline 2.5.1

# Getting Started
## Prerequisites
 - Node 14+ with npm
 - Wails CLI v2.9.0 or newer | (https://wails.io/docs/gettingstarted/installation)
 - Angular CLI | Install with `npm i -g @angular/cli`

## Creating the Projekt
Create a new Application with the Wails CLI and this template:
```
wails init -n projektname -t https://github.com/ilip/wails-ng
```

## Running the Application in Developer Mode
The easiest way is to use the Wails CLI: `wails dev`

This should hot refresh when making changes the Frontend and rebuild when making changes in the Go.

## Building the Application for Production
When building for Production, there are some parts to notice:
 - Angular is going to use the `frontend/src/environments/environment.prod.ts` when building the frontend.
 - You should properly change the Icons for your Application in `build/` and `build/windows` (when building for Windows)
 - The Developer Console will not work.

Finally, you can build you Application with: `wails build`
