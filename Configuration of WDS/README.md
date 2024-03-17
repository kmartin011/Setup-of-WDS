<h1>Configuration of WDS</h1>

<h2>Creation of a Hard Drive to House all Images</h2>
<p>It is a good idea to store all the images you may want to deploy to devices on one drive. I created a new drive on another machine that was already on my domain (WSUS-Client) to house all the images I needed. To do this I simply opened VMware and navigated to the settings of the VM and added a new 50GB Hard Drive.
<br>
<br>
I then went into the machine and opened disk manager by right clicking the windows button. Inside disk manager I took the disk online and then initialized it. I gave it a volume letter of W and called it WDS.</p>

![image](https://github.com/kmartin011/Setup-of-WDS/assets/148782985/8235bf87-4bad-4c70-9536-66b9ed82147e)

<h2>Configuration of WDS on Server</h2>

<p>Once I had configured my WSUS-Client machine with a new volume to host all my image files. I’d have to point to it so that WDS would know where to get the image files from. In order to get to do this, I simply opened server manager and right clicked my management server and opened DHCP manager. Inside here I expanded my DHCP scope and selected scope options, I then right clicked and selected configure options. In the scope options menu, I navigated to numbers 66 and 67 where I put the name of the WSUS-Client which holds all my image file and specified the bootfile name.
</p>

![image](https://github.com/kmartin011/Setup-of-WDS/assets/148782985/d631e2f6-afb0-490b-9289-3e99f073e0de)

![image](https://github.com/kmartin011/Setup-of-WDS/assets/148782985/ef1c3805-946b-4fba-8b37-cd168213cef5)




