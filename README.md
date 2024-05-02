# agora-ui-kit-customize
### Customizing UI with Agora UI KIT
If you're looking to tailor the user interface (UI) of your application using Agora UI KIT, you've come to the right place! Below, we'll walk 
you through how to customize the UI to fit your specific needs.

Getting Started
First, integrate Agora UI KIT into your project by passing props to the AgoraUIKit component. These parameters are predefined and accept only valid inputs.

![image](https://github.com/mayurmewada/agora-ui-kit-customize/assets/84275081/61bbee30-5c55-4328-ac8a-dd70638f6d29)


<AgoraUIKit
  styleProps={styleProps}
  callbacks={callbacks}
  rtcProps={rtcProps}
  AppID={rtcProps.appId}
  token={rtcProps.token}
/>
Customizing Style Props
The styleProps object allows you to tweak various aspects of the UI to match your design requirements. Below are some examples of style properties you can modify:

pinnedVideoContainer: Styling for the main video container.
maxViewContainer: Styling for the maximum view container.
scrollViewContainer: Styling for the scroll view container.
localBtnContainer: Styling for the local button container.
minViewContainer: Styling for the minimum view container.
localBtnStyles: Styles for specific local buttons like mute video, mute audio, and end call.
customIcon: Custom icons for mic, mic off, videocam, videocam off, and call end.
Feel free to adjust these properties according to your preferences.

Handling Callbacks
Callbacks allow you to define actions triggered by specific events within the UI. Here's an example of how you can handle the EndCall callback:

const callbacks = {
  EndCall: () => { 
    if (dimensions.width < 991) {
      setShow(!show);
    } else {
      setChatVisible(!chatVisible);
    }
  },
}; 
In this example, the EndCall callback toggles the visibility of a chat window based on the screen width.

Usage
You can seamlessly integrate the provided code snippets into your project to achieve a customized UI tailored to your application's needs.

Feel free to experiment with different style properties and callbacks to create a unique user experience for your users.
