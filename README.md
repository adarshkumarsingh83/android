# android

> Android Application development 


----

# Android 

---

## Installing Ide for Android 
* Install jdk on machine 
* Download "Android Studio" and install it 
	* https://developer.android.com/studio
* new project -> empty activity -> name -> package name -> langauge = java -> finish 

### Ide settings 
* preferences -> editor -> generatl -> chagen gont size (zoom) with cmd|mounse wheel

### Adding emulator on the ide 
* Open Dvd Manager -> create virutal device -> select the type of phone and the -> next -> system image (android os version) -> download -> finish 
name -> orientation -> finish 


### adding actual phone with ide 
* apps -> setings -> system -> aboutdevice -> build no -> tap for 7 times -> then developer option will appers -> usb debugging on -> 
* connect with usb to the machine and install drivers if required 
* then phone will pop up with option for 
* after that it will show as option with emulator for installing app/deployeing app to the phone 


### Structure of the project 
```
app
|-> manifests  
|     |->  
|-> java 
|     |-> all java files MainActivity File and test files   
|-> java(generated)
|-> res
|     |-> activity_xx.xml  // all the xml resources for the layouts 
|     |-> values           // configration for key value pair for ui  
|-> res(generated)
|-> Gradle scripts 
|     |->  build.gradle    // for the importing lib 
```


### Activity 
* pages on phone

### Main Actitity 
* home page on the app 

### Intent 
* sharing data between Activity using Intent 
