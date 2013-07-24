apk-waveform-sample
=====================

A simple Glassware apk that receives audio input from the microphone and
displays it on the screen as an animated waveform, along with the decibel
level.

## Prerequistes

* [Android SDK](http://developer.android.com/sdk/index.html) - This is needed for development.
* [Glass](http://www.google.com/glass/start/how-to-get-one/) - You can push the code to an Android device but the goal of this project is to get started writing .apk for Glass.

## Importing and compiling the code

Checkout the code into your filesystem and use your favorite IDE to import and compile the code.

### In Eclipse and ADT

1. Click **File > Import ... > Existing Android Code into Workspace**.
2. Click **Browse**, select the location of the `apk-waveform-sample/` directory, and click **OK**.
3. Select the **apk-waveform-sample** project to import it and select
**Copy projects into workspace**.
6. Click **Finish** to complete the import.

### In Android Studio

1. Checkout the sample to a location where you keep your Android
development projects. A `apk-waveform-sample/` directory is created.
2. Click **File > Import Project...**, select the location of the `apk-waveform-sample/` directory, and click **Next** until you see the **Finish** button.
3. Click **Finish** to complete the import.


## Turning on debug mode

You'll need to turn on debug mode before you do any type of development on
Glass. Go to **Settings > Device Info > Turn on debug** to enable it.

## Push the .apk on Glass

You can use your IDE to compile, push and run the .apk or use this command line with `adb`:

    adb install -r apk-waveform-sample.apk

## Run the .apk

You can use your IDE to run the .apk or use this command line with `adb` when the Glass screen is **on**:

    adb shell am start -n com.google.glass.samples.waveform/.WaveformActivity
