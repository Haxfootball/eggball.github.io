# Instructions on how to Auto-Upload Tagpro Replays to Cloud.

**Prerequisites:**
You must download Tampermonkey add-on for your browser first.


**Scripts**
There are two scripts needed to upload your replays.

1. Tagpro Analytics updated script: https://res.cloudinary.com/eggball/raw/upload/v1613667826/scripts/TagPro_Analytics_Egg.user.js
2. Tagpro VCR updated script: https://res.cloudinary.com/eggball/raw/upload/v1613667826/scripts/TagPro_VCR_Eggball.user.js

The analytics script was updated so the match ID is saved off. The VCR script was updated to save off the replay and upload it to cloudinary with the ID of the Match ID from Analytics site.

**Important:** You should turn off your current tagpro analytics script and VCR script so you're not duplicating scripts doing the same thing. I renamed the scripts so they will not override your current scipts when downloaded. The analytics script and VCR will continue to behave the same way as before, but were just enhanced/updated. You also need to ensure that the Tagpro Analytics script has a higher priority (lower #) than the VCR script. This way the Analytics script can send the match ID correctly to the VCR script. This should be the default behavior if the scripts are downloaded in the correct order.
![Sample Tampermonkey Order](Tampermonkey.png)
