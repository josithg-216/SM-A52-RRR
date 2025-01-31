# A52 Roms and Recovery Guide

## Points to  remember before coming out from stock rom 
### 1 . Knox Security will be tripped 
- Knox security will be tripped no matter what you do , you cannot undo it , 
- Consequences : Cannot use Knox based services ( Secure folder , Samsung Pay ) when returning to stock rom from a custom rom 
### 2 . Dev's Responsibilities
- developers are not responsible for Bricked devices or Dead SD cards 
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

# List of custom roms 

### 1 [Lineage os](https://wiki.lineageos.org/devices/a52q/) 
- **Maintainer** : Simon1511
- **ROM Status** : Official + OTA
- **Stability** : Stable 
- **Android Version** : 15 QPR 1
- **UI** : Based on AOSP
- **Rom Version** : 22.1
- **Download links** : [LineageOS](https://download.lineageos.org/devices/a52q/builds)
- **Official Wiki** : [LOS A52 wiki](https://wiki.lineageos.org/devices/a52q/install/#)
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
- **Download Wiki** : [Crdroid A52 wiki](https://xdaforums.com/t/crdroid-11-1-stable-android-15-qpr1-for-a52-4g-a52q-unofficial.4672356/)
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
 - [**Telegram DM**](@testamic2)
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


### 5 [PixelOS](https://github.com/PixelOS-AOSP)
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

### 6 [EvolutionX](https://xdaforums.com/t/rom-15-0-0_r10-unofficial-evolution-x-10-2-01-29-25.4705163/)
- **Maintainer** : Chuqol
- **ROM Status** : Unofficial 
- **Stability** : Stable 
- **Android Version** : 15 
- **Rom Version** : 10.2
- **UI** : Based on AOSP UI
- **Download** : [EvoX Download](https://sourceforge.net/projects/evolution-x-a52q/files/)
- **Source Code:** : [EvoX Source](https://github.com/Evolution-X/)
- **Community Support** : [Telegram](https://github.com/Evolution-X/)
- **Rom's Detailed XDA Post and wiki** :[EvoX XDA](https://xdaforums.com/t/rom-15-0-0_r10-unofficial-evolution-x-10-2-01-29-25.4705163/)
- **Google Apps** :  Included
- Maintainer's Profile : joeyhuab and AnierinB
	 -  [XDA](https://xdaforums.com/m/chuqol.12753012/)
---
# Donate to Devs 
- Please cross check / Double check the devs Paypal name before donating (there is a chance of you misclicking the link)
- Lineage os [Simon1511](https://www.paypal.com/paypalme/SimonS1511)
- Crdroid [TestaMic](https://www.paypal.com/paypalme/FilipCojocaru)
- UN1CA (Check his [Github](https://github.com/sponsors/salvogiangri) Sponsor page )
- EvolutionX [Chuqol Dev](https://www.paypal.com/donate/?hosted_button_id=66X29XLEZKPH6)
---

# CheckSums 

- **LineageOS** (SHA256)
```
ba6ad0bc5fe78f349bbe211f0e1022939a39155fb4798b9a3cd43bc2419b1149
```

- Crdroid (SHA256)
```
e6047f3b495b8a58ee163a657e8e35935cd57c2719d972e1d1d448cf6910925d
```

- UN1CA (SHA1)
```
e114f9e498cfc55c4eb1fd1cae69ae74
```
---

# Kernel 

## Ascendia Kernel 
- Developer and Maintainer : RisenID ( Ruchit Marathe )
- Ascendia isn't compatible with A15 as of now wait until developers release a patch 
- Source code : [Ascendia Source](https://github.com/RisenID/kernel_samsung_ascendia_sm7125)
- Kernel Support - 
	 [Telegram](https://t.me/AscendiaChat)
---
# Rooting 
## Magisk 
- Download [Magisk](https://github.com/topjohnwu/Magisk/releases/tag/v28.1)
- Rename .Apk as .Zip
- Enter the recovery and flash Magisk,zip
- installation along with Rom is recommended
- After installing Magisk via Recovery , Reboot the device. 
- Open Magisk App
- Patch the app with (recommended method)
- Reboot again 
- Check the root status with root checker app 

## KernelISU
- Installation of kernelISU is always recommended only with ascendia kernel 
- Wait for Android 15 Ascendia patch
---

# Patch for Rooted devices
- Rooted devices can install patches like Knox Parch and Integrity fix patch

## Knox Patch for Stock Rom 
- **Developer** : Salvogiangri ( Salvo Giangreco )
- **Requirements** : Magisk or KerenelISU
- **Patch Link** : [Knox Patch](https://github.com/salvogiangri/KnoxPatch)

## Play integrity fix :
- **Developer** : chiteroman
- **Requirements** : Magisk or KerenelISU
- **Patch Link** : [Integrity Fix](https://github.com/chiteroman/PlayIntegrityFix/releases/tag/v18.5)
---

# Google Apps 
- Dont Install Google Apps if it is already included in build 
- If GApps are not included , follow the steps below 
- [MindTheGapps](https://wiki.lineageos.org/gapps/)
- [NiksGapps](https://nikgapps.com/downloads)
- download any one of gapps and flash it via recovery

# Reinstall Stock Rom ( One ui )
- Discontinued
- Donwload the stock rom from [SAMFW](https://samfw.com/firmware/SM-A525F)
- Enter download mode and open odin in your pc
- extract the downloaded rom
- Disable auto reboot in settings (odin)
- Place the files in respective Odin slot and fash
---

# One UI Debloat 
- Download [UniveralAndroidDebloater]() 
- Enable USB debugging from Developer options
- Plug the phone into the pc 
- Open UAD_GUI
- Select the files according to this [PDF](https://github.com/josithg-216/SM-A52-RRR/releases/tag/OneUI-Debloat)
- After selecting them , Delete them
---
# Device Support Group 
- [Telegram Device Group](https://t.me/SamsunGalaxyA52)
- [SubReddit](https://www.reddit.com/r/GalaxyA52/)
---

# Thanks Giving
- Thank you all the developers who are working hard to take our device experience to the next level , You will be remembered , Thank YOU , Love You 3000 :3
---

# Note 
- This repo will be actively maintained , Changes will be done 3 days once , Anyone is welcomed to make changes
---

# Big Thanks to Samsung Developers and Modding Community 
---
