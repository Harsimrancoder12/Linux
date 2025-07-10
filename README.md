## Linux over Windows
### Why to use Linux over Windows?

      
| Reason                         | Explanation                                                             |
| ------------------------------ | ----------------------------------------------------------------------- |
| **Cost**                       | Linux is free, while Windows requires a paid license.                   |
| **Open Source**                | Linux’s code is open for review, customization, and improvement.        |
| **Security**                   | Linux requires host password for every change hence it's more secure.   |
| **Customizability**            | Linux offers extensive options to customize the UI.              |
| **Performance**                | Linux can run efficiently on older hardware.                            |
| **Software Freedom**           | You can freely modify and redistribute Linux software.                  |
| **Stability and Reliability**  | Preferred for servers and critical systems due to strong stability.     |
| **Community Support**          | Large, active communities for help and troubleshooting.                 |
| **No Forced Updates**          | Users control when and what updates to install. It's never "take it or leave it", there's always choices.|


### Downloaded 3 softwares:
1. [Oracle Virtual Machine](https://download.virtualbox.org/virtualbox/7.0.20/VirtualBox-7.0.20-163906-Win.exe)
2. [Ubuntu 24.04.02](https://login.gndec.ac.in/ubuntu-24.04.2-desktop-amd64.iso)
3. [Microsoft Visual C++](https://download.visualstudio.microsoft.com/download/pr/40b59c73-1480-4caf-ab5b-4886f176bf71/D62841375B90782B1829483AC75695CCEF680A8F13E7DE569B992EF33C6CD14A/VC_redist.x64.exe)

   
**After instalation, start Oracle VM.**
- Go to new.
- Then enter the name, *Ubuntu*
- Select the path of Ubuntu in ISO image.
- Enter password and username.
- Give required memory space and Processors.
## Issues faced:
After powering up, the display only showed a black screen with error:

![Error](../images/error.jpg)


**To solve:**
- Go to settings -> Display
- Change the Graphics controller to **VBoxVGA.**
  
   ![Solved](images/Screenshot%202025-06-25%20210905.png)
   ![Solved](images/Screenshot%202025-06-25%20211122.png)

## Booting and its types:
Booting is the process of starting up or restarting a computer, which involves initializing hardware, loading the operating system, and preparing the computer for use.
### Types of Booting:
- **Cold boot/ Hard boot:**
  This refers to starting the computer from a completely powered-off state.
- **Warm boot/ Soft boot:**
  This is when the operating system alone is restarted wihtout turning it off.
