android-proguard-snippets
==========================

Example Proguard configurations for common Android libraries

### Usage
```groovy 
android {
  buildTypes {
    release {
      runProguard true
      // Library specific proguard files
      proguardFile 'proguard-google-play-services.pro'
      proguardFile 'proguard-gson.pro'
      ...
      // Default proguard files
      proguardFile 'proguard-project.pro'
      proguardFile getDefaultProguardFile('proguard-android.txt')
    }
  }
}
```

### Libraries
* ACRA 4.5.0
* ActionBarSherlock 4.4.0
* Amazon Web Services 1.6.1 / 1.7.0
* Butterknife 5.1.2
* EventBus 2.0.2
* Google Analytics 3.0+
* Google Guava
* Google Play Services 4.3.23
* GSON 2.2.4
* Flurry 3.4.0
* New Relic
* Square Otto
* Square Picasso
