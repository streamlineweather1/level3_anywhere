<header>
</header>

## Introducing Level3_Anywhere

The level3_anywhere software package provides a python-based application to convert level3 radar products from an original Radar Product Generator (RPG) radar site to any other valid RPG radar site. This application is designed to allow for a more robust case study archive for training of meteorologists within software that decodes level3 radar data, such as the Advanced Weather Interactive Processing System (AWIPS). With level3_anywhere, past significant weather event from anywhere within the NEXRAD network can be remapped and displayed to the radar and corresponding geographic region of the user's choosing.<br>

The software can handle automatic processing of everything from one single level 3 product file to hundreds or thousands of files that would constitute an entire weather event worth of level 3 files. All level 3 products and product identifiers are supported with the current software release.<br>

Below we see a screenshot of data from the KBMX radar (NWS Birmingham, AL) from April 11th, 2011 remapped to the KTBW radar (NWS Tampa Bay Area). In this instance, the Tuscaloosa EF-4 tornado event is now impacting the coastline of Pinelles County, Florida.<br><br>

<center><img src="images/bmx2tbw-1.png" alt="KBMX Remapped to KTBW" width="500" height="400">
<b>April 27th, 2011 Tuscaloosa to Birmingham Tornado - KBMX (Birmingham, AL) mapped to KTBW (Ruskin,FL)</b></center></center>

<!--![screenshot](images/bmx2tbw-1.png)-->

## How to Use

These python scripts are designed to be run via the command line. 

1) Place the scripts in a master directory of your chooseing. For this example the master directory will be <b>/home/bryan/Convert_Level3/</b><br>
2) Place the original level 3 radar files in a directory called "data" within the master directory. For this example <b>/home/bryan/Convert_Level3/data</b>.<br>
3) For the script <b> convert_level3.py </b> in which only the data RPG station is being changed and not the dates of the data, the command line structure is as follows:<br>

python convert_level3.py <old_station_id <new_station_id> <master path> <product string>" <br><br>
"product string" can be any valid level3 product Identifier (for example N0Q). In this case, all files in the /data/ directory containing the string "N0Q" will be converted to the new station id. If the string "all" is used for the product string, all files within the /data/ directory will be converted.<br><br>

<b>python convert_level3.py BMX TBW /home/bryan/Convert_Level3/data/ all</b><br>
- All files in the data directory from the BMX (Birmingham, AL) radar site will be converted to be from the TBW (Ruskin, FL) radar site. <br><br>

print("or...")
print("BMX TBW /home/bryan/Convert_Level3/data/ NQ0")

<hr style="width:50%;text-align:left;margin-left:0">

## Installation
No installation is required for this web application. Simply access the WeatherSense through your web browser from the link --link--

<hr style="width:50%;text-align:left;margin-left:0">

## Contributions
Contributions to Level2_Anywhere project are welcome. If you find any issues or have suggestions for improvements, please feel free to submit a pull request or open an issue in the GitHub repository.

<hr style="width:50%;text-align:left;margin-left:0">

## License
Level3_Anywhere is created by Bryan Mroczka of Streamline Weather Consulting, LLC. Users are free to use, modify, and distribute the code in accordance with the terms of the license.

<hr style="width:50%;text-align:left;margin-left:0">

## Acknowledgements

<hr style="width:50%;text-align:left;margin-left:0">

## Additional Remapping Examples - AWIPS2 Screenshots

<center><img src="images/KTLH2KBOX-1.png" alt="KTLH Remapped to KBOX" width="500" height="400">
<b>October 10th, 2018 Hurricane Micheal - KTLH (Tallahassee, FL) mapped to KBOX (Boston, MA)</center></b><br>

<br>

<center><img src="images/lck2tbw-1.png" alt="KLCK Remapped to KTBW" width="500" height="400">
<b>April 27th, 2014 Mayflower Arkansas long track EF-4 Tornado - KLZK (Little Rock, AR) mapped to KTBW (Ruskin, FL)<br>
</center></b>

<br>

<center><img src="images/sgf2okx-1.png" alt="KSGF Remapped to KOKX" width="500" height="400">
<b>KSGF (Springfield, MO) mapped to KOKX (Upton, NY)<br> at 7:55 PM EDT July 4th, 2019<br>
(Directly over Midtown Manhattan)</center></b><br>

<br>

<center><img src="images/ohx2fws-1.png" alt="KOHX Remapped to KFWS" width="500" height="300">
<b>May 1 - 2, 2010 Nashville Flash Flooding Event - KOHX (Nashville, TN) mapped to KFWS (Fort Worth, TX)<br>Date/Time Changed at 12:00AM New Years Eve 2020</center></b><br>

<br>

<center><img src="images/tbw2eax-1.png" alt="KTBW Remapped to KEAX" width="500" height="400">
<b>October 18th, 2019 Polk County, Florida EF-2 long track tornado - KTBW (Ruskin, FL) remapped to KEAX (Kansas City, MO) radar
</center></b>>br>


## Final Thoughts


<footer>

<!--
  <<< Author notes: Footer >>>
  Add a link to get support, GitHub status page, code of conduct, license link.
-->

</footer>
