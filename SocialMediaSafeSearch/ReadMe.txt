About Social Media SafeSearch Bot:

This is an unattended bot which will search the Input folder for images of JPG or PNG format , and create the list of file paths in the output excel file.
The bot then utilizes the Google vision API activities to use the safe search feature to get the likelihood of Adult, Violent, Racy or Medical Content and then updates the results in the output excel file. 
Then the Administrator can then use the output file to moderate the Images.

Pre Requiste:

1. UiPath Studio is installed with Packages :Uipath.Credentails.Activities , UiPath.GoogleVision.Activities & UiPath.Excel.Activities
2. Input Folder with few images of JPG or PNG format. (after each run do this)
3. Output Folder with a Excel file called "ImageDetails.xlsx" (with these columns : ImagePath |	Adult |	Violence |Racy |Medical )
4. Enable Google Vision API in Google developers cloud portal 
5. Google Vision API authetication: Google Client ID and Google Secret Key (need to update the same in the Windows credential manager)
6. Microsoft Excel application.
7. Update config.xlsx with input , output file paths and Credenitial name.
8. Open the SafeSearch.xaml and update the variable strOutputFile as per the config.xlsx

