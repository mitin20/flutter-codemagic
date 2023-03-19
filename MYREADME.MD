# pre-req
HOMEBREW_NO_AUTO_UPDATE=1 brew install flutter

# using GPT
GPT: give me a flutter hello world web app and instructions to run it locally
```
import 'package:flutter/material.dart';

void main() {
  runApp(
    MaterialApp(
      home: Scaffold(
        body: Center(
          child: Text('Hello, world!'),
        ),
      ),
    ),
  );
}

```
# create project
flutter create my_app

# Replace the contents of lib/main.dart
cd my_app
vim lib/main.dart
```lib/main.dart
import 'package:flutter/material.dart';

void main() {
  runApp(
    MaterialApp(
      home: Scaffold(
        body: Center(
          child: Text('Hello, world!'),
        ),
      ),
    ),
  );
}

```

# Run the app: Open your terminal/command prompt and navigate to the my_app folder. Run the following command:
flutter run -d chrome

# lets try with an android one
GPT: now give me an android hello world app with instructions to run it locally

flutter create my_hello_world_app
cd my_hello_world_app
vim lib/main.dart
```lib/main.dart
import 'package:flutter/material.dart';

void main() => runApp(MyApp());

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Hello World',
      home: Scaffold(
        appBar: AppBar(
          title: Text('Hello World'),
        ),
        body: Center(
          child: Text(
            'Hello, World!',
            style: TextStyle(fontSize: 32.0),
          ),
        ),
      ),
    );
  }
}

```
# ensure with
flutter doctor

# check emulators
flutter devices

# choose emulator
flutter emulators --launch <emulator_id>

# alt
Connect your Android device to your computer with a USB cable.

# Run flutter run to launch the app on your device or emulator.
flutter run