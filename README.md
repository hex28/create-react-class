# create-react-class

A quick script to create jsx files for your project in Node.js

## How to
You can quickly use the script by downloading the git. You can keep it within its folder or you can take out the individual files.
If you decide to keep the files in the folder, remember to change the root directory

```
const rootdir = __dirname; //change __dirname to your root directory.
```

after that call the script
```
node createNewReactClass.js
```
follow the prompt and it should create a new template JSX file where you sent it to.

## Edit the template file
You can edit the template of the JSX file by going into prototypeReactFile.txt.
By Default it looks like so
```
import React from 'react';
import ReactDOM from 'react-dom';

export default class ${classname} extends React.Component {
  constructor(props){
    super(props);
  }

  render() {
    return (

    );
  }
}

```
Don't edit '${classname}'. Other than that you're free to make the template look however you like.

## Add to package.json
You can add a script to your package.json to make it easier to run.
```
  "scripts": {
    ...,
    "create-new-class": "/create-react-class/createNewReactClass.js",
  },
```
then you can use npm or yarn to run the file
```
npm create-new-class
yarn create-new-class
```

## Final Words

I may not have picked the best names for the files  ¯\\\_(ツ)_/¯\. You're free to rename them however you like.

Hope you'll be able to use this in your React projects! Good luck!
