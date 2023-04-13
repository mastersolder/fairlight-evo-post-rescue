Master Solder's - Fairlight EVO Post rescue page
================================================

This guide is designed to assist in building a functional computer unit necessary for operating the Fairlight EVO Post mixing console in case of emergency (system or hardware failures). By following these steps, users will be able to run the Dream II software on any x64 system with a CC-2 card, without the need for a dongle (which can no longer be bought, created or recovered).

The development of EVOPostPatchTool was initiated with the objective of circumventing the security measures implemented in Dream II x64 v5.3.22.7215, the latest software utilized by the Fairlight EVO mixing console. Following the acquisition of Fairlight by Black Magic Design in 2016, the support for this highly valued console was terminated, leaving the console owners out in the cold without any viable options for maintenance or upgrades. The console's operation is contingent upon a license key incorporated within a USB dongle, which is directly associated with the USB flash drive serial number, mainboard (system-id) and CC-2 serial number. In the event of a malfunction or failure of any of these elements, the continued use of the EVO console is rendered unfeasible, an outcome that is deemed unsatisfactory, especially given the cost of the device in 2017. Consequently, this tool was designed to provide assistance to EVO console owners in such situations.

This tool has the capability to patch your Dream II software, thereby enabling it to function at full capacity without the need for a dongle and license on any system, with any CC-2 card.

Although Dream II could be considered abandoned software, it should be noted that utilizing patching software may breach its license agreement. Consequently, the use of this tool is solely at one's **own risk and responsibility**. We strongly recommend its use on a system that has been newly installed, subsequent to running the setups of Windows 7 Pro &amp; EVO Post Setup.

It is imperative to emphasize that the acquisition of legal software should always be prioritized, wherever feasible. It is worth noting that this tool was solely developed to offer support to current EVO console owners and should not be construed as a means to facilitate software piracy.

*Dedicated to Fairlight.  
Master Solder*

# Continue at own risk and responsibility

## Install instructions

Step 1: Install a fresh SSD and Windows 7 Pro ([en_windows_7_ultimate_with_sp1_x64_dvd_u_677332.iso](https://archive.org/details/en_windows_7_ultimate_with_sp1_x64_dvd_u_677332_202006)).

Step 2: Ensure that the ethernet adapter is functioning correctly by installing drivers if necessary.

Step 3: Verify that the graphics adapter is running with its vendor drivers and is capable of hardware acceleration. If required, install DirectX. Failure to do so may result in Dream II not starting with no feedback.

Step 4: Install the full version of .NET Framework 4 ([dotNetFx40_Full_x86_x64.exe](https://archive.org/details/dotNetFx40_Full_x86_x64_201607)).

Step 5: Update Windows using the built-in Windows Update feature as much as possible.

Step 6: Install the following manual windows updates (pick the Windows 7 x64 versions):

- [windows6.1-kb3125574-v4-x64_2dafb1d203c8964239af3048b5dd4b1264cd93b9.msu](https://www.catalog.update.microsoft.com/Search.aspx?q=KB3125574)
- [windows6.1-kb4490628-x64_d3de52d6987f7c8bdc2c015dca69eac96047c76e.msu](https://www.catalog.update.microsoft.com/search.aspx?q=kb4490628)

Step 7: Install the latest version of the EVO Post software ([Post x64_v5.3.22.7215_setup.exe](http://steverance.com/Downloads/Release%20Software/Post%20x64_v5.3.22.7215_setup.exe))

- Choose to enable the optional 3DAW components
- Skip registration (if asked), choose "already registered".

Step 8: Install the CC-2 Crystal Driver:

- Run as administrator: C:\Program Files\Fairlight\Dream II\Crystal Drivers\CC1_Driver_Install.bat
- Reboot
- Verify that under Device Manager / Sound, video and game controllers, there is a device named "Fairlight CC-2 Card," and that the driver runs without any warnings. If not, try to manually assign a driver by pointing to this directory: C:\Program Files\Fairlight\Dream II\Crystal Drivers\x64

Step 9: Run [EVOPostPatchTool](https://github.com/mastersolder/fairlight-evo-post/releases) as an administrator and follow the instructions in the tool.

Step 10: Enjoy using your EVO Post system again.

