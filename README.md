# Authenticator
### Two-Factor Authentication Client for iOS.


[![MIT License](http://img.shields.io/badge/license-mit-blue.svg?style=flat)](LICENSE.txt)


## Getting Started

1. Check out the latest version of the project:
  ```
  git clone https://github.com/mattrubin/Authenticator.git
  ```

2. In the Authenticator directory, check out the project's dependencies:
  ```
  cd Authenticator
  git submodule update --init --recursive
  ```

3. Open the `Authenticator.xcworkspace` file.
> If you open the `.xcodeproj` instead, the project will not be able to find its dependencies.

4. Build and run the "Authenticator" scheme.


## Managing Dependencies

Authenticator uses [Carthage] to manage its dependencies, but it does not currently use Carthage to build those dependencies. The dependency projects are checked out as submodules, are included in `Authenticator.xcworkspace`, and are built by Xcode as target dependencies of the Authenticator app.

To check out the dependencies, simply follow the "Getting Started" instructions above.

To update the dependencies, modify the [Cartfile] and run:
```
carthage update --no-build --use-submodules
```

[Carthage]: https://github.com/Carthage/Carthage
[Cartfile]: Cartfile


## License

This project is made available under the terms of the [MIT License](http://opensource.org/licenses/MIT).

The modern Authenticator grew out of the abandoned source for [Google Authenticator](https://code.google.com/p/google-authenticator/) for iOS. The original Google code on which this project was based is licensed under the [Apache License, Version 2.0](https://www.apache.org/licenses/LICENSE-2.0).
