# Congratulations

![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?logo=kotlin&logoColor=white) ![Android](https://img.shields.io/badge/Android-3DDC84?logo=android&logoColor=white) ![Jetpack Compose](https://img.shields.io/badge/Jetpack_Compose-4285F4?logo=jetpackcompose&logoColor=white) ![minSdk 24](https://img.shields.io/badge/minSdk_24-555)

A first step into **Jetpack Compose**: a single-screen app with a `Scaffold`, a `Greeting` composable and a custom Material 3 theme. Small on purpose — it's the project where I learned how a Compose app is put together.

## Features

- `ComponentActivity` with `setContent { }` and edge-to-edge display
- `Scaffold` handling system-bar insets via `innerPadding`
- Custom **Material 3 theme** — colors, typography, light/dark and dynamic color
- `@Preview` with system UI for design-time iteration

## How it works

```kotlin
setContent {
    CongratulationsTheme {
        Scaffold(Modifier.fillMaxSize()) { innerPadding ->
            Greeting("Android", Modifier.padding(innerPadding))
        }
    }
}
```

## Project structure

```
com.example.congratulations
├── MainActivity.kt
├── ui/
│   ├── theme/Color.kt
│   ├── theme/Theme.kt
│   ├── theme/Type.kt
```

<sub>4 source files · 134 lines of code</sub>

## Tech stack

| | |
|---|---|
| **Language** | Kotlin |
| **UI** | Jetpack Compose |
| **Min / Target SDK** | 24 / 35 |

## Getting started

```bash
git clone https://github.com/rajabbov/Congratulations.git
```

1. Open the folder in **Android Studio** (Ladybug or newer).
2. Let Gradle sync.
3. Run the `app` configuration on a device or emulator.

---

Made by **Ibrohimjon Rajabboyev** · [@rajabbov](https://github.com/rajabbov)
