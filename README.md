# VrCubeWorld_NativeActivityVS
Version of the Oculus Mobile SDK sample VrCubeWorld_NativeActivity that builds and runs from Visual Studio 2019.

I've done my best to keep this as unchanged from the original Android Studio / Gradle project as possible.  

The package is installed as com.guiltydog.vrcubeworldna - I tried to keep it as per the original but then the app stopped running.

Known issues:

If you tap the Oculus Button on the right Touch Controller while the debugger is attached you'll get an Illegal instruction exception.  You can hit F5 a couple of time to Continue execution. This is suppoer annoying but I haven't yet figured out how to fix it.  To close the application in this situation just use Debug -> Stop Debugging.

I haven't figured out how to switch between Debug / Release versions of libvrapi.so as located in VrCubeWorld_NativeActivityVS.Packaging\libs\arm64-v8a. I've not found it a big deal as there is no source code for that library anyway, but it might be a problem in some instances.
