# pre-req
HOMEBREW_NO_AUTO_UPDATE=1 brew install flutter

# using GPT
: give me a flutter hello world web app and instructions to run it locally
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
