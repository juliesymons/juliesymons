#Download and Set up Instructions

*   [System Requirements](#sysreq)
*   [Programming Environment](#lang)
*   [Download, Install, and Configure Programming Environment](#steps)
*   [Download CCT-Tutorial and Verify](#clone)
*   [Common Problems](#gotchas)

<h2 id="sysreq">System Requirements</h2>
* 64-bit architecture (Linux, Windows, OS X)
* GPU Hardware (NVIDIA, AMD, Intel)
* OpenCL (already included by default with most GPU drivers)

<h2 id="lang">Programming Environment</h2>
* Scala 
* SBT (Scala build tool)
* IntelliJ IDEA (preferred IDE) 

<h2 id="steps">Download, Install, and Configure Programming Environment</h2>

Note: These instructions are based on the preferred IDE, IntelliJ IDEA. 

1.  Download and install the lastest 64-bit JDK (JDK8)
2.  Download and install the latest [IntelliJ IDEA IDE](https://www.jetbrains.com/idea/download) (Community Edition works fine) 
3.  Install Scala Plugin in IntelliJ. The Scala Plugin includes SBT.

     From the Welcome window, select *Configure*, select *Install JetBrains Plugins*, select *Scala*, click *Install*

4.  Configure the project SDK in IntelliJ 

     From the Welcome screen, Select *Configure*, select *Project Defaults*, select *Project Structure*. If there is *\<No SDK>*, click *New* to add the JDK that was installed in Step 1.

Now you are ready to clone a CCT repository. 


<h2 id="clone">Download CCT-Tutorial and Verify</h2>

1. Check out from Version Control.
2. Verify by running the BackgroundSubtraction sample application. (Requires X display capabilities on Linux)

Now you are ready for "Getting Started".  (add link to getting started or the home page of the tutorial)

<h2 id="gotchas">Common Problems</h2>
1.  git-lfs - describe problem/symptom and solution
2.  Proxy settings: set proxy environment variables and inside IntelliJ (Configure -> Plugins -> Browse Repositories -> HTTP Proxy Settings...)
3.  Intellij 32 bit launcher: 
4.  IDEA_JDK_64 environment variable 

  
