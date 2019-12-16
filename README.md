# Crypto_Proj
Secure Human Trafficking Data Application

#IDE - Netbeans IDE 8.2

1. Configure Dropbox API to the JAVA APP
  - Go to https://www.dropbox.com/developers/apps/create
  - Choose DropBox API
  - Choose Full DropBox Access
  - Give some name to the app and click Create App
  - Scroll down to OAuth 2
  - Click generate on Generated access token and copy the generated access token
 2. Click HTD Data Share folder and click File_Enc_DB.java 
   - On line 42, paste the copied generated access token : private static final String ACCESS_TOKEN = "paste the generated access token         here within the quotes";
 3. Add all the dependencies. Go to Dependencies folder and add all the jar files.
 4. Add the three files. Go to Data folder and add the 3 data files under the same project file in Netbeans.
 5. First run File_Dec_DB.java as it acts as the server. 
 6. Then run the File_Enc_DB.java program as it acts as the client. Then select the human_data.txt file by choosing the "Select File"         option and click the Encrypt button. This will automatically encrypt the file,generate iv file and enc_dec_key file and store the         encrypted file in your DropBox folder.
 7. Then click the "Select File" option on File_Dec_DB.java (org XYZ) and choose the encryptedfile.txt file from your DropBox. Then click     the Decrypt button. This will automatically decrypt the encrypted file and store it on DropBox. 
 8. Now click the "Next" button of File_Enc_DB.java (org ABC). It acts as the server now.
 9. And then click the "Next" button of File_Dec_DB.java (org XYZ). It acts as the client now. 
10. Now click on "Common Data" button of org XYZ. This sends a request to org ABC.Then click on "Common Data" button of org ABC so             that it sends the common data information to org XYZ. 
 11. Now repeat the same for "Victim Count" by first clicking the Victim Count button of org XYZ and then clicking the Victim Count button      on the org ABC portal.
 12. Repeat the same for "Median Age". 
