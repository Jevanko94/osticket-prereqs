# osticket-prereqs
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>
<p align="center">
</p>
<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />

⬇️⬇️⬇️⬇️⬇️Use this link to download the files⬇️⬇️⬇️⬇️⬇️

[https://drive.google.com/drive/folders/1gX3eCEKAB4RzKLbkAimJi77gjwS_nxl7?usp=sharing](https://drive.google.com/drive/folders/1QsdJJuqcprgYi2suTphGXoL2K_5SYfOD?usp=sharing)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- OsTicket 

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- HeidiSQL
- MySQL
- OsTicket
- PHP Manager
- php
- Rewrite
- VC_redist

<h2>Installation Steps</h2>

<p>
<img src="https://github.com/user-attachments/assets/852c18a9-97c4-47e1-a362-35f44827d5a6"
"/>

</p>
<p>
First go to Microsoft Azure and type Resource Group then click create Resource Group
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/1ac3d8e4-f111-4437-af18-a24fae32d245"


</p>
<p>
Now type RG-osticket for the name of the Resource Group. Next for the region click US West US 3 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/908e6477-2127-4ad6-ab35-02720fe79ef4"
>
</p>
<p>
Now go to the review and create tab and click the create button on the bottom left 

<br />

<p>
<img src="https://github.com/user-attachments/assets/c7c818d6-e857-45f4-a14c-dad56b835daf"
/>
</p>
<p>
Now type Virtual Machines and click create azure virtual machine 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/b87c70ed-73cf-4755-b68b-5220ad4b5e18"
>
</p>
<p>
Now select the resource group we created RG-osticket then the virtual machine name type VM-osticket and the region select the same as the resource group US West US 3 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/30576e32-2682-425f-9744-b83216eedb0c"
/>
</p>
<p>
Now for the image select windows 10 pro version. For the size select standard Ec2 and the username type labuser and the password type a unique password remember to copy all this down on a notepad or physical paper
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/1cb48017-58fd-4a1f-9f35-2fd564d440c8"
</p>
<p>
Next click the licensing box and then click review and create 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/d174ecdd-dab6-45fe-9154-056c7452bb36"
"/>
</p>
<p>
Now go to the networking tab and make sure virtual network, subnet, and public ip all says (new)
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/13d3f8eb-2045-4ad7-b82a-74d7a27e0e46"
</p>
<p>
Next create the virtual machine and you will see the deployment process start 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/903b06ff-d235-407e-9ebc-a36f816ab203"

</p>
<p>
Now the process will be done when you see a green check mark 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/5e09d0d2-6aee-4193-830f-03c6f084a434"
</p>
<p>
Next go back to the virtual machine home page and click VM-osticket then copy the public IP address
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/da4e988f-edd9-4e75-b9b9-dfda7be1863c"

</p>
<p>
Next type Remote Desktop Connection in the search bar of your PC then click to open the app
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/ac9d27fe-a6a9-4357-8e77-adc59c62197c"

</p>
<p>
Paste the public IP of VM-osticket into the computer section then click connect 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/11baecda-4d2c-4ddd-b4ca-b7bb9ba6faf6"

</p>
<p>
<img src="https://github.com/user-attachments/assets/1615831f-175b-4f34-aa95-0e7a34370e90"

</p>
<p>
now for the user name type labuser and the password type the password you made for the VM
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/cd3ddadc-3f2a-4b09-ab92-1ce471cb827e"

</p>
<p>
Next click yes to connect to the VM
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/e9a6e64c-d61f-474d-a47d-115465441e91"

</p>
<p>
Now you will see the virtual machine log into labuser load
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/8627795d-fed5-426e-b03c-6f277f057a2b"

</p>
<p>
Now click no for all the following in the image above 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/1d2463e0-161b-4c8b-b8e3-e0b920f3aa62"

</p>
<p>
Now once the networks tab shows on the right side of the screen then click yes 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/8295cc9a-2a58-408c-9d9d-ed0b46dc85c2"

</p>
<p>
Next right click the windows icon on the bottom left then click run 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/34bee8a0-0c0d-4673-a61f-c29340d85aa2"

</p>
<p>
Now type control type then click ok 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/b08f8401-1a45-480c-8127-a02b244536ef"

</p>
<p>
Now click programs 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/e8a19e10-7e18-4480-abaf-5befb2e219e8"

</p>
<p>
Click programs and features
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/5d7673ea-ebb5-4923-a79a-728d80e99a55"

</p>
<p>
Now click Internet Information Services
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/a1a650ac-9207-44ed-bc29-17aa638c2b09"

</p>
<p>
Now click world wide web services 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/7768cd38-c86e-4873-b2e0-d602a0eb457b"

</p>
<p>
Next click application development features 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/4ae64bf1-344e-45fb-aa7a-62e625fb5658"

</p>
<p>
Next click the box for CGI
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/f85ae36a-8bcf-404b-ab87-1d9211ad8ad9"

</p>
<p>
Next click Common HTTP Features 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/61f39e95-d469-4b99-9e15-317a1a0ec36b"

</p>
<p>
Now in Common HTTP Features click the box for everything then click ok 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/e552ed95-ff6b-4877-b951-ebb208dc8fd5"

</p>
<p>
Then you will see a loading screen process 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/f04be8e7-42cb-44f8-899b-2461bb6a6e19"

</p>
<p>
Now open up microsoft excel and click start without your data
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/ba514572-b3ab-4a29-b7b4-ea49cd4e3e4e"

</p>
<p>
Now click continue without this data 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/aff772c1-5a7e-43fd-b698-b2d5912687c4"

</p>
<p>
Next click confirm and continue 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/4f9860cd-07b9-41fb-a466-4275912a0eb9"

</p>
<p>
Finally click continue and start browsing 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/3205cdfd-5153-4bb6-a61e-32d3dfef208a"

</p>
<p>
Next once the process is complete click close 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/6fa29fc6-2b80-456c-a0b1-d3f5faa7872c"

</p>
<p>
Now in order to see if the process worked type 127.0.0.1 in the search bar and you will see the same image above 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/e9b04296-755a-4a8e-b716-e4b855003ca6"

</p>
<p>
Next open the link and download PHP Manager for IIS click the download symbol on the side
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/0a927830-6fed-401d-bcdc-a3bb7832a064"

</p>
<p>
Now open up file explorer and go to your downloads folder then double click PHP manager 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/13e81914-3ac0-4cb7-b91c-160db689970b"

</p>
<p>
Next click next 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/47c4971e-d1ae-4aa6-9888-3850bf7fb1c6"

</p>
<p>
Next click I agree and then next 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/e66be1dd-303d-4c62-8bdd-8ad98c1bf282"

</p>
<p>
Finally click close 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/a1cf2e60-62fc-49d2-a2d9-0a237eac8d31"

</p>
<p>
Next go back to the link and download Rewrite Module click the download symbol 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/e87d9886-8850-420a-9174-baeaa8fdaaad"

</p>
<p>
Go back to file explorer and double click rewrite 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/57d78570-7d95-4e62-b4d6-7728c1adc426"

</p>
<p>
Click I accept then install 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/630e708c-b68e-49ce-b4b1-3c0f7174b8af"

</p>
<p>
Now let the process start 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/e9f80eb9-b42f-4566-b99f-451c5d96f024"

</p>
<p>
Next click finish
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/e48fefc2-ea41-4283-9b62-40202e942ad4"

</p>
<p>
Next go back to the link and download PHP 7.3.8 click the download symbol 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/f13feed3-7989-4272-ad07-4c3ebe722c89"

</p>
<p>
Go back to file explorer and you will see the file in the download folder 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/8affe2fc-2254-4175-a6cd-cc35647aba7e"

</p>
<p>
Now click on Windows (C) 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/3e23a414-971c-40e4-8f8d-79fa6690e714"

</p>
<p>
From here right click anywhere and click new then select folder 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/a39f6b85-7839-434f-962e-d900d45bb94a"

</p>
<p>
Now name the folder PHP
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/1f1870ef-6320-42ee-82b1-29b0a26c93c8"

</p>
<p>
Go back to the download folder and right click php folder then click Extract All
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/c6c7b659-0e65-4ba0-9aa6-c886a5b54c07"

</p>
<p>
Now click browse 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/09232923-94c0-4036-b3a9-db4161b89422"

</p>
<p>
Next go to Windows (C) then click the PHP folder we created 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/a43aa800-1e94-40ca-8d94-3e1fa885ea7c"

</p>
<p>
Now once you are in the folder click select folder on the bottom right 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/30fdb415-a37e-49cd-8ffa-aa028c95f681"

</p>
<p>
Now click the extract button
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/eee805ad-8ebd-492f-b5b7-a46041b60a4d"

</p>
<p>
Next you will see all the files load into the PHP folder
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/11b448f5-61f5-434b-ae25-5569053ce89f"

</p>
<p>
Next go to the link and click the link to download VC RedistX86.exe click the download symbol
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/89a6cc21-b93d-4357-a5b5-08da1fc2d841"

</p>
<p>
Now go to file explorer and double click VC_redist 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/e80fb105-d2e6-497f-b7fe-49917692a27a"

</p>
<p>
Click Install 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/2eefe59a-5b36-4183-8225-4dbf00d8b8fe"

</p>
<p>
Now once the process is done click close 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/53d6477e-c4dd-4758-91e0-e6f10f3fb91f"

</p>
<p>
Next click the link an download MySQL 5.5.62 then click the download symbol 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/1b4b9c08-c735-45a9-bd53-6fbab82af471"

</p>
<p>
Now go to file explorer and double click mysql to open the program 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/b0d368cc-7d4d-459b-be70-6952a9e5c8f6"

</p>
<p>
Next click next 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/6c03d529-fec4-4e4b-90ae-3a1cdc9d33e1"

</p>
<p>
Next click next 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/bee12d5d-c816-4223-96da-ccab48c6f581"

</p>
<p>
Now click Typical 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/b0f6b18c-dec2-4d11-8b1e-7adf9aeb5106"

</p>
<p>
Next click install 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/0a84ed5e-bf37-4ef3-a5be-26f1f587d1d2"

</p>
<p>
Now click finish 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/8c142cb4-9fc9-4ca9-8dc7-87fc1c5ca299"

</p>
<p>
Now click next 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/633eb983-1a7f-4992-b681-4b05595e51f0"

</p>
<p>
Now click Standard Configuration then click next 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/150edba2-70f2-428b-a179-41c748614dfa"

</p>
<p>
Now click Install as Windows Service then click next 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/a2ed5cc2-5e4b-455c-ac95-4e8c747a1538"

</p>
<p>
Now type the password. For this example I'm going to type Password1 then click next 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/122b4182-c94f-4099-aff9-91e4f4e5c4a8"

</p>
<p>
Next click execute to finish the process
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/4ccb3942-2f6a-439d-8ab1-ec529f5667af"

</p>
<p>
You will then see the process finish 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/57a6f66c-f0cc-45bd-89e6-07bfbe87a146"

</p>
<p>
Now type IIS or Internet Information Services then right click then click run as administrator 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/44515fe1-c7ee-4dcd-9865-c65f3e0e374b"

</p>
<p>
Now click PHP Manager 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/e8685e7a-7fc9-48ee-8d10-c67cf3415064"

</p>
<p>
Next click Register new PHP version 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/7306b22a-d9c4-47cd-a13c-c22189c3df0d"

</p>
<p>
Now you will see this tab, click the three dots on the right side  
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/41dce522-08b6-49ef-9243-06acfc979849"

</p>
<p>
Now go to Windows (C) then click the PHP folder we created earlier 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/5fc2287d-3891-4f09-90db-10fd8095594e"

</p>
<p>
Now click the PHP foler then click php-cgi 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/6fe86a46-0b84-4ade-aa72-032f408026ff"

</p>
<p>
Now you will see the path before you on the white bar then click ok 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/2901ff42-d1e1-4c1e-a35e-2ce825c59a87"

</p>
<p>
Now you will see that the caution sign disappeared from PHP Setup
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/595a7d95-2565-4cb7-9983-e11733485091"

</p>
<p>
Go back to Microsoft Azure and click VM-osticket then click restart. Then click yes to restart the VM
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/604b21b8-d05b-4ab0-9986-946a44874efb"

</p>
<p>
Now you will see that the VM is loading 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/a8f40e8b-259b-4660-bb76-dcd4f9f2f2fa"

</p>
<p>
Now go to the link and download osTicket then click the download symbol
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/6d7500d3-480a-4fb7-aff7-4aa50c591d90"

</p>
<p>
Next open file explorer and you will see osTicket was installed as a zip file 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/87137fd3-8cc0-4926-a9a5-7f2235e18bb1"

</p>
<p>
Next go to Windows (C)
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/38c62aa3-8966-435c-9dcb-3a4f4f697e53"

</p>
<p>
Next click inetpub folder 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/74f015e7-a565-4e39-8bad-f1ccc3d3b733"

</p>
<p>
Now click the wwwroot folder
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/4414217e-1841-4c14-b1b2-428383070e78"

</p>
<p>
Now you will be in the wwwroot folder and see the following 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/3c1336c0-039f-4d02-8de2-9f45665e2370"

</p>
<p>
Next go back to the osTicket folder and click the upload folder 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/0a9c2c82-d3a7-41b9-8f95-b950a333cba7"

</p>
<p>
Now drag the upload file to the wwwroot folder
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/621a3fbf-9c46-44e5-b5f2-dcf69b8dffbc"

</p>
<p>
Once the files are done copying over rename the file osTicket in wwwroot folder
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/28fdac07-22ef-45ce-872d-21715d855117"

</p>
<p>
Next type IIS or Internet Information Services then right click and open as administrator
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/dbbe6ba6-8cae-4594-8245-04d6d9703be9"

</p>
<p>
Now click the VM-osticket and then click restart on the right side 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/f197a0a5-6ab4-4762-9f28-d0d6dd997082"

</p>
<p>
Next click the sites folder 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/9f2dcf36-4862-41fd-9705-162014bd9a5f"

</p>
<p>
Next click the osTicket folder 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/ccf7c523-5f38-45d3-93ec-ce9f609a8378"

</p>
<p>
Now click Browse *80 (http) 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/e92cf47e-ff23-4f18-8af8-0bbfed5fc0bb"

</p>
<p>
You will see the page load with alot of green check and red checks 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/15ebb322-7846-416c-a168-40002b458777"

</p>
<p>
Next go to PHP Manager 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/f5a7a817-f7fd-4e79-89b4-c0cce8c30757"

</p>
<p>
Next click enable or disable an extension 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/cf316f5f-3597-43de-ba8b-ca478e807d7c"

</p>
<p>
Now find php_imap.dll we can see its disbale then click, then go to the top right then click enable 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/6032a21f-0633-4ee4-bd42-525b31f13ab4"

</p>
<p>
Now find php_intl.dll then click, then go to the top right then click enable 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/685a94b1-e2c8-4d3d-88d3-dc1bd8b694d5"

</p>
<p>
Now find php_opcache.dll then click, then go to the top right then click enable
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/3d3d933e-6476-4d35-bd09-990505010049"

</p>
<p>
Now go back to the osTicket home page 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/6817e1a3-678a-4c6b-9301-028e8ba092fe"

</p>
<p>
Next click continue 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/9243111c-d6f7-43aa-b765-a02532c669c0"

</p>
<p>
Now go back to the osTicket folder from wwwroot
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/a9082e43-3950-44fb-b4f6-468d31027b33"

</p>
<p>
Next click the include folder 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/420cadec-f01f-456e-b2e9-1a8a3ade5c87"

</p>
<p>
Now click ost-sampleconfig.php
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/0b8bf4b9-b1e9-4fd8-a608-63f3547fff14"

</p>
<p>
Now rename the file to ost-config.php
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/d60627ee-f02a-4b9a-9032-afe8e002cced"

</p>
<p>
Next right click the file then go to properties 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/efccc130-0736-48c7-8e4f-aff86b2815df"

</p>
<p>
Now click the security tab 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/6b8591bb-9d72-4e85-aa80-909367e8bdf3"

</p>
<p>
Next click the advanced button
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/bed09729-ae50-4835-9986-3bdec63efbb7"

</p>
<p>
Now click disable inheritance 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/48cfbe4d-958a-44aa-b086-084fcc538d64"

</p>
<p>
Next click remove all inherited permission from this object 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/76698c06-c1be-4b37-b711-aa32bc5c3d98"

</p>
<p>
Next click add 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/7ec15b41-f9bd-45fb-b38e-802c7ac64dfd"

</p>
<p>
Next click select a principal
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/13145929-b0ce-4c0e-8343-cf506171320c"

</p>
<p>
Now type everyone 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/87b7593e-b545-4172-a955-e38b65e770a8"

</p>
<p>
Now click ok 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/4eccd1e3-ece1-437f-8e8a-90f42e9c6ad5"

</p>
<p>
Now click all the permissions then click ok 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/97fc2a5d-e066-489c-a4cf-56eb34fceebf"

</p>
<p>
Now click apply 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/7661fcd3-b3a6-4d00-8f06-dd68d90b5484"

</p>
<p>
Next click ok 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/9fb91e24-1b33-4ffa-8135-e7334e60ae75"

</p>
<p>
Now click ok 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/d8d9ea2c-79f8-4be1-87f3-e02e4fee5114"

</p>
<p>
Next go back to the OsTicket home page and click continue
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/4eb6caf9-2feb-410b-beda-f854a72f1c9c"

</p>
<p>
For the helpdesk name type josh help desk, the deafult email type josh@help.com. Now for admin user the first name type josh then the last name type garcia. For email address type josh@gmail.com. For the username josh then type the password I will type Password1. 
</p>

<p>
<img src="https://github.com/user-attachments/assets/f61d5208-2da8-4ee1-a78b-1b8364ff27b1"

</p>
<p>
Now go to back to the link and download HeidiSQL then click the download symbol
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/6f1baf4e-cea5-41d1-b560-9300f10d17e9"

</p>
<p>
Now go to file explorer and double click HediSQL
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/04c15988-cd55-40ee-91a5-80424ce1bb2f"

</p>
<p>
Next click I accept the agreement then click next 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/246bfedb-2e63-405d-9b41-d2acab9fd8e7"

</p>
<p>
Next click install
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/44b4b395-0234-4839-9f47-044d61726c33"

</p>
<p>
You will see the process start 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/cc3694c1-e9b5-41a9-b559-f3aece4d6835"

</p>
<p>
Next click finish 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/bf7a74cb-e6cf-4794-a3d5-7637d307bf0c"

</p>
<p>
Next click skip 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/28f3fc03-4c14-4f14-a775-03eb7cf5720e"

</p>
<p>
Now type root
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/aa002f40-cec3-4139-a21f-3984308417f3"

</p>
<p>
Next for the password section type Password1 then click open
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/404cbac0-8ef8-4979-90ce-9a179f45b28e"

</p>
<p>
Now you will see the unamed tab 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/a87cd869-190c-47f6-b904-d2baa1b2c649"

</p>
<p>
Next type root for the MySQL Username then for the MySQL Password type Password1
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/9d0e27bf-4286-472c-8015-fc6c7ddf58c5"

</p>
<p>
Now right click Unamed then go to create new then click Database
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/967ba176-4172-49ac-b838-d46a61e2e83f"

</p>
<p>
Next type osTicket then click ok 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/bd4ecdbc-ed35-4ccd-bcdf-bf8011abbfe5"

</p>
<p>
Next type osTicket for MySQL Database
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/eb22c624-2050-4663-8a3b-3858d1789c04"

</p>
<p>
Now you will see the process load 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/3304fdb8-2bee-462f-858e-b70d04741aaa"

</p>
<p>
Next you will see the process finish and osTicket was installed
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/784822c6-b7f8-47f9-aa27-8ded2954892c"

</p>
<p>
Next go to the osTicket folder and delete the setup folder
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/5b2394f0-a487-4f20-bc43-c694aa0cb8c4"

</p>
<p>
Now click ost-config.php
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/3756d949-69b6-40c2-b9eb-871c548ba2c1"

</p>
<p>
Right click and go to properties 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/db70c15f-3768-4601-a271-ff3d22c25290"

</p>
<p>
Next click advanced 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/d37763a1-984f-4eab-aa2e-c9d99116eebe"

</p>
<p>
Now click permissions
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/3fb7701c-3f7a-4208-995c-ff6a77947943"

</p>
<p>
Next click allow everyone then click edit 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/60d38c46-9a2d-4534-b2be-eaa3e9437c79"

</p>
<p>
Now uncheck full control, modify, and write then click ok  
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/aa73ed48-6296-4c86-97e9-0a0f0a871518"

</p>
<p>
Now click apply
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/23fab22b-6ddf-47e5-811b-762ffedaf756"

</p>
<p>
Finally click ok then click the link to continue the Post-Installation Configuration https://github.com/Jevanko94/post-install-config/tree/main
</p>
<br />
