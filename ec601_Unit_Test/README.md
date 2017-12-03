# EC601_Assignment 5 Unit Test:thumbsup::thumbsup::thumbsup:
## Brief Introduction :sunglasses:
  Hello Everyone! :trollface::trollface::trollface::trollface:
  
  This is the page for **EC601(Fall 2017) A1 Assignment 5 Unit Test** 
  [@github/qinjinjia/ec601_unit_test](https://github.com/qinjinjia/ec601_Unit_Test)
  
  The Author: :boy: **Qinjin Jia** qjia@bu.edu   :point_right:[@github/qinjinjia](https://github.com/qinjinjia)
  
  **The Unit Test Assignment is based on [EC601 HW2 Mini Project](https://github.com/qinjinjia/ec601_miniproject)**
      
  **Link:link:[https://ec601-hw2-task1-publish.firebaseapp.com](https://ec601-hw2-task1-publish.firebaseapp.com)** 
  
  **Link:link:[https://ec601-hw2-chat.firebaseapp.com](https://ec601-hw2-chat.firebaseapp.com)**
     
  :mailbox_closed:Please feel free to contact me, if you have any suggestions or concerns.
  
  
## :sun_with_face: **Task 1 - Test Cases**
   
**1) Generate your own test cases.**

**2) Run your own black box testing.**
  
  **Test Case Sheet Link:point_right: [Qinjin Jia's Resume Test Case Sheet.xlsx:link:](https://github.com/qinjinjia/ec601_Unit_Test/blob/master/Qinjin%20Jia's%20Resume%20Test%20Case%20Sheet.xlsx)** 
  
  Screenshot of the Test Case Sheet:
  
  <img src="https://github.com/qinjinjia/ec601_Unit_Test/blob/master/Unit%20Test%20Screenshot.png" width="400" height="200">

## :full_moon_with_face: **Task 2 - Automated Test**
  
**1) Run an automated test, e.g., AWS test farm and monkey test.**

**2) Interpret the results.**

**Due to the APP developed in HW2 is the Resume Website,**
**[CrossBrowserTesting](https://app.crossbrowsertesting.com/test-center) is used for the automated test**

The automated test tests the website on two differnt platforms: **Mac Safair(version 11) and Window 10 Chrome(version 61)**

[Script for Web automated Test on Mac Safari](https://github.com/qinjinjia/ec601_Unit_Test/blob/master/webunittest_safair.py)

Automated Test Platform(Mac Safari) parameters:

```python
        caps['name'] = 'Qinjin Jia's Resume'
        caps['build'] = '1.0'
        caps['browserName'] = 'Safari'
        caps['version'] = '11'
        caps['platform'] = ''
        caps['screenResolution'] = '1366x768'
```
**The automated test results(Mac Safari):** 
```
dhcp-wifi-8021x-155-41-104-88:Desktop Banyan$ python webunittest_safair.py
Loading Url
Maximizing window
Checking title
Done with session c1f20e48-40a6-4948-ac1d-1ce0a823535f
./anaconda3/lib/python3.6/unittest/suite.py:84: ResourceWarning: unclosed <socket.socket fd=8, family=AddressFamily.AF_INET, type=SocketKind.SOCK_STREAM, proto=6, laddr=('155.41.104.88', 62538), raddr=('104.20.76.153', 443)>
  return self.run(*args, **kwds)

----------------------------------------------------------------------
Ran 1 test in 6.576s

OK
```

|Check |Result |    
|---|---  
|Loading Url|Successful |
|Maximizing window |Successful |
|Checking title |Successful |


</br>


[Script for Web automated Test on Window 10 Chrome](https://github.com/qinjinjia/ec601_Unit_Test/blob/master/webunittest_chrome.py)

Automated Test Platform(Window 10 Chrome) parameters:

``` #python
        caps['name'] = 'Qinjin Jia's Resume'
        caps['build'] = '1.0'
        caps['browserName'] = 'Chrome'
        caps['version'] = '61x64'
        caps['platform'] = 'Windows 10'
        caps['screenResolution'] = '1366x768'
```
**The automated test results(Window 10 Chrome):** 
```
dhcp-wifi-8021x-155-41-104-88:Desktop Banyan$ python webunittest_chrome.py
Loading Url
Maximizing window
Checking title
Done with session 2feaa9ba-8fe4-4270-b29d-2943c3d6a5f6
./anaconda3/lib/python3.6/unittest/suite.py:84: ResourceWarning: unclosed <socket.socket fd=8, family=AddressFamily.AF_INET, type=SocketKind.SOCK_STREAM, proto=6, laddr=('155.41.104.88', 62345), raddr=('104.20.35.153', 443)>
  return self.run(*args, **kwds)

----------------------------------------------------------------------
Ran 1 test in 10.293s

OK
```

|Check |Result |    
|---|---  
|Loading Url|Successful |
|Maximizing window |Successful |
|Checking title |Successful |

## :full_moon:  **Task 2(Additional) - Automated Test for Android APP**
**Due to the APP developed in my HW2 is the Resume Website,**
**[CrossBrowserTesting](https://app.crossbrowsertesting.com/test-center) is used for the automated test of my developed WEB APP in HW2.**

However, **learning the automated test for Android APP with AWS application testing is also important. Therefore, an Android APP [app-release.apk](https://github.com/qinjinjia/ec601_Unit_Test/blob/master/app-release.apk) is forked from the repository [MyFirstAndroidApp](https://github.com/developerChenRui/MyFirstAndroidApp) of :girl: [developerChenRui](https://github.com/developerChenRui) with authorization. Thanks :tada:!**

**[AWS application testing](https://aws.amazon.com/device-farm/) is used for the automated test of the forked Android APP [app-release.apk](https://github.com/qinjinjia/ec601_Unit_Test/blob/master/app-release.apk).**

The automated test tests the **Android APP** on five different devices :point_down::

<img src="https://github.com/qinjinjia/ec601_Unit_Test/blob/master/Android%20APP%20AWS%20Unit%20Test%20devices%20list.png" width="600" height="180">

There are **three test suits** for each test :point_down::

<img src="https://github.com/qinjinjia/ec601_Unit_Test/blob/master/Android%20APP%20AWS%20Unit%20Test%20Suites%20and%20Results.png" width="600" height="180">
 
The **test video generated by AWS** is shwon in table below, 

|Device |Test Video |    
|---|---  
|Loading UrlAmazon Kindle Fire HDX 7 (2013)|[Amazon Kindle Fire HDX 7 (2013).mp4](https://github.com/qinjinjia/ec601_Unit_Test/blob/master/Test%20Videos%20Generated%20by%20AWS/Amazon%20Kindle%20Fire%20HDX%207%20(2013).mp4) |
|LG G Pad 7.0" (AT&T) |[LG G Pad 7.0" (AT&T).mp4](https://github.com/qinjinjia/ec601_Unit_Test/blob/master/Test%20Videos%20Generated%20by%20AWS/%20LG%20G%20Pad%207.0%22%20(AT%26T).mp4) |
|Samsung Galaxy S5 (T-Mobile) |[Samsung Galaxy S5 (T-Mobile).mp4](https://github.com/qinjinjia/ec601_Unit_Test/blob/master/Test%20Videos%20Generated%20by%20AWS/%20Samsung%20Galaxy%20S5%20(T-Mobile).mp4) |
|Samsung Galaxy S6 (Verizon) |[Samsung Galaxy S6 (Verizon).mp4](https://github.com/qinjinjia/ec601_Unit_Test/blob/master/Test%20Videos%20Generated%20by%20AWS/%20Samsung%20Galaxy%20S6%20(Verizon).mp4) |
|Samsung Galaxy Tab 4 10.1" (WiFi) |[Samsung Galaxy Tab 4 10.1" (WiFi).mp4](https://github.com/qinjinjia/ec601_Unit_Test/blob/master/Test%20Videos%20Generated%20by%20AWS/Samsung%20Galaxy%20Tab%204%2010.1%22%20(WiFi).mp4) |

In **Built-in Explorer Test Suite**, there are two events:

```
AppExplorer version: 9, Package: com.example.chenrui.myapplication, Launchable: com.example.chenrui.myapplication.MainActivity, Label: ZZApplicationLabel
1.	Activity com.example.chenrui.myapplication.MainActivity launched, COMMENT:[null]
2.	Tapping FrameLayout at (640,400), TOUCH:[640,400]
```

**Detailed Test results** for the **Built-in Explorer Test Suite**:
```
{"rootCause":"NO_FAILURE_DETECTED","isWifiConnected":true,"isLaunchScreenshotTaken":true,"isOpenGLApp":false,"unsuccessfulWatcherCount":0,"unvisitedComponentCount":0,"visitedComponentCount":1,"imageCount":0,"deviceFingerprint":"samsung\/matissewifiopenbnn\/matissewifiopenbnn:4.4.2\/KOT49H\/T530NUOVU1AOA2:user\/release-keys","ignoredComponentCount":0,"isLaunchSuccessful":true,"visitedScreenCount":1,"isExitDetected":false,"isCrashDetected":false,"totalTimeInMillis":31841,"isExitAfterSystemPopup":false,"visitedActivities":"[.MainActivity]","visitedActivityCount":1,"observation":"PASSED_BY_AVS","eventCount":2,"successfulWatcherCount":0,"securityThreat":"NO_ISSUE","sessionCount":1,"pid":11715,"securityStatus":{"totalOpenedSockets":0,"totalConnection":0,"totalOpenedPorts":0,"socketStats":[]},"isWebViewApp":false,"isExitAfterApplicationPopup":false,"isDropboxLogCollected":false,"isNonNativeViewApp":false,"isEntitlementPopup":false}
```
According to the detaield results, **there are no failure detected.**

|Test Suite |Result |    
|---|---  
|Setup Suite |Successful |
|Built-in Explorer Test Suite |Successful |
|Teardown |Successful |

<br/>

:sun_with_face: **Finally, thank you for watching :D)**:exclamation:

:trollface::trollface::trollface::trollface::trollface::trollface::trollface::trollface::trollface::trollface::trollface::trollface::trollface::trollface::trollface::trollface::trollface::trollface::trollface::trollface::trollface::trollface::trollface::trollface::trollface::trollface::trollface::trollface::trollface::trollface::trollface::trollface::trollface::trollface::trollface::trollface::trollface::trollface::trollface::trollface::trollface::trollface::trollface:
