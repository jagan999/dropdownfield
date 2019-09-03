# dropdownfield
Custom Flutter Widget for a customizable dropdown field with auto-complete functionality
This widget is meant to be used within a Flutter Form

<img src="https://bitbucket.org/AndroidFreak/dropdownfield/raw/17b75f64d770ced35e16b1c32678062c56f483b1/example/dropdownfield.png" height="320px" >

## Installing:
In your pubspec.yaml, add the following dependency
```yaml
dependencies:
  dropdownfield: 1.0.0
```

## Example Usage:
```dart
import 'package:dropdownfield/dropdownfield.dart';

    DropDownField(
        value: accountname,
        required: true,
        strict: true,
        labelText: 'Account Name *',
        icon: Icon(Icons.account_balance),
        items: accountNames,
        setter: (dynamic newValue) {
            accountname = newValue;
        }
    ),
```
## Features:
Can be used for showing drop-down of suggestions for a form field
Provides auto-complete functionality - as the user types, shows all suggestions that match part of the typed in text
Provides validation of user-typed value against the list of suggestions by default. Can be turned off by setting strict=false
Provides ability to do "mandatory" value check if needed
Quick clear icon to clear out typed in value
Appearance can be customized to match your application theme
Clicking dropdown arrow will automatically close the soft keyboard

## License:
This project is licensed under the BSD License - see the LICENSE file for details
