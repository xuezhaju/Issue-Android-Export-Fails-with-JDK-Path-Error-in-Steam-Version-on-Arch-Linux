Issue: Android Export Fails with JDK Path Error in Steam Version on Arch Linux

Tested versions

    Version with the issue: Godot Steam Version (4.4.1.stable)

    Version without the issue: Godot from Arch Linux official repositories (4.4.1) - Works correctly ✅

    Additional testing: I have not tested other Godot versions (such as 4.3.stable or earlier 4.4 dev snapshots) due to limited time and resources. The focus of this report is to highlight the discrepancy between the Steam distribution and the official repository version.

    Conclusion: This bug appears to be specific to the Steam distribution/build of Godot 4.4.1, as the same official version from Arch repositories functions correctly with identical settings and projects.

## Description of the Problem 
1. When I try to export my project for Android, the process seems to complete successfully ("everything is OK"). However, the editor also displays an error message: "Invalid Java SDK path in Editor Settings. Missing 'bin' directory".I then installed Godot from the Arch Linux official repositories using the command ** sudo pacman -S godot ** . Using the exact same export settings, the version from the official repositories works without any errors.
2. The key store path selected through the file manager will not be updated in the export settings.
   
 
## [The complete error report GitHub repository link](https://github.com/xuezhaju/Issue-Android-Export-Fails-with-JDK-Path-Error-in-Steam-Version-on-Arch-Linux)

### **Exact Steps to Reproduce**
1. Set up a clean installation of Arch Linux.
2. Install Steam via the command : 
    sudo pacman -S steam
3. Install the Godot Engine from the Steam client.
4. Clone the repository that demonstrates the issue:
    git clone https://github.com/xuezhaju/Qixi-Gift.git
5. Observe that the export process completes but the following error message is displayed:
6. Then you can see the error message:
    "Invalid Java SDK path in Editor Settings. Missing 'bin' directory"


### **Minimal reproduction project**

**N/A** - This issue is not project-dependent. The bug occurs universally in the Steam version of Godot when attempting Android export, regardless of project content. The error is related to JDK path detection in the editor itself.

However, for testing consistency, contributors can use any Godot project or create a new empty project to reproduce the issue.

- [The complete error report GitHub repository link](https://github.com/xuezhaju/Issue-Android-Export-Fails-with-JDK-Path-Error-in-Steam-Version-on-Arch-Linux)