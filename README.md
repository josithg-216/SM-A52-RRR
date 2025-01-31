# A52 Roms and Recovery Guide

## Points to  remember before coming out from stock rom 
### 1 . Knox Security will be tripped 
- Knox security will be tripped no matter what you do , you cannot undo it , 
- Consequences : Cannot use Knox based services ( Secure folder , Samsung Pay ) when returning to stock rom from a custom rom 
### 2 . Dev's Responsibilities
- developers are not responsible for ==Bricked devices and Dead SD cards== 
- developers will not be responsible for future problems that occur on the device
---

# Odin And Recovery 
### Recoveries 
- If you downloading a custom rom check whether there is recovery included with rom , if included use that , use the below mentioned recoveries only to install patches on Stock ROM or if the ROM does not come out with a recovery 
- [TWRP](https://twrp.me/samsung/samsunggalaxya52q.html)
- [OrangeFox](https://orangefox.download/device/a52q)
- If the recovery is in .img format , use the following command to convert it into .tar
```
  `tar --format=ustar -cvf Filename.tar Filename.img`
```
---
### Odin ( Flashing Recovery )
- Download Odin : [ODIN](https://odindownload.com/)
- Enable developer options and Enable OEM Unlocking inside it 
- Plug the phone to your pc
- Enter download mode and Unlock bootloader
- Rebbot 
- Open ODIN
- Enter download mode again
- Check the log whether the device is added in ODIN 
- Insert the recovery file in AP slot 
- insert [vbmeta_disabler](https://github.com/josithg-216/SM-A52-RRR/releases/tag/Vbmeta_disabler) in CSC slot 
- Disable auto reboot in Settings 
- Click on start 
- After the result is PASS , Move to recovery 
---

## List of custom roms 

### 1 [Lineage os](https://wiki.lineageos.org/devices/a52q/) 
- **Maintainer** : Simon1511
- **ROM Status** : Official + OTA
- **Stability** : Stable 
- **Android Version** : 15 QPR 1
- **UI** : Based on AOSP
- **Rom Version** : 22.1
- **Download links** : [LineageOS](https://download.lineageos.org/devices/a52q/builds)
- **Official Wikki** : [LOS A52 Wikki](https://wiki.lineageos.org/devices/a52q/install/#)
- **Source Code** : [Lineage Source](https://github.com/LineageOS)
- **Community support** : [Telegram](https://t.me/Lineageos_group)
- **Google Apps** : Not Included ( Can be installed , scroll down for details )
- **Known Bugs** : 
	1. **Does not pass integrity checks** 
		-  fails Play integrity and SafetyNet checks 
		-  Can be solved via patch , Scroll down for more details )
	2. **No VoLTE** 
		- VoLTE (Voice over Long-Term Evolution) wont work . In simple terms you will not be able to use internet when you are in a call  
		- This cannot be solved due to Samsung's proprietary implementation 
- [**Gerrit**](https://review.lineageos.org/q/status:open+-is:wip) 
- **Detailed XDA Post** : [XDA LOS A52](https://xdaforums.com/t/rom-15-0-encryption-official-lineageos-22-for-a52-4g.4712064/)
- **Maintainer's profiles** : Simon1511
	- [**XDA**](https://xdaforums.com/m/simon1511.7334446/)
	- [**Github**](https://github.com/Simon1511)
	- [**LOS Gerrit**](https://review.lineageos.org/q/owner:me@simon1511.de)
---

### 2 [Crdroid](https://xdaforums.com/t/crdroid-11-1-stable-android-15-qpr1-for-a52-4g-a52q-unofficial.4672356/)
- **Maintainer** : Testa Mic (Matei9) 
- **ROM Status** : Unofficial + OTA
- **Stability** : Stable 
- **Android Version** : 15 QPR 1
- **UI** : Based on AOSP UI
- **Rom Version** : 11.1
- **Download links** : [Crdroid](https://github.com/matei9/android_vendor_crDroidOTA/releases/tag/crdroid111stable)
- **Download Wikki** : [Crdroid A52 Wikki](https://xdaforums.com/t/crdroid-11-1-stable-android-15-qpr1-for-a52-4g-a52q-unofficial.4672356/)
- **Source Code** : [Crdroid Source](https://github.com/matei9/android_vendor_crDroidOTA)
- **Community support** : [Telegram](https://t.me/crDroidAndroid)
- **Google Apps** : Not Included ( Can be installed , scroll down for details )
- **Known Bugs** : 
	1. **Does not pass integrity checks** 
		-  fails Play integrity and SafetyNet checks 
		-  Can be solved via patch , Scroll down for more details )
	2. **No VoLTE** 
		- VoLTE (Voice over Long-Term Evolution) wont work . In simple terms you will not be able to use internet when you are in a call  
		- This cannot be solved due to Samsung's proprietary implementation 
- **Detailed XDA Post** : [XDA CrD A52](https://xdaforums.com/t/crdroid-11-1-stable-android-15-qpr1-for-a52-4g-a52q-unofficial.4672356/)
- **Maintainer's Profile** : Testa Mic
	- [**XDA**](https://xdaforums.com/m/testamic.12736440/)
	- [**Github**](https://github.com/matei9)
---

### 3 [Rising os](https://t.me/SamsunGalaxyA52/109055)
- **Maintainer** : RisenID (Ruchit Marathe)
- **ROM Status** : Unofficial
- **Stability** : Stable 
- **Android Version** : 15 
- **Rom Version** : 6.0
- **UI** : Based on AOSP UI
- **Download link** : [RisingOS](https://downloads.simon1511.de/s/ktrYHmpnp6Y6WFY)
- Google Apps :
	- Not Included in Vanilla build  ( Can be installed , scroll down for details )
	- Included in GAPPS build 
- **Known Bugs** : 
	1. **Does not pass integrity checks** 
		-  fails Play integrity and SafetyNet checks 
		-  Can be solved via patch , Scroll down for more details )
	2. **No VoLTE** 
		- VoLTE (Voice over Long-Term Evolution) wont work . In simple terms you will not be able to use internet when you are in a call  
		- This cannot be solved due to Samsung's proprietary implementation  
- **Maintainer's Profiles** : RisenID
	 - [XDA](https://xdaforums.com/m/risenid.12060347/)
	 - [Github](https://github.com/RisenID)
---

### 4 [UN1CA](https://www.google.com/url?sa=t&source=web&cd=&ved=2ahUKEwimuuDSlZ6LAxVsRmcHHfrBIIYQFnoECAkQAQ&url=https%3A%2F%2Fgithub.com%2Fsalvogiangri%2FUN1CA&usg=AOvVaw3FP9q9uWlAmds0YocaD9G3&opi=89978449)
- **Maintainer** : Salvogiangri ( Salvo Giangreco )
- **ROM Status** : Official 
- **Stability** : Stable 
- **Android Version** : 14 
- **Rom  Version** : 2.5.4
- **UI** : Based on One UI
- **Download link** : [UN1CA](https://github.com/salvogiangri/UN1CA/releases/tag/2.5.4) 
- **Source Code** : [UN1CA Source](https://github.com/salvogiangri/UN1CA)
- **Community support** : [Telegram](https://t.me/unicarom)
- Google Apps : Included
-  **Known Bugs** : 
	1. Does not pass integrity checks 
		-  fails Play integrity and SafetyNet checks 
		-  Can be solved via patch , Scroll down for more details )
- **Maintainer's Profiles**
	- [Github](https://github.com/salvogiangri)
---


### 5 [Pixel OS](https://github.com/PixelOS-AOSP)
- **Maintainer** : koko-07
- **ROM Status** : Unofficial
- **Stability** : Stable 
- **Android Version** : 15 
- **Rom Version** : 15
- **UI** : Based on AOSP UI
- **Rom's Detailed XDA Post** : [XDA Pixel OS](https://xdaforums.com/t/rom-15-unofficial-pixelos-for-galaxy-a52-4g-stable.4702572/#post-89803350)
- **Download Link** : [PixelOS Download](https://sourceforge.net/projects/pixelos-a52/files/A52/)
- **Source Code** : [PixelOS Source](http://github.com/PixelOS-AOSP)
- **Community Support** : [Telegram](https://t.me/posa52qq)
- **Google Apps** : Included
-  **Known Bugs** :
	1. No VoLTE 
		- VoLTE (Voice over Long-Term Evolution)  wont work . In simple terms you will not be able to use internet when you are in a call  
		- This cannot be solved due to Samsung's proprietary implementation 
- Maintainer's Profile : KoKo-07
	- [XDA](https://xdaforums.com/m/koko-07.12900040/) 
	- [Github](https://github.com/koko-07870)
---

### 6 [Evolution x](https://xdaforums.com/t/rom-15-0-0_r10-unofficial-evolution-x-10-2-01-29-25.4705163/)
- **Maintainer** : Chuqol
- **ROM Status** : Unofficial 
- **Stability** : Stable 
- **Android Version** : 15 
- **Rom Version** : 10.2
- **UI** : Based on AOSP UI
- **Download** : [EvoX Download](https://sourceforge.net/projects/evolution-x-a52q/files/)
- **Source Code:** : [EvoX Source](https://github.com/Evolution-X/)
- **Community Support** : [Telegram](https://github.com/Evolution-X/)
- **Rom's Detailed XDA Post and Wikki** :[EvoX XDA](https://xdaforums.com/t/rom-15-0-0_r10-unofficial-evolution-x-10-2-01-29-25.4705163/)
- **Google Apps** :  Included
- Maintainer's Profile : joeyhuab and AnierinB
	 -  [XDA](https://xdaforums.com/m/chuqol.12753012/)
