# Android Integration Test

## Espresso Library
Espresso helps you:

- Interact with views, like clicking buttons, sliding a bar, or scrolling down a screen.
- Assert that certain views are on screen or are in a certain state (such as containing particular text, or that a checkbox is checked, etc.).

### Espresso Setup
1. Make sure the library is added up in **app/build.gradle**
> androidTestImplementation "androidx.test.espresso:espresso-core:$espressoVersion"
2. Turn off device / emulator **Window animation scale, Transition animation scale, and Animator duration scale** in `Developer Options`

### Espresso Example
![espresso-example](https://user-images.githubusercontent.com/12756891/118758424-38f4b380-b899-11eb-9c2b-e87037beea72.png "Espresso example")

source : 
- [Espresso](https://developer.android.com/training/testing/espresso)
- [Training Link](https://developer.android.com/codelabs/advanced-android-kotlin-training-testing-test-doubles)
