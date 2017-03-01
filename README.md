# Deloitte Digital Academy iOS Training - Lesson 3
*iOS -- Backend Integration, using Firebase*

## Install CocoPods:
1) open terminal and paste the following:
sudo gem install cocoapods
```javascript
[sudo gem install -n /usr/local/bin cocoapods]
```

2) In terminal navigate to your working Directory and run:

```javascript
pod init
```

3) You will see in the directory an empty Podfile.

4) Open the pod file using a text editor, and add between the "  # Pods for FirebaseFirstLook-iOS" and "end" lines:

```javascript

pod ‘Firebase/Core’
pod ‘Firebase/Auth’
pod ‘Firebase/RemoteConfig’

```

5) Save the file and close the text editor.

6) Next we will install the pods via the Podfile.

```javascript
pod install
```

If you have setup Firebase during Lesson 3 - your done setting up. if not.

## Setting up Firebase:
1) Login using Gmail/Google account

2) Click on “Add Firebase to your iOS app”

3) Enter your bundle name; i’m using com.davidkalman.ddfirebase - but do what you want

4) DO NOT ENTER ANYTHING ELSE

5) Click Add app

6) It will prompted you to download a PLIST file, download it. there is a sample file in the repo for you to use to connect to the sample firebase if you dont want to make your own

7) Drag it to the files section in Xcode; and FINISH in the window that Xcode pops up. 

8) back in the Firebase window, click next, next, finish - we dont need any of that at this point of time.


## Configing your XCode project
1) Open the XcodeWorkspace (White Xcode Icon, not Blue)

2) goto App Delegate; and add the following line under the comment:
// TODO: Call the Firebase app configuration code

```javascript
FIRApp.configure()
```

If there are any more questions; send any one of the Apple Training Team an email.

THANKS! :)