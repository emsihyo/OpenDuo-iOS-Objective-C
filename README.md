# Agora OpenDuo for iOS (Objective C)

*其他语言版本： [简体中文](README.zh.md)*

The Agora OpenDuo sample app supports the following platforms:
* [iOS](https://github.com/AgoraIO/OpenDuo-iOS-Objective-C)
* [Android](https://github.com/AgoraIO/OpenDuo-Android)
* [Web](https://github.com/AgoraIO/OpenDuo-Web)

This readme describes the steps and considerations for demonstrating the Agora OpenDuo iOS sample app.

## Introduction

Built upon the Agora Video SDK and the Agora Signaling SDK, the Agora OpenDuo for iOS is an open-source demo that integrates video chat into your Web applications.

This sample app allows you to:

- Login the signaling server
- Make a call
- Accept or hang up a call
- Mute/unmute a user
- Switch the camera

## Preparing the Developer Environment

* Xcode 9.0 or later
* An iPhone or iPad

NOTE: The iOS emulator is NOT supported.

## Running the App
1. Create a developer account at [Agora.io](https://dashboard.agora.io/signin/), obtain an App ID, and enable the App Certificate. 
2. Fill in the AppID and the App Certificate in the *KeyCenter.mm*.

        static NSString * const kAppID = @"Your App ID"
        static NSString * const kAppCertificate = @"Your App Certificate";

3. Download the **Agora Video SDK** and the **Agora Signaling SDK** from [Agora.io](https://www.agora.io/en/download/).
4. Unzip the downloaded **Agora Video SDK** and copy **libs/AgoraRtcEngineKit.framework** to the *OpenDuo* folder of your project.
5. Unzip the downloaded **Agora Signaling SDK** and copy **libs/AgoraSigKit.framework** to the *OpenDuo* folder of your project.
6. Open OpenDuo.xcodeproj, connect your iPhone/iPad device, set up your code signature, and run the sample app.

## About the Dynamic Key

This sample project provides a preset Dynamic Key. For security reasons and to avoid errors, Agora recommends generating the Dynamic Key on your business server. 

For information on SignalingToken, see [SignalingToken](https://docs.agora.io/en/2.2/addons/Signaling/Agora%20Basics/key_signaling?platform=All%20Platforms).

For information on AccessToken, see [AccessToken](https://docs.agora.io/en/2.2/product/Interactive%20Broadcast/Agora%20Basics/key_native?platform=Android). 

## Contact Us

- You can find the API documentation at [Developer Center](https://docs.agora.io/en/).
- You can report issues about this demo at [issue](https://github.com/AgoraIO/OpenDuo-iOS-Objective-C/issues).

## License

The MIT License (MIT). 

