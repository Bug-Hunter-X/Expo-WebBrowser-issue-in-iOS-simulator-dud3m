# Expo WebBrowser issue in iOS simulator

This repository demonstrates an issue with Expo's WebBrowser.openBrowserAsync() function in the iOS simulator. The function does not open the specified URL in the simulator, while it works correctly on a physical device.

## Bug Description

The issue lies in the fact that WebBrowser.openBrowserAsync() fails to open the URL in the iOS simulator. It returns a result object, but the URL is not opened in a new browser tab. This behavior is only seen in the simulator and not on physical iOS devices.

## Solution

The solution involves using a different method to open URLs in the iOS simulator. This will ensure that the links are opened in the default browser.

## How to reproduce the issue

1. Clone this repository.
2. Install the dependencies using `npm install`.
3. Run the app in the iOS simulator.
4. Try clicking the button, which is supposed to open a URL in the browser.