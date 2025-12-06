<img src="https://github.com/KilianKegel/pictures/blob/master/baustelle.png"  width="50" height="50"><img src="https://github.com/KilianKegel/pictures/blob/master/VS2026.png"  width="125" height="125"><img src="https://github.com/KilianKegel/pictures/blob/master/baustelle.png"  width="50" height="50">
<br>![Visitor](https://visitor-badge.laobi.icu/badge?page_id=KilianKegel.kiliankegel)


# Latest NEWS

## <img src="https://github.com/KilianKegel/pictures/blob/master/New-icon.png"  width="50" height="50">EDK2 Emulator 64Bit + 32Bit + EDK2 StdLibc + toro C Library
[![](https://github.com/KilianKegel/EDK2-EMU/blob/main/media/screenshot.png)](https://github.com/KilianKegel/EDK2-EMU)

## <img src="https://github.com/KilianKegel/pictures/blob/master/refresh-icon.png"   height="50">[<img src="https://github.com/KilianKegel/Visual-ACPICA-for-UEFI-ShellPORTABLE/blob/main/LOGOWin64.PNG" height="200">](https://github.com/KilianKegel/Visual-ACPICA-for-UEFI-ShellPORTABLE?tab=readme-ov-file#visual-acpica-for-uefi-shell)
### enable Windows 64 full DEBUG support (including [**toro C Library** source code](https://github.com/KilianKegel/Visual-TORO-C-LIBRARY-for-UEFI?tab=readme-ov-file#toro-c-library-sourcecode))

## <img src="https://github.com/KilianKegel/pictures/blob/master/New-icon.png"  width="50" height="50">toroCVS (C-Validation-Suite) report ***math.h***
All **C90/ANSI C** functions of **math.h** compared against original **Microsoft C Library** implementation:<br>
[![](https://github.com/KilianKegel/toroCVSreport/blob/main/documents/toroCVS.png)](https://github.com/KilianKegel/toroCVSreport?tab=readme-ov-file#mathh)

## <img src="https://github.com/KilianKegel/pictures/blob/master/refresh-icon.png"  width="50" height="50">[*toro C Library*](https://github.com/KilianKegel/toro-C-Library) with [high precision, micro footprint hardware arithmetic](https://github.com/KilianKegel/Visual-TORO-C-LIBRARY-for-UEFI/tree/main/toroCLibrary/Library/math_h) 
### 20250830, v0.9.5 Build 755
* add [**errno.h**]((https://www.open-std.org/JTC1/SC22/WG14/www/docs/n1256.pdf#page=198)) support for [**math.h** functions](https://www.open-std.org/JTC1/SC22/WG14/www/docs/n1256.pdf#page=224)
* publish **math.h** [**C-Validation Suite results**](https://github.com/KilianKegel/toroCVSreport?tab=readme-ov-file#mathh)

[<img src="https://upload.wikimedia.org/wikipedia/commons/1/14/Intel_C8087.jpg" width="800" >](https://upload.wikimedia.org/wikipedia/commons/a/aa/Intel_8087_die.JPG)<br><br>
[![IEEEx87](https://github.com/KilianKegel/pictures/blob/master/IEEEMilestone.png)](https://math.berkeley.edu/news/congratulations-professor-william-velvel-kahan)

***"Credit must be given to those people who played key roles in the development of the 8087.<br>
The 8087 would not have been possible without the clear insight and strong guidance offerred by*** **Prof. W. Kahan** ***at UC Berkeley.<br>
We did not do as well as he wanted, but we did better than he expected."***
<sup>[[0]](https://github.com/KilianKegel/4KPages-8087PRIMER/blob/main/images/COVERfront.jpeg)</sup>
<sup>[[1]](https://github.com/KilianKegel/4KPages-8087PRIMER/blob/main/images/THE8087PRIMER_005.jpg)</sup>
<sup>[[2]](https://github.com/KilianKegel/4KPages-8087PRIMER/blob/main/images/THE8087PRIMER_006.jpg)</sup>

<br>The [**8087**](https://en.wikipedia.org/wiki/X87#8087) successor [**80387**](https://en.wikipedia.org/wiki/X87#80387) is fully [**IEEE 754**](https://en.wikipedia.org/wiki/IEEE_754-1985) compliant.<br>

The Math-Coprocessor is the foundation of this math library, providing a space-optimized, 
ROM-able implementation of C's MATH.H functions while maintaining the precision and correctness 
already established in earlier x87-based math libraries.<br>

Since the traditional math coprocessor **80387** is still present in current x86 processors and is 
also ***not deprecated*** in the [**X86S specification**](https://www.intel.com/content/www/us/en/developer/articles/technical/envisioning-future-simplified-architecture.html) [.PDF](https://github.com/KilianKegel/4KPages-TechDocs/blob/main/x86s-eas-external-1.1.pdf),
it can be safely used here, now and in the future on x86-based platforms.<br>

The **80387** processor has various improvements over its **8087** predecessor, such as<br>
  * range extension for transcendental function:

    | Instruction  | function                      |
    |--------------|-------------------------------|
    |FPTAN         | Partial tangent               |
    |FPATAN        | Partial arctangent            |
    |F2XM1         | 2<sup>x</sup> - 1             |
    |FYL2X         | Y * log<sub>2</sub>X          |
    |FYL2XP1       |Y * log<sub>2</sub>(X + 1)     |
    
* new instructions, e.g.

    | Instruction  | function                 |
    |--------------|--------------------------|
    |FXAM          |  Examine Floating-Point  |
    |FSIN          | sine                     |
    |FCOS          | cosine                   |

That has reduced the programming effort dramatically and made algorithms very simple and easy to implement.<br>

## [*toro C Library* *source code*](https://github.com/KilianKegel/Visual-TORO-C-LIBRARY-for-UEFI)<br> builds with [LLVM/CLANG tool chain](https://llvm.org/) in Visual Studio 2022
[<img src="https://llvm.org/img/LLVMWyvernSmall.png">](https://github.com/KilianKegel/Visual-TORO-C-LIBRARY-for-UEFI/tree/main?tab=readme-ov-file#torosrc)

# About
**The content on this page is all about developing of <img src="https://github.com/KilianKegel/pictures/blob/master/uefi-logo.png"  width="20" height="20"> UEFI  applications
and drivers using Microsoft <img src="https://github.com/KilianKegel/pictures/blob/master/vs-icon.svg"  width="20" height="20"> Visual Studio 2022 for x86 platforms.**

**The [*toro C Library*](https://github.com/KilianKegel/toro-C-Library) introduced here is written independently of any other source code.<br>
It is a new, independent implementation of the [ANSI C89 / ISO C90+C95 Standard C Library](https://nvlpubs.nist.gov/nistpubs/Legacy/FIPS/fipspub160.pdf).<br>
([Only floating point print/scan-support is currently missing](https://github.com/KilianKegel/toro-C-Library?tab=readme-ov-file#known-bugs) — Instead [MATH.H](https://github.com/KilianKegel/Visual-TORO-C-LIBRARY-for-UEFI?tab=readme-ov-file#20250309-v090-build-243) functions are available !!!)**

### License [**toro C Library** *binary*](https://github.com/KilianKegel/toro-C-Library)
[**toro C Library** binary](https://github.com/KilianKegel/toro-C-Library) is free to use like the [**GLIBC runtime library**](https://www.gnu.org/licenses/gcc-exception-3.1-faq.html)

**Developers are free to use [**toro C Library** binary](https://github.com/KilianKegel/toro-C-Library) to compile any program, regardless of its [license](https://github.com/KilianKegel/toro-C-Library/blob/master/LICENSE.md)**.

### License [**toro C Library** *source code*](https://github.com/KilianKegel/Visual-TORO-C-LIBRARY-for-UEFI)
```
    Copyright (c) 2017-2025, Kilian Kegel. All rights reserved.
    SPDX-License-Identifier: GNU General Public License v3.0
```

# Flagship Projects based on [**toro C Library**](https://github.com/KilianKegel/toro-C-Library)
| Flagship Project | Content|
|--------------|--------------------|
|[**toro C Library**<br>source code](https://github.com/KilianKegel/Visual-TORO-C-LIBRARY-for-UEFI)| <img src="https://llvm.org/img/LLVMWyvernSmall.png"  width="256" height="144">  |
|[**ANSI C for UEFI Shell**](https://github.com/KilianKegel/Visual-ANSI-C-for-UEFI-Shell)| getting started with simple programs <img src="https://github.com/KilianKegel/pictures/blob/master/New-icon.png"  width="18" height="18"> LLVM/CLANG support<br><img src="https://github.com/KilianKegel/Visual-ANSI-C-for-UEFI-Shell/blob/master/CfgMgr.png"  width="256" height="144"><br>|
|[**ACPICA**](https://github.com/KilianKegel/Visual-ACPICA-for-UEFI-ShellPORTABLE?tab=readme-ov-file#visual-acpica-for-uefi-shell)| [**Intel ACPI COMPONENT ARCHITECTURE**](https://www.intel.com/content/www/us/en/developer/topic-technology/open/acpica/overview.html)<br><img src="https://github.com/KilianKegel/Visual-ACPICA-for-UEFI-ShellPORTABLE/blob/main/LOGOWin64.PNG"  width="291" height="45"><br>Original Intel reference implementation running in UEFI Shell:<br>- AslCompiler.EFI<BR>- AcpiBin.EFI<BR>- AcpiDump.EFI<BR>|
|[**UEFI-SHELL**](https://github.com/KilianKegel/UEFI-SHELL)| Build original UEFI SHELL from latest available [**EDK2 drop**](https://github.com/tianocore/edk2/tags)<br><img src="https://github.com/KilianKegel/pictures/blob/master/torouefishell.png"  width="256" height="144"><br>1. integrate Tianocore EDK2 build tools into project (*portable build*)<br>2. introduce ♉toro-UEFI-SHELL with *plugins* and other improvements build with VS2022.   |
|[**TSCSync**](https://github.com/KilianKegel/Visual-TSCSync-for-UEFI-Shell)| TimeStampCounter-Synchronizer<br><img src="https://github.com/KilianKegel/Visual-TSCSync-for-UEFI-Shell/blob/main/TSCSyncDemo.gif"  width="256" height="144"><br>1. Introduce **TUI** TextUserInterface, a menu driven UEFI application — that looks not so bad...<br>2. Introduction of multi chart <img src="https://github.com/KilianKegel/pictures/blob/master/Microsoft_Office_Excel_(2019%E2%80%93present).svg.png"  width="20" height="20"> Excel .XLSX file generation using open source [**libxlsxwriter**](https://github.com/jmcnamara/libxlsxwriter)<br>3. Introduce reliable speed measurement to enable TSC for timer and wallclock usage [**AcpiClkWait()**](https://github.com/KilianKegel/Visual-TSCSync-for-UEFI-Shell/blob/main/TSCSync/AcpiClkWait.c#L51) vs. [**InternalAcpiDelay()**](https://github.com/tianocore/edk2/blob/master/PcAtChipsetPkg/Library/AcpiTimerLib/AcpiTimerLib.c#L150)|
|[**Visual-LIBXLSXWRITER-for-UEFI-Shell**](https://github.com/KilianKegel/Visual-LIBXLSXWRITER-for-UEFI-Shell)| Create XLSX tables in UEFI and Windows applications<br>[**libxlsxwriter**](https://github.com/jmcnamara/libxlsxwriter?tab=readme-ov-file#libxlsxwriter)-port to **Visual Studio**<br><img src="https://github.com/KilianKegel/Visual-LIBXLSXWRITER-for-UEFI-Shell/blob/main/visualUefiWideXLSXWriter.png"  width="256" height="144"><br>Also for Windows.|
|[**EDK2 Emulator**](https://github.com/KilianKegel/EDK2-EMU)|Get started with the original **TianoCore UEFI/BIOS Framework** in the Windows Emulator.<br><br>Understand UEFI software, configuration and build architecture from the ground up.<br><img src="https://github.com/KilianKegel/EDK2-EMU/blob/main/media/screenshot.png"  width="256" height="144"><br>|

## <img src="https://github.com/KilianKegel/pictures/blob/master/refresh-icon.png"  width="48" height="48">HOWTO
| HOWTO|
|--------------|
|[**Howto setup a UEFI-Development-PC**](https://github.com/KilianKegel/Howto-setup-an-UEFI-Development-PC#howto-setup-a-uefi-development-pc)|
|[**Howto create a UEFI-Shell-Boot-Drive**](https://github.com/MinnowWare/Howto-create-a-UEFI-Shell-Boot-Drive#howto-create-a-uefi-shell-boot-device)|
|[**Howto configure VS2022 to build .EFIexecutables**](https://github.com/KilianKegel/Howto-configure-VS2022-to-build-.EFI-executables#howto-configure-vs2022-to-build-efi-executables)
|[**Howto-configure-DDK-and-WDK-for-Standard-C-usage**](https://github.com/KilianKegel/Howto-configure-DDK-and-WDK-for-Standard-C-usage) |
|[**[obsolete] Howto-setup-a-YOCTO-Development-PC**](https://github.com/KilianKegel/Howto-setup-a-YOCTO-Development-PC)|
|[**git-for-gits**](https://github.com/KilianKegel/git-for-gits)|

<!--
## Projects

[![Repo name](https://github-readme-stats.vercel.app/api/pin/?username=KilianKegel&repo=toro-C-Library#toro-c-library-formerly-known-as-torito-c-library)](https://github.com/KilianKegel/toro-C-Library#toro-c-library-formerly-known-as-torito-c-library)
[![Repo name](https://github-readme-stats.vercel.app/api/pin/?username=KilianKegel&repo=Visual-TORO-C-LIBRARY-for-UEFI)](https://github.com/KilianKegel/Visual-TORO-C-LIBRARY-for-UEFI)
[![Repo name](https://github-readme-stats.vercel.app/api/pin/?username=KilianKegel&repo=Visual-TSCSync-for-UEFI-Shell#visual-tscsync-for-uefi-shell)](https://github.com/KilianKegel/Visual-TSCSync-for-UEFI-Shell#visual-tscsync-for-uefi-shell)
[![Repo name](https://github-readme-stats.vercel.app/api/pin/?username=KilianKegel&repo=UEFI-SHELL-binary-source-and-build-environment#edk2-uefi-shell--visual-uefi-shell)](https://github.com/KilianKegel/UEFI-SHELL-binary-source-and-build-environment#edk2-uefi-shell--visual-uefi-shell)
[![Repo name](https://github-readme-stats.vercel.app/api/pin/?username=KilianKegel&repo=Visual-ANSI-C-for-UEFI-Shell#visual-ansi-c-for-uefi-shell)](https://github.com/KilianKegel/Visual-ANSI-C-for-UEFI-Shell#visual-ansi-c-for-uefi-shell)
[![Repo name](https://github-readme-stats.vercel.app/api/pin/?username=KilianKegel&repo=Visual-DOS-Tools-for-UEFI-Shell)](https://github.com/KilianKegel/Visual-DOS-Tools-for-UEFI-Shell)
[![Repo name](https://github-readme-stats.vercel.app/api/pin/?username=KilianKegel&repo=Visual-ACPICA-for-UEFI-Shell)](https://github.com/KilianKegel/Visual-ACPICA-for-UEFI-Shell)
[![Repo name](https://github-readme-stats.vercel.app/api/pin/?username=KilianKegel&repo=Visual-LIBWIN32-for-UEFI)](https://github.com/KilianKegel/Visual-LIBWIN32-for-UEFI)
[![Repo name](https://github-readme-stats.vercel.app/api/pin/?username=KilianKegel&repo=Visual-HWTools-for-UEFI-Shell)](https://github.com/KilianKegel/Visual-HWTools-for-UEFI-Shell)
[![Repo name](https://github-readme-stats.vercel.app/api/pin/?username=KilianKegel&repo=Visual-LIBXLSXWRITER-for-UEFI-Shell)](https://github.com/KilianKegel/Visual-LIBXLSXWRITER-for-UEFI-Shell)
[![Repo name](https://github-readme-stats.vercel.app/api/pin/?username=KilianKegel&repo=CdePkg#CdePkg)](https://github.com/KilianKegel/CdePkg#CdePkg)
[![Repo name](https://github-readme-stats.vercel.app/api/pin/?username=KilianKegel&repo=CdePkgValidation#cdepkgvalidation)](https://github.com/KilianKegel/CdePkgValidation#cdepkgvalidation)
[![Repo name](https://github-readme-stats.vercel.app/api/pin/?username=KilianKegel&repo=-obsolete-EDK2020-MinnowBoard#edk2020-minnowboard-featuring-cdepkg-c-development-environment-package)](https://github.com/KilianKegel/-obsolete-EDK2020-MinnowBoard#edk2020-minnowboard-featuring-cdepkg-c-development-environment-package)
[![Repo name](https://github-readme-stats.vercel.app/api/pin/?username=KilianKegel&repo=Howto-setup-a-UEFI-Development-PC)](https://github.com/KilianKegel/Howto-setup-an-UEFI-Development-PC#howto-setup-a-uefi-development-pc)
[![Repo name](https://github-readme-stats.vercel.app/api/pin/?username=KilianKegel&repo=Howto-create-a-UEFI-Shell-Boot-Drive)](https://github.com/MinnowWare/Howto-create-a-UEFI-Shell-Boot-Drive#howto-create-a-uefi-shell-boot-device)
[![Repo name](https://github-readme-stats.vercel.app/api/pin/?username=KilianKegel&repo=Howto-configure-VS2022-to-build-.EFI-executables#howto-configure-vs2022-to-build-efi-executables)](https://github.com/KilianKegel/Howto-configure-VS2022-to-build-.EFI-executables#howto-configure-vs2022-to-build-efi-executables) [![Repo name](https://github-readme-stats.vercel.app/api/pin/?username=KilianKegel&repo=git-for-gits)](https://github.com/KilianKegel/git-for-gits)
[![Repo name](https://github-readme-stats.vercel.app/api/pin/?username=KilianKegel&repo=Howto-configure-DDK-and-WDK-for-Standard-C-usage)](https://github.com/KilianKegel/Howto-configure-DDK-and-WDK-for-Standard-C-usage) 
[![Repo name](https://github-readme-stats.vercel.app/api/pin/?username=KilianKegel&repo=-obsolete-Howto-setup-a-YOCTO-Development-PC)](https://github.com/KilianKegel/-obsolete-Howto-setup-a-YOCTO-Development-PC)
[![Repo name](https://github-readme-stats.vercel.app/api/pin/?username=KilianKegel&repo=papers-bugs-miscellaneous-...-#cdepkg-blog-at--uefi--tianocore)](https://github.com/KilianKegel/papers-bugs-miscellaneous-...-#cdepkg-blog-at--uefi--tianocore)
-->
### keywords
<h6>ANSI C for UEFI, ISO C for UEFI, ANSI C UEFI, ISO C UEFI, Standard C for UEFI, UEFI LIBC, EFI LIBC, LIBC UEFI , LIBC EFI , UEFI application, UEFI driver, Visual Studio UEFI, Visual Studio 2022 UEFI, UEFI Standard C Library, Standard C Library UEFI,Standard LIBC UEFI, C LIB UEFI, C LIBRARY UEFI, UEFI C, C UEFI, UEFI C Library, LIBC UEFI, programming uefi, uefi programming,
 UEFI, programming efi, efi programming, uefi app, app uefi, efi app, app efi, <br>👺 SCLIBnot Standard C LIBrary neat odd thing
<br>
<br>   
