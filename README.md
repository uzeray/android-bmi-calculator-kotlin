# BMI / Ideal Body Weight Calculator (Android, Kotlin)

A small native Android app that calculates **Body Mass Index (BMI)** and **Ideal Body Weight (IBW)** from user-entered age, weight, and height, and passes the results to a second screen via an `Intent`.

Originally built for [FitPatients.com](https://fitpatients.com) as a learning exercise in core Android/Kotlin fundamentals: activity lifecycle, form input handling, input validation, and passing data between activities.

## What it does

1. **Home screen** (`MainActivity`) — entry point with navigation buttons.
2. **Input form** (`BmrForm`) — takes age, weight (kg), and height (cm); validates that all fields are filled and within a sane range.
3. **Result screen** (`BmiResultScreen`) — receives the calculated BMI and IBW via `Intent` extras and displays them.

BMI is computed as `weight / (height_m)²`; IBW is derived from the difference between the calculated BMI and a target healthy BMI of 23.

> The home screen also has placeholder buttons for BMR (male/female) and diabetic calculators that are not wired up yet — the BMI/IBW flow described above is the complete, working feature.

## Stack

Kotlin · Android SDK · AppCompatActivity · Gradle

## Running it

Open the project in Android Studio and run on an emulator or device (`minSdk`/`targetSdk` as configured in `app/build.gradle`).

## Author

Ünal Zeray
