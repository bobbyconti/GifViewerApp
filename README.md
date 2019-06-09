# GifViewer

## :clipboard: Overview

<div style="width: 1000px; height 600px;"><img src="screencap.gif" width="30%" height="30%" align="right"></div>

GifViewer is an iOS app that allows users to browse trending gifs from the Giphy API. Users can scroll through the grid, select a gif, which opens a detail view of the gif, and then tap or swipe right to dismiss. The app incorporates:

- Objective-C
- Collection Views
- Detail Views
- NSURLSession
- Accessing APIs
- Parsing JSON
- UIView Animations
- Gestures

## :hammer_and_wrench: Custom Features

Additional features were added to the original functionality of the app, including:

- Collection View Header (UICollectionReusableView)
- Auto Layout (shows 3-column, auto-sizing layout on all devices)

## :white_check_mark: Getting Started

> :warning: This app is not available on the App Store.

### Prerequisites

- A valid API key from Giphy
- A Mac running Xcode

### Installation

1. Clone or download the project to your local machine
2. Open the project in Xcode
3. Replace `YOURAPIKEY` with your valid Giphy API key in `CollectionViewController.m`

```objc
- (void) refreshImages {
    NSURLSession *session = [NSURLSession sharedSession];
    NSURL *url = [NSURL URLWithString:@"https://api.giphy.com/v1/gifs/trending?api_key=YOURAPIKEY&rating=pg"];
```

4. Run the simulator

## :clap: Acknowledgements

The following resources were used in the development of this project. All custom code is my own.

- [Displaying API Data with Collection Views in Objective-C](https://teamtreehouse.com/library/displaying-api-data-with-collection-views-in-objectivec-2)

Interested in learning more about iOS Development? [Sign up today](http://referrals.trhou.se/bobbyconti1)!
