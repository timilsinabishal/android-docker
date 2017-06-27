# android-docker
Docker image of android sdk for faster CI implementation

This repository consist of docker images for android-sdk. Currently two variants of docker images are available.The default dockerfile is suitable for continous integration. And second version of images consist of ruby with fastlane, it can be used in continous deployment using fastlane along with continous integration. I made this images specifically for gitlab-ci but this should work in all other CI tools too (which supports docker).

You can also pass arguments to build image to your need according to tools used in your project. Example
```
docker build -t android --build-arg ANDROID_COMPILE_SDK=25 ANDROID_BUILD_TOOLS=25.0.3 ANDROID_SDK_TOOLS=25.2.5 
```
Please visit [docker hub](https://hub.docker.com/r/timilsinabishal/android/) to see all the images.
