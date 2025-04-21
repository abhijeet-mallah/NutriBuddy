# NutriBuddy
NutriBuddy is a Flutter-based mobile application designed to help users track their nutrition, fitness, and health goals. With features like meal alarms, step tracking, food recognition, and weekly reports, NutriBuddy empowers users to maintain a healthy lifestyle through personalized tracking and notifications.

---

## **Features**
### 1. **Meal Alarms**
- Set reminders for meals to maintain a consistent eating schedule.
- Notifications are sent using the `Awesome Notifications` package.
- Powered by `Android Alarm Manager` for scheduling alarms.

### 2. **Step Tracking**
- Tracks daily steps, distance, and duration.
- Displays hourly step data in a bar graph (X-axis: hours, Y-axis: steps with 500-step intervals).
- Sends notifications when daily step goals are achieved.
- Hourly step data is stored locally using `SharedPreferences` and synced to Firestore for previous days.

### 3. **Food Recognition**
- Recognizes food items using AI and provides nutritional information.
- Helps users log meals and track calorie intake.
- Integrates with APIs for food recognition and nutritional data.

### 4. **Weekly Reports**
- Summarizes weekly progress for steps, meals, and hydration.
- Displays data in a user-friendly format with charts and insights.
- Allows users to export reports as PDFs.

### 5. **Customizable Themes**
- Light and dark themes for better user experience.
- Users can switch themes from the settings screen.

### 6. **Notifications**
- **Meal Alarms**: Reminders for scheduled meals.
- **Step Goals**: Alerts when daily step goals are achieved.
- **General Notifications**: For app updates and reminders.

---

## **Technologies Used**
- **Flutter**: Cross-platform framework for building the app.
- **Firebase**:
  - **Authentication**: For user login and registration.
  - **Firestore**: For storing user data (e.g., steps, meals, reports).
  - **Cloud Functions**: For handling background tasks.
- **SharedPreferences**: Local storage for caching user data.
- **Android Alarm Manager**: For scheduling meal alarms.
- **Awesome Notifications**: For creating and managing notifications.
- **Provider**: For state management (e.g., theme switching).

---

## **Project Structure**
```
lib/
├── main.dart                     # Entry point of the application
├── screens/                      # Contains all UI screens
│   ├── login_screen.dart         # Login screen
│   ├── register_screen.dart      # Registration screen
│   ├── dashboard_screen.dart     # Main dashboard
│   ├── weekly_report_screen.dart # Weekly reports screen
│   ├── meal_alarm_screen.dart    # Meal alarm management
│   ├── food_recognition_screen.dart # Food recognition screen
│   ├── settings_screen.dart      # App settings screen
│   ├── profile_screen.dart       # User profile screen
│   └── splash_screen.dart        # Splash screen
├── services/                     # Contains background services
│   └── alarm_service.dart        # Handles alarm scheduling
├── providers/                    # State management
│   └── theme_provider.dart       # Manages app-wide theme state
├── utils/                        # Utility files
│   └── theme.dart                # Custom themes for the app
└── firebase_options.dart         # Firebase configuration
```

---

## **How to Run**
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/nutribuddy.git
   cd nutribuddy
   ```
2. Install dependencies:
   ```bash
   flutter pub get
   ```
3. Configure Firebase:
   - Add your `google-services.json` (for Android) and `GoogleService-Info.plist` (for iOS) files to the respective directories.
4. Run the app:
   ```bash
   flutter run
   ```

---

## **Future Enhancements**
- **AI-Powered Insights**:
  - Provide personalized health recommendations based on user data.
- **Integration with Wearables**:
  - Sync data from fitness trackers like Fitbit and Apple Watch.
- **Social Features**:
  - Allow users to share progress and compete with friends.

---

## **Contributing**
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add feature-name"
   ```
4. Push to your branch:
   ```bash
   git push origin feature-name
   ```
5. Open a pull request.

---

## **License**
This project is licensed under the MIT License. See the `LICENSE` file for details.

