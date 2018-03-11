# The App Sandbox



## Inter process communication in Android
* Intents
* Messenger
* ContentResolver
* Binder/IBinder

## Example of Data sharing between different processes


## What classes/methods do we need? Step1
* App2 wants to read data from App1
* It needs installation informationof App 1
* Get the Package Manager using [getPackageManager()]() of Context class
* PackageManager contains various kinds of information related to the application packages that are currently installed on the device.


## What classes/methods do we need? Step2
* Call ApplicationInfo getApplicationInfo(String packageName, int flags) of PackageManager to retrieve all of the information about app 1.
* packageName = package name of App 1
* flags = Any combination of
  GET_META_DATA,
  GET_SHARED_LIBRARY_FILES,
  GET_UNINSTALLED_PACKAGES to modify the data returned.
  
## What classes/methods do we need? Step2
* ApplicationInfo corresponds to information collected from the AndroidManifest.xml's <application>
* Find the directory containing Ap1's persistent data using dataDir variable of ApplicationInfo
  
  
  
  

