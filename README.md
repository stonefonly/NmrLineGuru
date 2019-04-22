# NmrLineGuru (ver 2.0)

Standalone and User-Friendly GUIs for Fast 1D NMR Lineshape Simulation and Analysis with Multi-State Equilibrium Binding Models

Chao, Mar 2019

## Version Info

1.1 --> 2.0

* Add fitting GUIs for 2-, 3-, and 4-state models
* Fix bugs and update default parameter values
* Include MCR in the installation packages

1.0 --> 1.1

* Bug fix for the GUI starting problem
* A zipped installation file is added for Unix platform

## Introduction

**Nuclear magnetic resonance (NMR) spectroscopy** is a powerful tool for studying protein interactions. The **residue-level** resolution enables the study of dynamics and kinetics of individual binding steps in a multi-state equilibrium for multi-domain proteins. 

This type of study is not very possible for other biophysical methods (e.g. isothermal titration calorimetry, surface plasmon resonance, or fluorescence titration), which are  based on only a single readout of the **whole molecule**.

However, it's often technically difficult to analyze the NMR lineshape data obtained from a titration experiment involving multi-state equilibrium for multi-domain proteins due to the following reasons:

* Multi-state equilibrium involves complex math models
* Fitting NMR lineshape data involves not only equilibrium models but also kinetic models relating with NMR lineshape theory and matrices
* Most existing tools for fitting NMR lineshape data require full installation of MATLAB and other dependencies, lack user-friendly GUIs, require programming knowledge to edit setup scripts, and can only support the simplest 2-state binding model

In the past years, We've been studying the dynamics of Syk tandem SH2 (tSH2) domains and Syk tSH2 interactions with dp-ITAM peptides. NMR lineshape analysis was used to investigate the dynamics and kinetics of each step in the related multi-state equilibrium:

> C Feng and CB Post (2016). Insights into the allosteric regulation of Syk association with receptor ITAM, a multi-state equilibrium. Physical Chemistry Chemical Physics 18 (8), 5807-5818. <a href="https://doi.org/10.1039/c5cp05417f" target="_blank">[DOI]</a> <a href="https://drive.google.com/open?id=0B3uitI9T92-gaDhDdDU5WDhoT1U" target="_blank">[PDF]</a>

During the study, several binding models were built mathematically and a batch of MATLAB code was developed to simulate/fit NMR lineshape data.

To help others dealing with similar research questions, we made a standalone and graphical user interface (GUI) based user-friendly tool: **NmrLineGuru**. 

## Version and Installation

The current version of NmrLineGuru contains 6 GUIs to simulate or fit NMR lineshape data for 2-state, 3-state, and 4-state binding models. More GUIs may be added in future releases.

We provide compiled installation files for two platforms:

* 64-bit version for Windows.
* 64-bit version for Linux. Ubuntu Linux is preferred but it should also work on other Linux releases. 

Please download the correct version and run the install file. During installation, please follow the on-screen prompts to install the software. This software requires the free MATLAB Compiler Runtime (MCR) version 8.3 (R2014a). If your system doesn't have MCR 8.3, the installer will prompt to install it as well.

**For Windows users:**

+ Download and execute [**NmrLineGuru_2.0_Windows.exe**](https://forms.gle/pTGjZG1vS1rHyJas8), the 64-bit version for windows.
+ During installation, select the option to create a shortcut for NmrLineGuru on the desktop. 
+ After installation, click the shortcut to start the program.

**For Linux users**:

+ Download and execute [**NmrLineGuru_2.0_Linux.install**](https://forms.gle/pTGjZG1vS1rHyJas8), the 64-bit version for Linux.
+ During installation, please keep a note of the install path for both NmrLineGuru and MCR. You can install them to anywhere you like. 
+ After installation, run the following command in a shell to start NmrLineGuru:   
  `{NmrLineGuru_Root}/application/run_NmrLineGuru.sh  {MCR_Root}/v83`   
  For example, you installed NmrLineGuru in */home/chao/NmrLineGuru* and MCR in */home/chao/mcr*, so the command line to start NmrLineGuru should be:   
  `/home/chao/NmrLineGuru/application/run_NmrLineGuru.sh  /home/chao/mcr/v83`   
  You may optionally add an alias for this command in the shell starting script. Search *linux shell alias* for how-to.

## Interface and Functions

After starting the software, a GUI selector will appear:

![](screenshots/1-GUI-selector.png)

You'll need to select the binding model and action (simulate or fit). Then, the corresponding GUI will appear to simulate or fit NMR lineshape data with the specified model.

Please follow the tutorials in our project Wiki for how to use these GUIs:   
[https://github.com/stonefonly/NmrLineGuru/wiki](https://forms.gle/pTGjZG1vS1rHyJas8)

## Citation and Contact Info

For academic use, please cite the following references if you used this software for your research or presentation. Your citation is the driving force for us to keep this tool online and work on future releases!

> C Feng, EL Kovrigin and CB Post (2019). NmrLineGuru: Standalone and User-Friendly GUIs for Fast 1D NMR Lineshape Simulation and Analysis of Multi-State Equilibrium Binding Models. Submitted to Scientific Reports.

> C Feng and CB Post (2016). Insights into the allosteric regulation of Syk association with receptor ITAM, a multi-state equilibrium. Physical Chemistry Chemical Physics 18 (8), 5807-5818. <a href="https://doi.org/10.1039/c5cp05417f">[DOI]</a> <a href="https://drive.google.com/open?id=0B3uitI9T92-gaDhDdDU5WDhoT1U">[PDF]</a>

For commercial use, please contact us directly to obtain a license (Copyright @ Purdue Research Foundation, 2019)

Please email us (cbp AT purdue DOT edu) if you have any questions, suggestions, or need consulting services. 
