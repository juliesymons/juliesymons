#Download and Set up Instructions

*   [System Requirements](#sysreq)
*   [Programming Environment](#lang)
*   [Download/Install/Confgiure Steps](#steps)
*   [Gotchas](#gotchas)
    *   [Proxy](#proxy)
    *   [32-bit](#arch)
    *   [Git-lfs](#git-lfs)

<h2 id="sysreq">System Requirements</h2>
* 64-bit architecture (Linux, Windows, MacOS)
* GPU Hardware (NVIDIA, AMD, Intel)
* OpenCL (already included by default with most GPU drivers)

<h2 id="Language">Programming Environment</h2>
* Scala 
* SBT (Scala build tool)
* IntelliJ IDEA (preferred IDE) 

##Download, Install, Configure environment

Note: These instructions are based on the preferred IDE, IntelliJ IDEA. 

1.  Download and install 64 bit JDK (JDK8)
2.  Download and install IntelliJ IDEA IDE (Community Edition works fine) // choose 64 bit desk top icon 
// check if 64 bit launcher is still required
3.  Configure IntelliJ
3a.  Set the environment variable IDEA_JDK_64 to point to the JDK. For example:
> IDEA_JDK_64=C:\Program Files\Java\jkd1.8.0._73
3b.  Install Scala Plugin (Configure -> Plugins -> Scala -> Install/Update) - does download and configure
      now it is a "Featured Plugin"
3c.  Configure project SDK (Configure->Project Defaults->Project Structure->For Project SDK, add a new JDK to the one installed above.
4.  Download the cct-tutorial from IntelliJ 
4a.  Check out from Version Control
4b.  Verify


Other Gotchas
1.  set proxy environment variables and inside IntelliJ (Configure -> Plugins -> Browse Repositories -> HTTP Proxy Settings...)
2.  try with intellij 32 bit?
3.  IDEA_JDK_64 // try without this set on Omen
4.  git-lfs
