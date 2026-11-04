# EXP 10 – Implementing Fragments in Android Studio using Kotlin

## Aim
To develop an Android application using **Fragments** in Kotlin, demonstrating communication between two fragments using Bundle arguments and Fragment Transactions.

## Objective
- To understand the concept of Android Fragments.
- To implement ListFragment and DetailFragment.
- To pass data from one fragment to another.
- To dynamically display course details when a user selects an item.

## Theory

A **Fragment** is a reusable portion of an Activity's user interface. It has its own layout and lifecycle and can be combined with other fragments inside an Activity.

Fragments help create flexible and modular Android applications.

### Types of Fragments Used

1. **ListFragment:** Displays a list of courses using ListView and ArrayAdapter.
2. **DetailFragment:** Displays information about the selected course.

### Fragment Communication

Data is passed between fragments using a Bundle.

- `Bundle`: Stores data in key-value pairs.
- `FragmentTransaction`: Adds, replaces, or removes fragments dynamically.
- `replace()`: Replaces the existing fragment with another fragment.
- `commit()`: Executes the fragment transaction.

## Application Description

The application displays a list of four programming courses:

- Android
- Java
- Kotlin
- Python

When the user selects a course, the application displays its corresponding description in the DetailFragment.

## Procedure

1. Open Android Studio.
2. Create a new project using the Empty Views Activity template.
3. Select Kotlin as the programming language.
4. Create the required fragment classes:
   - ListFragment.kt
   - DetailFragment.kt
5. Design the layouts for the fragments.
6. Implement ListView and ArrayAdapter in ListFragment.
7. Pass the selected course name using Bundle arguments.
8. Use FragmentTransaction to display DetailFragment.
9. Add the required fragment container in the activity layout.
10. Run the application on an emulator or Android device.
11. Select different courses and verify that their descriptions are displayed.

## Project Structure

```text
exp_10/
│
├── app/
│   └── src/
│       └── main/
│           ├── java/com/example/exp_10/
│           │   ├── MainActivity.kt
│           │   ├── ListFragment.kt
│           │   └── DetailFragment.kt
│           │
│           ├── res/
│           │   └── layout/
│           │       ├── activity_main.xml
│           │       ├── fragment_list.xml
│           │       └── fragment_detail.xml
│           │
│           └── AndroidManifest.xml
│
└── README.md
```

## Expected Output

1. The application displays four courses: Android, Java, Kotlin and Python.
2. When the user clicks on Android, its description is displayed.
3. When the user clicks on Java, its description is displayed.
4. Similarly, Kotlin and Python display their respective descriptions.

## Concepts Learned

- Android Fragments
- Fragment Lifecycle
- ListView and ArrayAdapter
- Bundle Arguments
- Fragment Transactions
- Dynamic UI Updates
- Kotlin Programming

## Result

Successfully developed and executed an Android application using Kotlin and Fragments. The application displays a list of programming courses and dynamically shows the corresponding course description when an item is selected.

## Conclusion

Through this experiment, we learned how to implement fragments in Android applications, communicate between fragments using Bundle arguments, and dynamically update the user interface using Fragment Transactions.
