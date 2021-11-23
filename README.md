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
* preferences -> editor ->genral -> autoimport -> dropdown insert import for all 

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
|     |
|     |->  AndroidManifest.xml  // for adding permission for the the operatioss for the uses 
|                               // change the main activity to something else activity for app 
|                               // change the label of the app 
|-> java 
|     |-> all java files MainActivity File and test files   
|-> java(generated)
|-> res
|     |-> activity_xx.xml  // all the xml resources for the layouts 
|     |-> values           
|           |-> strings.xml // configration for key value pair for ui  
|-> res(generated)
|-> Gradle scripts 
|     |->  build.gradle    // for the importing lib 
```


### Activity 
* pages on the app 

### Main Actitity 
* home page on the app 

### android.content.Intent Class 
* sharing data between Activity using Intent 

* source Activity 
```
Intent i = new Intent(context,SubActivityName.class);
i.putxtras("key","value");
istartActivitty(i);
```

* Destination Activity 
```
Intent i = getINtent();
String value = i.getStringExtra(key);
```

### for Log 
* Import android.util.lOg
* Log.d(tag="xx",msg="xxx")

### android.view.View Class 
* EditVeiw 
* TexttView 
* Button 

### To get the Component by its id 
* R.id.[id_name]
* findViewById(R.id.[id_name]) 

### Toast 
* Toast.makeText(content,msg,Toast.LENGHT_LONG).show()
* this / ClassName.this

### Creating Child Acttivity 
* select the java package and right click on that 
* new -> Activity -> Empty Activity -> name -> package type -> langauge = java -> finish 


### How to Change the Main Activity 
* AndroidManifest.xml 
```
<activity android:name ".xxx" 
		  android:label="xxxxx">
          <activity android:name ".xxx" 
		            android:label="xxxxx">
                     // ADD THE BELOW INENT-FILE TAG TO ANY ACTIVITY AND MAKE IT MAIN ACTIVITY 
                      <intent-filter>
                          <action android:name="android.intent.action.MAIN"/>
                          <action android:name="android.intent.category.LAUNCHER"/>
                      </intent-filter>	

		  </activity >	
</activity >		  
```


### Creating a navigation for activity 
* AndroidManifest.xml 
```
<activity android:name ".xxx" 
		  android:label="xxxxx"
		  adnroid:parentActivityName".ParentActivity"/>
```