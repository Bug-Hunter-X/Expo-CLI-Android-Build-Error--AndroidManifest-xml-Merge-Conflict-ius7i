# Expo CLI Android Build Error: AndroidManifest.xml Merge Conflict

This repository demonstrates a bug encountered when building an Android app using the Expo CLI. The issue stems from a conflict during the merging of the main application's `AndroidManifest.xml` file and Expo's manifest.  The error messages are often vague, making diagnosis challenging.

## Bug Description

The build process fails with an error related to the `AndroidManifest.xml` file. The precise error message may vary, but it generally points to a conflict in the application ID, package name, or other attributes between the two manifests.  This can occur at different stages of the build.

## Reproduction Steps

1. Clone this repository.
2. `npm install` or `yarn install`
3. `expo start`
4. Attempt to build an Android APK using `expo build:android`.

## Solution

A solution is provided in the `bugSolution.js` file and described in the `solutionContent` section of this JSON.  The key is to carefully review and, if necessary, correct any discrepancies between your `app.json` and your `AndroidManifest.xml` (if you've customized it).