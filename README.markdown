# Expense tracker using Scaloid

An Android application to keep track of your personal expenses, using [Scaloid](https://github.com/pocorall/scaloid).

Prerequisites
-------------
* Maven 3
* Android SDK
  - Both SDK Level 8 and the most recent version should be installed.

Build
-----
You can build using Maven:

    $ mvn clean package

This will compile the project and generate an APK. The generated APK is
signed with the Android debug certificate. To generate a zip-aligned APK
that is signed with an actual certificate, use:

    $ mvn clean package -Prelease

The configuration for which certificate to use is in pom.xml.

Run
---
Deploy to an Android virtual device (AVD):

    $ mvn android:deploy
