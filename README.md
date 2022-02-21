```
npm i -g appium
appium
appium-doctor --ios
```

```
xcodebuild -showsdks
Simulator - iOS 15.2          	-sdk iphonesimulator15.2
```

```
Go to project directory and execute
xcodebuild -sdk iphonesimulator15.2
Copy the path of simulator
```

```
/Users/saiashishdarapureddy/Desktop/folders/IOS\ Development/
appiumTest/build/Release-iphonesimulator/appiumTest.app
```

```
Xcode => Open Developer Tool => Simulator
```

```
Download appium dmg file (appium.io) from here : https://github.com/appium/appium-desktop/releases/tag/v1.22.2
```

```
Click on the Apple icon in your system. 
Go to the System Preferences->Security Privacy-> General.
Click on the open anyway button from the bottom.
Run again Appium inspector screenshot.28-Jun-2021
```

```
Appium Inspector
```

```
After starting server using appium desktop,
select search icon to open appium inspector. At the new window
```

```
Add following details:
deviceName iPhone 13
platformName iOS 
platformVersion 15.2 
udid EBDA7F9A-95AF-4A37-A04E-2FCF311E2AEC (top)
app /Users/saiashishdarapureddy/Desktop/folders/IOS Development/appiumTest/build/Release-iphonesimulator/appiumTest.app
noReset true appium will re-install app if it already exists
automationName XCUITest
```

```
Bug:
Failed to create session. The requested resource could not be found, or a request was received using an HTTP method that is not supported by the mapped resource
```

```
Fix:
1. Go to Appium Server GUI -> Advanced
Server address: localhost
Port: 4723
Allow CORP: yes

2. Go to Appium Inspector
Remote host: localhost
Port: 4723
Path: /wd/hub

3. Allow Unauthorized Certificates

4. Select your capabilities

5. Start server
```

```
Xcode -> Window -> Devices and Simulators -> Select Device for which you want identifier (Inside details you can see identifier)
```

```
Appium’s XCUI Driver => IOS Device  (  WebDriverAgent + XCUI Library )
```
