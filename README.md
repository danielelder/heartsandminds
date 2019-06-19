# Hearts and Minds

This repository contains the code you need to start building a user interface for the Hearts and Minds charity website.

## Pattern Lab

This project uses Pattern Lab to provide live examples of the Hearts and Minds frontend components. This helps developers to build thoughtful, pattern-driven user interfaces using atomic design principles.

Find out more about [Pattern Lab](https://patternlab.io/).

## Atomic Design

The Atomic Design methodology considers all the details that go into creating and maintaining robust user interfaces whilst providing a coherent way of explaining itself using chemistry.

### Naming conventions

| Property  | Description |
|-----------|-------------|
| Atoms     | The foundational building blocks that comprise all our user interfaces such as type, labels, colours and spacing. |
| Molecules | Molecules are our building blocks or ‘atoms’ that we are piecing together to form a functional element. | 
| Organisms | Organisms are slightly more complex and form bigger chunks of our product. We can think of these organisms in our user interface as groups of molecules. |
| Utilities | Utilities allow the default style or behaviour of atoms, molecules or organisms to be modified using and defined set of rules. |

Read more about [Atomic Design by Brad Frost](http://atomicdesign.bradfrost.com/).

## CSS Architecture

### Class Names

The CSS within this project follows the ABEM (Atomic Design, Block, Element, Modifier) naming convention. BEM is a class naming convention, allowing developers to write CSS in a modular and maintainable fashion.

Example BEM class names:

```
.block {}
.block__element {}
.block--modifier {}
.block__element--modifier {}
```

Learn more about [BEM](http://getbem.com/).


### Atomic Design class prefixes:

| Property  | Class prefix |
|-----------|--------------|
| Atoms     | a-           |
| Molecules | m-           | 
| Organisms | o-           |
| Utilities | u-           |

Example classes using ABEM (Atomic Design and BEM):

```
.o-block {}
.o-block--modifier {}

.m-block__element {}
.m-block__element--modifier {}

.a-block__element {}
.a-block__element--modifier {}

.u-align-center {}
```

### Structure

The folder structure is based on BEM architecture. Styles are split into four folders comprising of Abstract, Base, Modules, and Utilities.

| Folder    | Purpose                                                   |
|-----------|-----------------------------------------------------------|
| Abstract  | mixins, variables (font, colors definitions, etc.)        |
| Base      | Resets and general selector styles (body, h1, p, a, etc.) |
| Modules   | Atoms, molecules and organisms                            |
| Utilities | Helpers and overrides (shame file)                        |

## Browser support

Hearts and Minds User Interface currently supports the following browsers:

| Operating system | Browser                                |
|----------------- |----------------------------------------|
| Windows          | Edge (latest 2 versions)               |
| Windows          | Google Chrome (latest 2 versions)      |
| Windows          | Mozilla Firefox (latest 2 versions)    |
| macOS            | Safari 12+                             |
| macOS            | Google Chrome (latest 2 versions)      |
| macOS            | Mozilla Firefox (latest 2 versions)    |
| iOS              | Safari for iOS 12+                     |
| Android          | Google Chrome (latest 2 versions)      |

## Developing this project

```bash
git clone https://github.com/danielelder/heartsandminds.git
cd heartsandminds
npm install
npm run pl:serve
```

### Build and Test

| Command              | Description |
|----------------------| ----------- |
| `npm run pl:serve`   | Builds the Pattern Lab site and watches for changes |
| `npm run pl:help`    | Displays the Pattern Lab help |
| `npm run pl:version` | Displays the installed version of Pattern Lab |
