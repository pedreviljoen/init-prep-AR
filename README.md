# .init Workshop

<div align="center">
  <img src="assets/init_logo.jpg" width="70%">
</div>

# Preparations

Welcome to the first .init workshop. This document serves as a guide for the technical setup of your machine, along with providing necessary technical reading to help you understand the technologies that we will be using on the day.

The day's mission is to help you learn new technologies that will expand your knowledge, exposing you to things that you do not necessarily work with each day. In order to prevent a frustrating experience and rather ensure that the day is a whole lot of fun, it is important to be well prepared in terms of PC setup and a basic understanding of the technologies we will use. 

We will build an AR app that suggests food recipes after recognising your available food items using AI. The technologies involved is the interesting part of the learning.

We will use the following technologies on the day: 

* React Native      - JS framework for mobile application.
* Viro React        - Mobile framework for AR apps.
* Google Vision API - Google's cloud solution for image processing.

But first we will need to setup our machines, to make sure we can develop on the day.

# Setup

Open up your terminal for the next part. We recommend using VS Code, a simple code editor. But you can use any editor of your choice.

## Node & Watchman

Your machine will need the following basic tools. We recommend to install these through Homebrew. But you can use whatever install method you want, as long as the dependancies are installed in your PATH.

If you don't have Homebrew, please check it out [here](https://brew.sh/) & install.

Next steps are simple. First we will install `node` and `watchman`.

```shell
$ brew install node
```

and don't forget watchman

```shell
$ brew install watchman
```

## Package manager

Check if you have a package manager, we recommend [`npm`](https://www.npmjs.com/). You could also use [`yarn`](https://yarnpkg.com/en/).

Run the following to check:

```shell
$ npm -v
# Or
$ yarn -v
```

If your terminal returns a version number, you are all set. If not you can run the following command:

```shell
$ brew install node
```

This will install `node` and `npm`.

## Ngrok

If you don't have Ngrok, you can download and install it [here](https://ngrok.com/download).

## React Native Command Line Interface

Next step is to install the React Native CLI, run the following command:

```shell
$ npm install -g react-native-cli
```

## ViroReact Command Line Interface

Next step is to install the ViroReact CLI, run the following command:

```shell
$ npm install -g react-viro-cli
```

## Useful plugins

If you decided to use VS Code as your code editor, some useful plugins are:

* JS Hacker Pack
* Color Highlight
* Bracket Pair Colorizer
* Auto Close Tag
* Auto Rename Tag
* Guides
* VS Live Share: If you guys want to code with multiple machines

& that is it with setup!


# Pre- Reading

The following material will give you valuable context of the technologies that we will be using on the day. Work through this content to ensure that you have the necessary foundations to take the most out of the day.  

## ViroReact

ViroReact is a developer platform for rapidly building AR/VR applications using React Native. Whether you are looking to build a new AR/VR application, or add AR/VR features to your existing applications, the ViroReact platform enables you to create powerful mobile AR/VR applications using a single code base. We will be working with the AR component of Viro during the make day. 

This link will provide you with an overview of ViroReact and its application, [here](https://docs.viromedia.com/v2.6.1)

The next link points to important documentation on the fundamental elements involved in ReactViro AR. Read through it [here](https://docs.viromedia.com/v2.6.1/docs/augmented-reality-ar) and specifically pay attention to the theory of:

* Camera Tracking. 
* AR Components.

The most important AR components to get familiar with before the workshop are: 

[ViroARSceneNavigator](https://docs.viromedia.com/v2.6.1/docs/viroarscenenavigator)

[ViroARScene](https://docs.viromedia.com/v2.6.1/docs/viroarscene)

[ViroARPlane](https://docs.viromedia.com/v2.6.1/docs/viroarplane)

[ViroText](https://docs.viromedia.com/v2.6.1/docs/virotext2)

[Viro3DObject](https://docs.viromedia.com/v2.6.1/docs/viro3dobject)

## Google's Vision API

Google provides numerous cloud solutions. Similar to the services offered by Amazon with their Web Services (AWS). We will be making use of Google Cloud Vision API, which provides insight by utilising their pretrained API models. All of which is encapsulated into an easy-to-use REST API. To read more about Cloud Vision API, please see [here](https://cloud.google.com/vision/).

The API is a REST API that uses HTTP POST to perform data analysis on images sent with the POST object. JSON is the standard format for both Request/Response bodies.

We have taken care of most of the heavy lifting for you in the project. However, if you want to play around with some of the response features. You can change your request body to include these features. You will see an example of the response in the documentation. See the [docs](https://cloud.google.com/vision/docs/request).

You will notice the image needs to be base64 encoded. We have done this for you in the project, but you can read up about base64 encoding on [mdn](https://developer.mozilla.org/en-US/docs/Web/API/WindowBase64/Base64_encoding_and_decoding).

For interested readers, you can also do text/label detection with Google Vision. An interesting use case is to extract data of an universal object, ie a credit card. A cool thought would be, how to manipulate the data in the response to extract the info of a credit card. You can read more about [text](https://cloud.google.com/vision/docs/ocr)/[label](https://cloud.google.com/vision/docs/labels) detection.

# AR tutorial

This AR tutorial is a good excercise to work through before the workshop. The tutorial can be found [here](https://github.com/pedreviljoen/init-prep-AR-tutorial), checkout a branch and play around with a possible solution. If you get stuck, our implementation of a solution can be found [here](https://github.com/pedreviljoen/init-prep-AR-tutorial-solution).

Give it a bash, and we look forward to building cool tech on the day.

Au revoir