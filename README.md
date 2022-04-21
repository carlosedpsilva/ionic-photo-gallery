# My First Ionic App: Photo Gallery (Ionic Angular and Capacitor)

Simple Ionic project based on the documentation project.

Powered by [Ionic Angular](https://ionicframework.com/docs/angular/overview) (web app) and [Capacitor](https://capacitor.ionicframework.com) (native app runtime).

## How to Run this Project

1) Install Ionic if needed: `npm install -g @ionic/cli`.
2) Clone this repository.
3) In a terminal, change directory into the repo: `cd photo-gallery-capacitor-ng`.
4) Install all packages: `npm install`.
5) Run on the web: `ionic serve`.
6) Run on iOS or Android: See [here](https://ionicframework.com/docs/building/running).

## Creating the App

1) Create a new project: `ionic start photo-gallery tabs --type=angular --capacitor`.
2) Change directory into the new project: `cd photo-gallery`.
3) Install native functionality dependencies: `npm install @capacitor/camera @capacitor/storage @capacitor/filesystem`.
4) Install web-base functionality dependencies: `npm install @ionic/pwa-elements`.
5) Import `@ionic/pwa-elements` by editing `src/main.ts`.

    ```ts
    import { defineCustomElements } from '@ionic/pwa-elements/loader';

    // Call the element loader after the platform has been bootstrapped
    defineCustomElements(window);
    ```

6) Run the app: `ionic serve`.
