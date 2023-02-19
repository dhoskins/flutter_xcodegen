# xcodegen

This codebase is a vanilla Flutter project created using `flutter create`, with the default `Runner.xcodeproj` and `Runner.xcworkspace` replaced with an Xcodegen `project.yml`.

The `project.yml` file was inspired by [this Medium article](https://liewjuntung.medium.com/flutter-solving-ios-xcodeproj-merge-conflicts-with-xcodegen-3e1fff77ea93).

The default Flutter app runs well from within Xcode, but `flutter run` gives the following error:

```
Launching lib/main.dart on iPhone 13 mini in debug mode...
Running Xcode build...
Xcode build done.                                           12.7s
Build succeeded but the expected app at /Users/.../xcodegen/build/ios/Debug-iphonesimulator/Runner.app not found
Could not find the built application bundle at build/ios/iphonesimulator/Runner.app.
Error launching application on iPhone 13 mini.
```

Steps:

- Install `xcodegen`
- In the `iOS` folder, run the command `xcodegen`
- In the root folder, run `flutter run`
