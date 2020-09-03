---
title: 'Learning React with Udacity - React Native'
date: '2017-12-10T00:00:00.0000'
layout: post
draft: false
path: '/posts/react-learning-notes-react-native'
category: 'Blog'
tags:
  - 'React'
  - 'React Native'
  - 'App'
  - 'Udacity'
  - 'notes'
description: 'Course notes on my final module from the Udacity ReactJS Redux and React Native Nanodegree.'
featuredImage: './react-logo.png'
---

##What is React Native?
React Native is a framework which allows you to build native mobile apps with JavaScript and React. React Native will enable you to develop for many platforms such as iOS and Android at the same time. “learn once, write anywhere.” I already like the sound of that.

##Getting set up
Getting your dev environment set up requires you to install `create-react-native-app`. That's it. Nice job Facebook.

You'll need some way to test your application on various devices so download Expo which will get your app running on your devices. If you don't have physical devices, you can emulate iOS devices on a mac using Xcode and Android devices using Android studio. Getting the emulators all set up and running took me quite a bit of time and required lots of tinkering to get them to work correctly. I expect most of this is due to my inexperience using these emulators.

Much like web vs native, there are distinctions between the UI of an android and an iOS app. There is also a different experience for each device, so it is vital to retain this consistency, making your app easy for your users. As a designer, it is great to see a peppering of UI fundamentals in a dev-heavy course.

##React Native Components
React Native has its own set of components to help build the UI for each platform. I like to think of these components like native-specific HTML elements which get rendered differently, depending on the platform. Mobile devices typically navigate by touch, so gestures, known as 'Touchables' are components which provide the all-important interaction between your user's fingers and the app.
React Native comes with a bunch of default components which put complicated to build functionality into the hands of anyone who can write JavaScript.

##Persisting Data
Application data can be stored using AsyncStorage and works much like the browser equivalent localStorage. Since Redux works with React Native, you can save your redux store in the AsyncStorage so your application can pick up from where it left off.

##App Appearance and Layout
The layout of React Native apps is managed using Flexbox (with a few quirks), which is excellent news since I'm already familiar with Flexbox. For a more native feel, the Platform API contains specific code to style your components to conform to the native platform style.

##Styling
Great news for those of you that know CSS! You can style a React Native app using CSS, which means one less thing to learn. React Native uses a StyleSheet API to create stylesheets out of javascript objects. You can keep the styling out of the render function which makes it much more readable. There are also CSS in JS libraries such as Glamorous and Styled Components which couple the styling with the component. On a first look of the Styled Components library, it seems that you can have a theme component which gives you the ability to pass down variables to use in your CSS. Themes or variables allow you to maintain consistency as well as update the look and feel of the app from a single point.

##Building Navigation
Thankfully navigation is something that is handled by React Native. There are a bunch of navigator components built right in. These navigator components conform to the style and behaviour of a native app. The TabNavigator component creates native tabs (like the Instagram nav) in your app which allow you to switch between views. The StackNavigator lets you transition between screens which stack on top of each other. The DrawerNavigator component creates a sliding drawer which can slide in from either side of the app.

##Native Features
These are the most exciting features for me which improve the user experience and make your app feel like you made it in Xcode. These are the deeper routed device functions such as geolocation, animation, local notifications and image picker file browser. I'm very excited to play with these features.

##Summary
After working through the previous two sections and assignments, I'm beginning to get the hang of React. The React Native sections have been an exciting finish to this course. I've always wanted to build and release a mobile app but have stalled many times with committing time to learn Swift. React Native has given me the confidence that I needed to develop and publish my app. An app that I can hold in my hands and use. The testing environments were pretty tricky to get working and playing nicely at first, but I guess the same goes for learning anything for the first time. I'm excited to kick off with this final assignment and build my first ever app.
