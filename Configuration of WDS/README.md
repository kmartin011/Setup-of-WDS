<h1>Configuration of WDS</h1>
<p>
  Now that most of the pre-configuration have been done, we can start the setup of WDS.  This will be done on the WSUS-Client server. 
</p>

![image](https://github.com/kmartin011/Setup-of-WDS/assets/148782985/4e6a7d1f-07f6-4abf-ac3e-57fbc0dd5621)

<p>
  First, I opened windows manager again and navigated to WDS tab on the left column, this brings up the WDS Window. Here, I right clicked my server in the left column and selected Configure Server. All the requirements listed above has already been done. I left the option Integrated with Active Directory selected and went to the next page. 
  <br>
  <br>
  For the path of the remote installation folder I made sure to target the new drive that I made (w drive). 
</p>

![image](https://github.com/kmartin011/Setup-of-WDS/assets/148782985/932d6a16-c6b3-421d-99fb-865aca6f77e7)

<p>
  On the next page I selected “Respond to all client computers (known and unknown). 
  <br>
  This may not be the most secure way to deploy this on a real LAN but I selected this one to help with the demo. I then clicked next and finished the installation.
<br>
<br>
  Once I completed the wizard the folders listed below were automatically created including the Images folder. 
</p>

![image](https://github.com/kmartin011/Setup-of-WDS/assets/148782985/a6c770c0-c355-4d85-b13b-0be6a805d9ca) ![image](https://github.com/kmartin011/Setup-of-WDS/assets/148782985/33cabfbc-0323-4ddd-869a-4dc72abfcfa7)

<p>
  While inside the WDS manager still, I right clicked the install images tab on the left and selected Add New Image, I gave the image group a name “NETW2500KM-Image”. Next I selected the location for the image file. Since I had already had the DVD mounted to the VM, I just navigated to the D drive\sources folder and selected the install.wim file and went to the next page. For the next two pages I left them at default and then finished the installation
  <br>
  <br>
  Below shows an image of the images created
</p>

![image](https://github.com/kmartin011/Setup-of-WDS/assets/148782985/ec772cb3-a82b-4cef-86e4-080bcbd7ce90)

<p>
  Next, I will setup the boot image which is very similar to the previous step. I just right clicked boot images and selected add new boot image. I navigated to the D drive again, sources folder and then selected boot.wim. I left the next pages as default and then finished the wizard.
</p>

![image](https://github.com/kmartin011/Setup-of-WDS/assets/148782985/812946bb-a531-4e9e-9437-8cf54463420c)


