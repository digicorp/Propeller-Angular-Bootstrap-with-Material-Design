<br>
<p align="left">
  <a href="https://propeller.in/frameworks/angular">
    <img height="40" src="http://angular.propeller.in/propeller-angular-logo.png" />
  </a>
  <p align="left">
    Propeller Angular is a Material Design Front-end UI framework based on Angular 9, Bootstrap 4 and Sass. It is responsive and makes building web applications and websites faster with less coding.
  </p>
</p>

## Table of contents

- [Key Features](#key-features)
- [Download](#download)
- [Prerequisites](#prerequisites)
- [Package Installation using Command](#package-installation-using-command-line)
- [Get Started with Propeller Angular Themes](#get-started-with-propeller-angular-themes)
- [Setup](#setup)
- [Usage](#usage)
- [Bugs and feature requests](#bugs-and-feature-requests)
- [Community](#community)
- [License](#license)
- [Author](#author)

## Key Features

- Built using Native Angular 9
- Based on Bootstrap 4 and Material Design
- Supports Angular CLI
- Built using TypeScript
- Themed using Sass
- Detailed User Manual


## Download

Purchase the Angular Version of the Propeller library and get hands on the Angular components based on Bootstrap 4 and Material Design.

<a href="https://propeller.in/frameworks/angular/#pricing"><strong>View Packages</strong></a>

## Prerequisites

Before you start using Propeller Angular, make sure you have the packages @angular/cli and typescript npm installed globally in your system.These packages are necessary to develop an Angular application.

To install @angular/cli execute below command in your command line:

```
npm install -g @angular/cli
```

To install typescript execute below command in your command line:

```
npm install -g typescript
```

Checkout the [Angular CLI](https://cli.angular.io/) website to get more information on how to get started with a new Angular app.


## Package Installation using Command Line:

Follow the below steps to install the Propeller Angular package using Command Line. Also, download the zip file from the receipt within 48 hours of purchase as it contains the themes - Propeller Angular Admin Theme and the Starter Template.

**Step 1:** Create new angular project using Angular CLI command:

```
ng new your-angular-project --style=scss
```

**Step 2:** cd your-angular-project

**Step 3:** To install propeller-cli execute below command in your command line:

```
npm install -g propeller-cli
```

**Step 4:** Run the following CLI command in the command line to install the propeller angular packages

```
pmd install propeller-angular-bootstrap
```

**Step 5:** Enter the email address you used to make the purchase of the Propeller Angular in the Propeller website

**Step 6:** Enter the Product Key from the email you would have received after making the purchase

**Step 7:** Once you submit the product key it will automatically perform the pmd install command and install the Propeller Angular package and Bootstrap in your project. Once all the directory is setup, it's time to run the app on localhost. To do so, run:

```
ng serve --o
```

**Step 8:** On executing the above command, you will be able to see the default app screen on the port 4200.


## Get Started with Propeller Angular Themes
**Step 1:** Download the zip file from the email received on making the purchase. The zip file contains the themes - Propeller Angular Admin Theme and the Starter Template.

**Step 2:** Unzip the downloaded package and open your unpacked directory.

**Step 3:** Depending on your node module manager install all the dependencies by executing the following command in the command line:

```
npm install
```

**Step 4:** To install propeller-cli execute below command in your command line:

```
npm install -g propeller-cli
```

**Step 5:** Run the following CLI command in the command line to install the propeller angular packages

```
pmd install propeller-angular-bootstrap
```

**Step 6:** Enter the email address you used to make the purchase of the Propeller Angular in the Propeller website

**Step 7:** Enter the Product Key from the email you would have received after making the purchase

**Step 8:** Once you submit the product key it will automatically perform the pmd install command and install the Propeller Angular package and Bootstrap in the theme. Once all the directory is setup and all the dependencies are installed, it's time to run the theme on localhost. To do so, run:

```
ng serve --o
```

**Step 9:** On executing the above command, you will be able to see the default app screen on the port 4200.

> **_NOTE:_** For customizing the theme, kindly check the theme user-manual in the documentation folder.

## Setup

Follow the below steps to setup Propeller Angular in your project.

### Include Material Icons Library 

Propeller Angular uses Material Icons in all its components. So it is a must to include the Material Icons library in your project for the components to work properly. To include the library, add the following code in your index.html

```
<link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">
```

### Include Bootstrap 4 Library

To make Propeller Angular components work, it is necessary to include Bootstrap in the project. You have two options:

1. add styles to angular.json:

```
"styles": [
    "../node_modules/bootstrap/dist/css/bootstrap.min.css",
    "styles.scss"
],
```

2. add styles to index.html:

```
<link href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css" rel="stylesheet">
```

### Include Propeller SCSS

Once the Bootstrap CSS is included, the next step is to include Propeller SCSS. To use the components with the Google’s Material Design styling in your application, you just have to import the following file in your styles.scss if you are using Angular CLI

```
@import "../node_modules/pmd-angular-bootstrap/assets/scss/propeller.scss";
```
Now, if you want to modify the styling of the components as per your branding or add layout specific styling in your application, you will have to follow the below steps:

1. Setup the SCSS file structure similar to the following in your project:

```
your-project/
└── src
    ├── styles
    |   └── variable.scss
    |
    └── styles.scss
```

Note: Here at Propeller, we follow the following folder and file structure to increase reusability in the projects.


```
your-project/
└── src
    ├── styles
    │   ├── base/
    |   ├── components/
    |   ├── layout/
    |   ├── templates/
    |   ├── vendors/
    |   └── variable.scss
    |
    └── styles.scss
```

The base folder contains of SCSS files like _reboot.scss which are used to style the HTML tags. The components folder contains SCSS files of the components you want to update. The vendors folder contains the third party CSS/SCSS files. The layout folder contains SCSS files the comman layout SCSS files and the templates folder contains the SCSS files specific to the particular templates of the application.

2. Once the file structure is in place, you will have to import the Propeller’s Sass source files in the styles.scss in the following form.

```
// Propeller variable and functions
@import "../node_modules/pmd-angular-bootstrap/assets/scss/functions";
@import "../node_modules/pmd-angular-bootstrap/assets/scss/mixins";
@import "styles/variable";

// Propeller styles
@import "../node_modules/pmd-angular-bootstrap/assets/scss/propeller.scss";

// Project styles
// Include the project specific below

```

Note: Here at Propeller, we follow the below structure for SCSS in all our themes and projects to increase re-usability in the projects. For example the _components.scss contains the list of SCSS files that are imported from the components folder. These .scss consists of the SCSS required to update or add new styling to the Propeller components as per your project.

```
// Project styles
@import "styles/base/reboot";
@import "styles/components/components";
@import "styles/templates/templates";
```

[Click here](http://angular.propeller.in/sass-integration) to understand how to use the Sass variables, mixins and functions provided by Propeller Angular.

### Import the component modules
Once the Propeller SCSS is setup, you can start using the Propeller components in your project. To use a Propeller Component, you will have to import the NgModule of that component:

```
import { PmdButtonModule } from 'pmd-angular-bootstrap/button';
import { PmdFormGroupModule } from 'pmd-angular-bootstrap/input';
@NgModule({
...
imports: [PmdButtonModule.forRoot(), PmdFormGroupModule.forRoot()],
...
})
export class ProjectAppModule { }
```

## Usage

Visit [Propeller Angular User Guide](http://angular.propeller.in/) to get the detailed guidelines for using any component.


## Bugs and feature requests

Found any bug or issue or have any feedback, suggestions or questions? Post them on our [GITTER CHAT ROOM](https://gitter.im/Propeller-Material-Design-Bootstrap-Framework/Propeller-Angular-Support).


## Community

Get updates on Propeller Angular's development. Chat with the Product team and community members using Propeller.

- Follow [@propellerkit on Twitter](https://twitter.com/PropellerKit).
- Chat with fellow members on [GITTER](https://gitter.im/Propeller-Material-Design-Bootstrap-Framework/Propeller-Angular-Support).


## License

Propeller Angular v1.0 (http://propeller.in/frameworks/angular) 
© 2016-2019 [Digicorp Information Systems Pvt. Ltd.](https://www.digi-corp.com/)
Licensed under [Propeller Angular Developer License](https://propeller.in/license/#license-content-1)


## Author

Developed and maintained at [Digicorp](https://www.digi-corp.com/).
