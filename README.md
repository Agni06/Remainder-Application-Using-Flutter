# Remainder-Application-Using-Flutter
To create a simple reminder application using Flutter and Dart as per the instructions, here's an overview of how to implement it step by step:

1. Setting Up Flutter Environment:
Install Flutter SDK and set up an IDE (like Android Studio or VS Code).
Create a new Flutter project:
flutter create reminder_app
cd reminder_app
2. UI Design:
The UI will consist of three dropdowns as described in the task:

Dropdown for selecting the day of the week.
Dropdown or time picker for selecting the time.
Dropdown for selecting the activity.
3. Flutter Widgets to Use:
DropdownButton: For days and activities.
Time Picker: Use showTimePicker for selecting the time.
Snackbar or AlertDialog: To notify the user when the reminder goes off.
Sound/Chime: Use the audioplayers package to play a sound when the reminder goes off.
4. Implementation of State Management:
Use StatefulWidget to handle state changes (such as dropdown selections and time).

5. Timer to Trigger Reminders:
Use Dart's Timer class to check the current time against the set reminder and play a sound when they match.
6. Steps to Run:
Place a chime sound file in the assets folder (e.g., assets/chime.mp3).
Add the following line in your pubspec.yaml file:
yaml
Copy code
assets:
  - assets/chime.mp3
Run the app using the Flutter run command:
bash
Copy code
flutter run
7. Packages Used:
audioplayers for playing the reminder sound: Add to pubspec.yaml:
yaml
Copy code
dependencies:
  audioplayers: ^0.20.1
This setup will allow users to select a day, time, and activity, and play a sound reminder when the time is reached.

