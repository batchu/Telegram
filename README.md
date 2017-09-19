## Better help with Vennela for Android

Clone the repo

git clone REPO_URL

Make sure that it's recursive and includes all the sub modules

git submodule update --init --recursive

Add the necessary Environment Vars (ANDROID_HOME, NDK_HOME, JAVA_HOME) and the necessary executable folders to your path


Open up SDK Manager. Go to SDK Tools. Ensure that CMAKE, LLDB & NDK are all installed.
Open up AVD Manager to create a new virtual device.

Fire up an emulator

emulator -avd ARMEABI-v7a -gpu off


To list the available emulators do this

emulator -list-avds


Build and run the apks

./gradlew installArmv7Debug

