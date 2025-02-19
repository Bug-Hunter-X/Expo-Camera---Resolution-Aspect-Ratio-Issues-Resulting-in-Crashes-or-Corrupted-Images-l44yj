# Expo Camera Resolution/Aspect Ratio Bug

This repository demonstrates a bug in the Expo Camera API where attempting to use unsupported resolutions or aspect ratios can cause crashes or unexpected image output.  The issue is compounded by unhelpful error messages, making it challenging to troubleshoot.

## Bug Description

When specifying a particular camera resolution or aspect ratio using the Expo Camera API, the application may crash, freeze, or generate an image with incorrect dimensions or noticeable artifacts.  The error messages provided are often insufficient for effective debugging.

## Reproduction Steps

1. Clone the repository.
2. Install dependencies: `npm install`
3. Run the app: `expo start`
4. Attempt to take a picture.  Observe if crashes or unexpected image output occur based on the resolution/aspect ratio settings in `bug.js`.

## Solution

The solution involves implementing robust error handling and dynamically adjusting the camera settings based on the device's capabilities.  This prevents attempts to use unsupported configurations. The improved code is in `bugSolution.js`

## Contributing

Contributions are welcome!