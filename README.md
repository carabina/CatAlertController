<p align="center">
	<img src="https://github.com/ImKcat/CatAlertController/raw/master/CatAlertController-Logo.png" alt="Logo">
</p>

<p align="center">
	<img src="https://img.shields.io/badge/Language-swift4-EF5138.svg?style=flat" alt="Language">
	<a href="http://cocoapods.org/pods/CatAlertController"><img src="https://img.shields.io/cocoapods/p/CatAlertController.svg?style=flat" alt="Support Platform"></a>
	<a href="http://cocoapods.org/pods/CatAlertController"><img src="https://img.shields.io/cocoapods/l/CatAlertController.svg?style=flat" alt="License"></a>
</p>

<p align="center">
	<a href="https://github.com/Carthage/Carthage"><img src="https://img.shields.io/badge/Carthage-compatible-4BC51D.svg?style=flat" alt="Carthage compatible"></a>
	<a href="http://cocoapods.org/pods/CatAlertController"><img src="https://img.shields.io/cocoapods/v/CatAlertController.svg?style=flat" alt="CocoaPods Version"></a>
</p>

<p align="center">
	<a href="https://travis-ci.org/ImKcat/CatAlertController"><img src="http://img.shields.io/travis/ImKcat/CatAlertController.svg?style=flat" alt="Travis CI Status"></a>
	<a href="https://codebeat.co/projects/github-com-imkcat-catalertcontroller-master"><img src="https://codebeat.co/badges/98f6b5c0-d53e-4e1d-836c-7b083e1368a4" alt="Codebeat"></a>
	<a href="https://beerpay.io/ImKcat/CatAlertController"><img src="https://beerpay.io/ImKcat/CatAlertController/badge.svg?style=flat" alt="Beerpay"></a>
</p>

- [Description](#description)
- [Requirements](#requirements)
- [Usage](#usage)
- [License](#license)

## Description

The `CatAlertController` is a high level manager object for `UIAlertController`.

## Requirements

- Swift 4+
- iOS 8.0+

## Usage

Here is the alert style sample code in iPhone:

```swift
CatAlertController(title: "CatAlertController", 
                    message: "This is CatAlertController", 
                    preferredStyle: UIAlertControllerStyle.alert)
                    .addAction(UIAlertAction(title: "Cancel", style: UIAlertActionStyle.cancel, handler: nil))
                    .addAction(UIAlertAction(title: "OK", style: UIAlertActionStyle.default, handler: nil))
                    .flash(from: self, animated: true, delay: 0.3, completion: nil)
```

Here is the action sheet style sample code in iPad:

```swift
// Don't worry the action sheet style present in iPad, it won't be crash, take it easy :)
CatAlertController(title: "Action Sheet Style", 
                    message: "This is CatAlertController", 
                    preferredStyle: UIAlertControllerStyle.actionSheet)
                    .addAction(UIAlertAction(title: "Item 1", style: UIAlertActionStyle.default, handler: nil))
                    .addAction(UIAlertAction(title: "Item 2", style: UIAlertActionStyle.default, handler: nil))
                    .addAction(UIAlertAction(title: "Item 3", style: UIAlertActionStyle.default, handler: nil))
                    .addAction(UIAlertAction(title: "Cancel", style: UIAlertActionStyle.cancel, handler: nil))
                    .flash(from: self, animated: true, delay: 1, completion: nil)
```

## License

CatAlertController is available under the MIT license. See the LICENSE file for more info.