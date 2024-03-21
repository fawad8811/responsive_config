# Responsive Config

A package for handling responsiveness in Flutter applications by providing utilities to calculate proportionate screen sizes.

## Introduction

Responsive Config is a Flutter package designed to simplify handling responsiveness in Flutter applications. It provides utilities to calculate proportionate screen sizes based on the device's screen size, making it easier to create layouts that adapt to various screen sizes.

## Features

- Calculate proportionate screen height and width based on the device's screen size.
- Easy to use and integrate into Flutter projects.
- Helps in creating responsive layouts that adapt to different screen sizes.
- Lightweight and efficient.

## Getting Started

### Installation
To use this package, add `responsive_config` as a dependency in your `pubspec.yaml` file.

```yaml
dependencies:
  responsive_config: ^version_number
```
## Usage
Import the package in your Dart code.Find the usage below.

```dart
class ExampleScreen extends StatelessWidget {
  const ExampleScreen({super.key});

  @override
  Widget build(BuildContext context) {
    // You need to initialize SizeConfig before using it
    SizeConfig().init(context);
    return Scaffold(
      appBar: AppBar(
        title: const Text('Example Screen'),
      ),
      body: Center(
        child: Column(
          mainAxisAlignment: MainAxisAlignment.center,
          children: [
            Text(
              'Proportionate Height: ${getProportionateScreenHeight(100)}',
            ),
            Text(
              'Proportionate Width: ${getProportionateScreenWidth(100)}',
            ),
          ],
        ),
      ),
    );
  }
}
```
## Additional information

Contributions and bug reports are welcome! Please feel free to contact mawais3665@gmail.com