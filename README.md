# RMX3371 OFP Guide
<div>
<p>This is a guide to move from Custom rom to RealmeUI using the ofp method.</p>
<br>
<p>First Download all the necessary files mentioned Below</p>
  <ul>
    <li><a href="https://github.com/yograjfire18/OppoRealme-OFP-Flash/releases/tag/1.0">Stock ROM flashing tool</li>
    <li>Firmware Links:
    <br>
    <ul>
      <li><a href="https://rms01.realme.net/sw/RMX3371export_11_A.04_2022080115370138.zip">Indian</a></li>
      <li><a href="https://rms01.realme.net/sw/RMX3371export_11_A.08_2022082316470137.zip">ID, TH, TW, PH, RU</a></li>
      <li><a href="https://rms01.realme.net/sw/RMX3371GDPR_11_A.08_2022082316480000.zip">Global</a></li>
    </ul>
    </li>
  </ul>
<p>Extract the stock rom flashing tool and the Firmware. Put the extracted firmware in the stock rom flashing tool folder as shown in the below image.</p>

<img src="assets/Screenshot 2024-04-29 125341.png">

<p>Now reboot to bootloader on your Smartphone, Connect it to pc and run the following command</p>

      fastboot devices

<p>If your device is connected, it would show something like the below image. If it isn't showing up, make sure  you properly install the adb drivers correctly.</p>

<img src="assets/Screenshot 2024-04-29 133839.png">

<p>After verifing the device is properly connected, Open the OPPORealme-OFP-Flash_1.0. Now Choose the option 0 and after the disclaimer choose option 1 as shown below in the image.</p>

<img src="assets/Screenshot 2024-04-29 134828.png">

<p>Wait for the flashing process to get finished(usually takes a long time so go and drink a cup of coffee during the flashing process.)</p>
<p>once the flashing is finished reboot to bootloader by the following below command or by pressing down power + volume down button</p>

    fastboot reboot bootloader
<p> now follow the following steps to complete the flashing process</p>
switchng to Slot a

    fastboot set_active a
<br>
rebooting to bootloader

    fastboot reboot bootloader
<br>
format

    fastboot -w
<br>
Time to reboot to RUI

    fastboot reboot

Congratulations! You have sucessfully Installed RealmeUI.
</div>
