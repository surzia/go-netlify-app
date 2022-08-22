# README
![](logo.jpeg)

Host a simple Go web application in Netlify

**Live Preview**

[![Netlify Status](https://api.netlify.com/api/v1/badges/575f6c75-113a-4512-879b-2dd4f888547f/deploy-status)](https://app.netlify.com/sites/go-netlify-app/deploys)

## Write a function

The [Netlify docs](https://docs.netlify.com/functions/build-with-go/) for golang are a great starting point.

## Build the binary
Push code to GitHub and instruct the Netlify CI on how to use the source code to build.

## Deploy to Netlify
Configure the settings in a `netlify.toml` file in the root of project.

```toml
[build]
  command = "${build command}"
  functions = "functions"
  publish = "${static html file}"
```