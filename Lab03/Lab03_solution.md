# Lab 3: Malware analysis



### Name: Mohamad Nour Shahin
### Group number: B22-CBS-01



# Questions to Answer

## 1. Preparation


Choose a sandboxing solution, some recommended ones includes the following.

- [Cuckoo (Bonus point if you set up Cuckoo in an isolated VM)](https://cuckoo.readthedocs.io/en/latest/installation/host/installation/)
- [Hybrid Analysis](https://www.hybrid-analysis.com/)
- [Any.run](https://app.any.run/)
- [Intezer Analyze](https://intezer.com/intezer-analyze/)
- [Joe Sandbox](https://www.joesandbox.com/#windows)

---

### Solution:

I will choose third choice [Any.run](https://app.any.run/) as we practice with it during lab.
I created an account on it.
here is the screenshot of it:

   ![alt text](image.png)


---

## 2. Let's get some malware

Select a malware that you want to analyse in the sandbox selected in step 1.
>
- You can download some malware/ransomware from the internet. For example [TheZoo](https://https//github.com/ytisf/theZoo), [MalwareBazaar Database](https://bazaar.abuse.ch/). You can also check your email for any spam with malicious attachment.

- Don't select the same malware used in the classwork.
- Be careful when you run them, these are real malware.
>


---




### Solution:

I searched in the [MalwareBazaar Database](https://bazaar.abuse.ch/), and I will use this [Malware](https://bazaar.abuse.ch/sample/01ec7b1066df7c55e262dc375bff5fd13a1fc9706c3db4b3522ac8b9d2453b52/) 


   ![alt text](image-1.png)

   ![alt text](image-2.png)

---


## 3. Sandbox analysis

Run your malware in the sandbox.

- See what kind of traces, artifacts, connections your sandbox detects.
- Analyze the behavior of the malware, and write about what the malware does and the goals of the malware.
- Does the malware have some sandbox detection? If yes, try to detect and defeat the techniques used for that.


### Solution:


1. Firstly I downloaded the malware as zip, unzip, upload the file to the [Any.run](https://app.any.run/) , and I will set the configuration:

   ![alt text](image-10.png)

- after unzip it:

   ![alt text](image-11.png)


   ![alt text](image-12.png)

- we add more time for analyzing.

   ![alt text](image-13.png)

- proccessing:

   ![alt text](image-14.png)

- after processing:

   ![alt text](image-15.png)

---

1. connections:

   ![alt text](image-24.png)

   ![alt text](image-25.png)

   ![alt text](image-26.png)

   ![alt text](image-27.png)

---

2. while monitoring the process:

- first process:

   ![alt text](image-19.png)

- second and third process:

   ![alt text](image-20.png)
   ![alt text](image-21.png)

- fourth process:

   ![alt text](image-22.png)  


- fifth process it's trying to sleep to evasion detection, but we got it with increasing the time and without it:
 
   ![alt text](image-23.png)

--- 

3.  I run it without more time, and I got same results. So the malware didn't have sandbox detection.


   ![alt text](image-16.png)

   ![alt text](image-17.png)


---

4. Links to reports generated by the tool:

   [Any.run](https://app.any.run/tasks/9e47862f-89ea-491c-b18a-ca3ec27bca42)

   [Without increasing the time](https://any.run/report/01ec7b1066df7c55e262dc375bff5fd13a1fc9706c3db4b3522ac8b9d2453b52/8ee8109d-d072-42d3-ab8c-98de8991229c)
   [With increasing the time](https://any.run/report/01ec7b1066df7c55e262dc375bff5fd13a1fc9706c3db4b3522ac8b9d2453b52/9e47862f-89ea-491c-b18a-ca3ec27bca42)


---

## 4. Remediation


- Suggest remediation actions for eradicating the malware from compromised endpoints. Include this in your malware analysis report.


> Note that generic recommendations will not be accepted. You need to suggest very specific steps that align with the results from your analysis.


For example:

- Remove the executable dropped at C:\Program Files\dotnet\malware.exe ✅
- Remove the dropped executable ❌
Another example:

- Create a rule on the network firewall to block IP address xx.xx.xx.xx ✅
- Create a firewall rule ❌
>





---



### Solution:


1. Remove the executable dropped at C:\Users\admin\AppData\Local\Temp\01ec7b1066df7c55e262dc375bff5fd13a1fc9706c3db4b3522ac8b9d2453b52.exe
2. kill this secduled task Updates\ZcwWvGIJLelYh

   ![alt text](image-28.png)


5. restart the configuration C:\Users\admin\AppData\Roaming\vkl.exe" to its previous value or defualt one.

   ![alt text](image-31.png)

6. Remove the script files  "C:\Users\admin\AppData\Local\Temp\install.vbs" 

   ![alt text](image-32.png)

7. Create a rule on the network firewall to block IP address 40.127.240.158 which has unkown Rep with proccess name: svchost.exe or null 

   ![alt text](image-33.png)

   ![alt text](image-34.png)

8. Create a rule on the network firewall to block IP address  239.255.255.250 which has unkown CN with proccess name: svchost.exe or null 

   ![alt text](image-33.png)

   ![alt text](image-34.png)

---
