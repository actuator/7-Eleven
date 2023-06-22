** 7-Eleven Bluetooth Smart Cup Jailbreak ** 



#  ![thumb](https://user-images.githubusercontent.com/78701239/236298562-adb7b1b2-4061-4501-b09f-b9f90c47b3e3.png)

https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2023-34761

In 2019 7-Eleven distributed a limited promotional item they generically named the 'Custom Message Cup’*.
* https://fccid.io/2AQNV-60961HC

Customers could personalize their cups with their own messages & slogans.

The cup consists of a plastic shell lined with an LED strip that communicates via BlueTooth Low Energy & allows users to send messages from their mobile device & is available for Android & iOs.

There is a word filter restriction on this promotional cup that displays filtered words using asterixis '*'.

![Capture](https://github.com/actuator/7-Eleven-Bluetooth-Smart-Cup-Jailbreak/assets/78701239/55b4e78e-755c-41b1-9e74-f2946e58b128)



Searching the source via JADX-GUI revealed the de-facto list of vulgar words & the regex word filter accomplished via  client-side filtering* so I proceeded to edit that wordlist. 


![pottymouth](https://user-images.githubusercontent.com/78701239/236337322-3666ac1d-a154-47a7-b8c2-e90a95548d2a.PNG)


APK Easy Tool was effective in providing a turn-key solution to decompile, sign & recompile the 'Hello Cup'(v1.3.1) Application.

The first step was to retrieve the Smali resource files that is essentially specialized assembly language code that is used to represent the Dalvik bytecode of Android applications & specific to the Android runtime environment.

![pogobad](https://user-images.githubusercontent.com/78701239/236341352-f93b04d0-090f-4bee-a6af-fb77140e3639.PNG)

Because I quit ‘Pokemon GO’ only the string 'pogo' will be restricted & everything else previously banned such as 'ugly' (really?) will no longer be filtered.

![APP-UI](https://user-images.githubusercontent.com/78701239/236963588-014a4e0c-9a1f-4ab4-a630-0f385805e8c9.gif)


As a result the message 'UGLY POGO STICK' previously rendered as '**** POGO STICK' will now display 'UGLY **** STICK'.

![LEDBLECUP](https://user-images.githubusercontent.com/78701239/236349091-86daaa0a-ba58-4dcf-902f-b9074ce6c887.gif)

Although modifying the application was trivial, it served as an interesting illustration bypassing client-side filtering.


** CWE-602: Client-Side Enforcement of Server-Side Security 

