<p align="center">
<img src="https://github.com/NeuralOS/extraUI/blob/master/neural_logo.jpg" > 
</p>

NeuralOS
===========
NeuralOS is a custom ROM (Operating System) from AOSP source which supports Qualcomm devices.

Thanks to
-------
* [**AEX**](https://github.com/AospExtended)
* [**TeamSubstratum (Theme Engine)**](https://github.com/Substratum)
* [**LineageOS/Cyanogenmod**](https://github.com/LineageOS)


How to Build?
-------------

To initialize your local repository using the NeuralOS trees, use a 
command like this:

```bash
  repo init -u git://github.com/NeuralOS/manifest.git -b pie9.0
```
  
Then to sync up:
----------------

```bash
  repo sync -c -jx --force-sync --no-clone-bundle --no-tags
```
Finally to build:
-----------------

```bash
  . build/envsetup.sh
  lunch aosp_device_codename-userdebug
  mka aex -jx
```
