# Sennheiser-G4-Scan-Converter
Made to be used with Google Sheets/Appscript & RF Explorer/Touchstone Pro Scans, to convert and format CSV's to Sennheiser WSM format

Link to my own sheet for usage:[Wireless Frequency Range Document - RF Explorer CSV to Sennheiser WSM CSV](https://docs.google.com/spreadsheets/d/1J3ns_adF1a7abeK9_Y9u7mm-bNHIiVYPU-pPMlAzFLo/edit?usp=sharing)

Largely inspired by this video: [Loading RF Scans ingo IAS, WWB6 and WSM - PeterErskine](https://www.youtube.com/watch?v=sivL8lQQKws&ab_channel=PeteErskine)
And people from this thread: [ProSoundWeb Community - RF Explorer to WSM](https://forums.prosoundweb.com/index.php?topic=163644.0)

## How to set up the .gs Appscript File on Google Sheets:
1. Open [My Sheet](https://docs.google.com/spreadsheets/d/1J3ns_adF1a7abeK9_Y9u7mm-bNHIiVYPU-pPMlAzFLo/edit?usp=sharing) and go to `File -> Make a Copy`

<img width="374" alt="image" src="https://github.com/user-attachments/assets/91c4075b-63d2-4274-bb86-5d302597476c">

2. In your new copy of this file: go to `Extensions -> Appscript` and on the left-hand side of the new window click the `Triggers` alarm icon.

![image](https://github.com/user-attachments/assets/786ea415-521f-46d4-9cf7-c6b59cde2cc7) ![image](https://github.com/user-attachments/assets/1a28cc16-03f8-4262-871b-876d4a447a5b)

3. In the bottom right, click `Add Trigger` and select the `onOpen` Function to run `On Open`, then click Save.

<img width="724" alt="image" src="https://github.com/user-attachments/assets/dc100588-5454-48b6-bdac-7e51ea190ce6">

4. Then, authorize the code to run from your account: LOOK THROUGH THE CODE FIRST BEFORE AUTHORIZING ANYTHING ON YOUR ACCOUNT!!!

5. Refresh the sheet, and see that the new menu dialog next to `Help`, `Create Sennheiser WSM File` has popped up

## How to use the sheet

1. Export your Touchstone Pro scan to `.csv` format

2. In the `RF Explorer Paste` tab, go to `File -> Import` and upload your CSV. Select `Replace Current Sheet` and then click `Import Data`

<img width="460" alt="image" src="https://github.com/user-attachments/assets/79fe66eb-e824-4469-85d9-7c2dd456ba2f">

Your Replaced sheet should look like this:

<img width="791" alt="image" src="https://github.com/user-attachments/assets/b041d6da-ec70-496b-a6a9-f3fb6d84af47">

3. Go to the `Create Sennheiser WSM File` Menu and select `Download Sennheiser WSM CSV`

4. When the dialog box appears with the download link, click it and download the file. That's your converted scan data!

## Notes:

I've provided an example Touchstone Pro Scan + a Sennheiser converted scan that works in my software in case you want to see the formatting for yourself or compare it to previous iterations.

The biggest note is that the Sennheiser file uses `;` instead of `,` for cell separation, and the Sennheiser data expects a scan % in between the Frequency and RF level 

I've also provided the .gs code in this file if you want to look at it yourself in a code editor



