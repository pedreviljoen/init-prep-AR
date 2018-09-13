# .init Workshop

<div align="center">
  <img src="assets/init_logo.jpg" width="70%">
</div>

# Preparations

Welcome to the first workshop of .init. This will serve as a guide with setup of your machine along with providing some technical reading that will assit you on the day.

Today's mission is to learn something that will expand your understanding. Something that you do not necessarily work with each day.

We will build an AR app that suggests food recipes. The technology involved is the interesting part of the learning.

We will touch on the following technologies: 

* React Native      - JS framework for mobile application.
* React Viro        - Mobile framework for AR apps.
* Google Vision API - Google's cloud solution for image processing.

But first we will need to setup our machines, to make sure we can develop on the day.

# Setup

Open up your terminal for the next part. We recommend using VS Code, a simple code editor. But you can use any editor of your choice.

## Node & Watchman

Your machine will need the following basic tools. We recommend to install these through Homebrew. But you can use whatever install method you want, as long as the dependancies are installed in your PATH.

If you don't have Homebrew, please check it out here https://brew.sh/ & install.

Next steps are simple. First we will install `node` and `watchman`.

```shell
brew install node
```

and don't forget watchman

```shell
brew install watchman
```

## Package manager

Check if you have a package manager, we recommend `npm`. You could use `yarn` also.

Run the following to check:

```shell
npm -v
```

If your terminal returns a version number, you are all set. If not you can run the following command:

```shell
brew install -g npm
```

## Ngrok

If you don't have Ngrok, you can download and install it here:

https://ngrok.com/download

## React Native Command Line Interface

Next step is to install the React Native CLI, run the following command:

```shell
npm install -g react-native-cli
```

## ViroReact Command Line Interface

Next step is to install the ViroReact CLI, run the following command:

```shell
npm install -g react-viro-cli
```

& that is it with setup!

## Useful plugins

If you decided to use VS Code as your code editor, some useful plugins are:

* JS Hacker Pack
* Color Highlight
* Bracket Pair Colorizer
* Auto Close Tag
* Auto Rename Tag
* Guides
* VS Live Share: If you guys want to code with multiple machines

# ViroReact

# Google's Vision API

Google provides numerous cloud solutions. Similar to the services offered by Amazon with their Web Services (AWS). We will be making use of Google Cloud Vision API, which provides insight by utilising their pretrained API models. All of which is encapsulated into an easy-to-use REST API. To read more about Cloud Vision API, please see below:

https://cloud.google.com/vision/

The API is a REST API that uses HTTP POST to perform data analysis on images sent with the POST object. JSON is the standard format for both Request/Response bodies.

We have taken care of most of the heavy lifting for you in the project. However, if you want to play around with some of the response features. You can change your request body to include these features. You will see an example of the response in the documentation. Please read the docs here:

https://cloud.google.com/vision/docs/request

You will notice the image needs to be base64 encoded. We have done this for you in the project, but you can read up about base64 encoding here:

https://developer.mozilla.org/en-US/docs/Web/API/WindowBase64/Base64_encoding_and_decoding

For interested readers, you can also do text/label detection with Google Vision. An interesting use case is to extract data of an universal object, ie a credit card. A cool thought would be, how to manipulate the data in the response to extract the info of a credit card. You can read more about text/label detection here:

https://cloud.google.com/vision/docs/ocr

https://cloud.google.com/vision/docs/labels