<p align="center">
<img src="https://i.imgur.com/NZy2lm2.png"/>  
</p>
                                                                 
<h1>Tenable Nessus Essentials (May 2023)</h1>
In this tutorial, I use Tenable's Nessus vulnerability scanner to observe results from basic scans and credentialed scans on a Windows Virtual Machine.
<br />


<h2>Environments, Operating Systems and Technologies Used</h2>
- Tenable Nessus Essentials

- Windows 10 
- VMware Workstation Player 17
- Command Line for using commands like perpetual ping

<h2>Creating the Windows Virtual Machnine using WMware Workstation Player 17<h2/>                                                             
Install VMware Workstation Player 17

Step 1. Go to VMware website, go to products, and 
select Workstation Player
<p>
<img src="https://i.imgur.com/7zEePso.png"/?
</p>
<br />
<br />

2. Select "Download Free"

<p>
<img src="https://i.imgur.com/2CQn642.png"/?
</p>
<br />
<br />

3. Select version, then "Download Now"

<p>
<img src="https://i.imgur.com/kys9bcy.png"/?
</p>
<br />
<br />

4.Select "Add WMware Workstation console tools..." then "Next"

<p>
<img src="https://i.imgur.com/bUNgoaQ.png"/?
</p>
<br />
<br />

Step 5. Search for Windows 10 ISO file form Microsoft & download

<p>
<img src="https://i.imgur.com/nYqiSse.png"/?
</p>
<br />
<br />  

6. Execute file when it finishes downloading, select "create installation", and hit "next"
<p>
<img src="https://i.imgur.com/b6tGXwE.png"/?
</p>
<br />
<br />                                                           
                                                            
7a. Select "ISO file" and hit "Next"
<p> 
<img src="https://i.imgur.com/2qqNgXd.png"/?
</p>
<br />
<br />

7b. Go back into VMware Workstation, select the Windows ISO file, name your Virtual Machine, click "Next"
<p>
<img src="https://i.imgur.com/qWZR808.png"/?
</p>
<br />
<br />

7c. Select "customize hardware" then select "Bridged" for the network connection. This allows the VM to use your physical network adapter
<p>
<img src="https://i.imgur.com/Mocs50t.png"/?
</p>
<br />
<br />

7d. Wait for Windows 10 to install
<p>
<img src="https://i.imgur.com/yrI5RrA.png"/?
</p>
<br />
<br />
  
Tenable Nessus Download  
8a. Locate Nessus Essentials unter the product tab of Tenable.com
<p>
<img src="https://i.imgur.com/jhIhBOh.png"/?
</p>
<br />
<br />
 
8b. Fill out the registration form & select "download"
<p>
<img src="https://i.imgur.com/k48Koq0.png"/?
</p>
<br />
<br />

8c. Select "download" again. Latest version as May 2023 is 10.5.1
<p>
<img src="https://i.imgur.com/ee5vB9k.png"/?
</p>
<br />
<br />  
  
Step 9a. Execute the downloaded file and select "Connect via SSL"
<p>
<img src="https://i.imgur.com/C19b7ta.png"/?
</p>
<br />
<br />
  
9b. Select "proceed to localhost (unsafe)"
<p>
<img src="https://i.imgur.com/WjLh2tX.png"/?
</p>
<br />
<br />  
  
9c. Insert the unique activation code you were sent to your email when you registered
<p>
<img src="https://i.imgur.com/OfZlz9H.png"/?
</p>
<br />
<br />
 
9d. Wait for Nessus to finish installing & initializing
<p>
<img src="https://i.imgur.com/GqWTi68.png"/?
</p>
<br />
<br />

10a. Open the Command Line Interface, use "ipconfig/all" command to generate & copy VM's IPv4 address
<p>
<img src="https://i.imgur.com/52dP1BZ.png"/?
</p>
<br />
<br />
  
10b. From your host machine open the Command Line & use the IPv4 address to perpetual ping the VM
<p>
<img src="https://i.imgur.com/cui2HMT.png"/?
</p>
<br />
<br />

New Basic Scan  
11a. After installing Nessus, select "Basic Network Scan"
<p>
<img src="https://i.imgur.com/UOPeds8.png"/?
</p>
<br />
<br />
  
11b. Name your scan, input the VM's IPv4 address as a target, & save your scan
<p>
<img src="https://i.imgur.com/EUMV5u3.png"/?
</p>
<br />
<br />
  
11c. Launch your scan & wait for it to complete
<p>
<img src="https://i.imgur.com/YM4ZBos.png"/?
</p>
<br />
<br /> 
 
11d. Once complete, you can select the "vulnerabilities" tab & observe them
<p>
<img src="https://i.imgur.com/VwHdaXH.png"/?
</p>
<br />
<br />   

Credentialed Scan  

Step 12a. Open "services.msc" then go to "remote registry" & enable it by selecting "apply" & "OK"
<p>
<img src="https://i.imgur.com/07dCU36.png"/?
</p>
<br />
<br />

12b. 
<p>
<img src="https://i.imgur.com/tVh4uSl.png"/?
</p>
<br />
<br />
  
12c.
<p>
<img src="https://i.imgur.com/cvAcUUK.png"/?
</p>
<br />
<br />  
  
12d.  
<p>
<img src="https://i.imgur.com/rHlWf6G.png"/?
</p>
<br />
<br />  
  
12e.
<p>
<img src="https://i.imgur.com/zpFnE3L.png"/?
</p>
<br />
<br />  

Step 13a.
<p>
<img src="https://i.imgur.com/wHyc98Q.png"/?
</p>
<br />
<br />   
  
13b.
<p>
<img src="https://i.imgur.com/HyfaFFM.png"/?
</p>
<br />
<br />

13c.
<p>
<img src="https://i.imgur.com/scIgT8v.png"/?
</p>
<br />
<br />  
