# Thermal Suit Display V21.1

Build-repair release of V21. UI, media, touch implementation and boot/launcher behavior are unchanged.

## Build fix
Plugin versions are declared both in the root `build.gradle.kts` and in `settings.gradle.kts` pluginManagement. This avoids the `Plugin [id: 'com.android.application'] was not found` failure caused by a missing/out-of-sync root plugin declaration.

## Required repository structure
```
app/
  build.gradle.kts
  src/
build.gradle.kts
settings.gradle.kts
gradle.properties
```

The GitHub workflow also verifies the structure before compiling.
