<a name="readme-top"></a>

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://www.flimlabs.com/">
    <img src="../../assets/flimlabs-logo.png" alt="Logo" width="120" height="120">
  </a>
</div>


<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li>
      <a href="#home-section">Home section</a>
      <ul>
        <li>
           <a href="#load-a-saved-experiment">Load a saved experiment</a>
        </li>
         <li>
           <a href="#load-a-saved-configuration">Load a saved configuration</a>
        </li>
         <li>
           <a href="#manage-settings">Manage settings</a>
        </li>
         <li>
           <a href="#start-an-experiment">Start an experiment</a>
        </li>
      </ul>
    </li>
    <li>
      <a href="#start-an-experiment">Start an experiment</a>
      <ul>
        <li>
           <a href="#configure-an-experiment">Configure an experiment</a>      
        </li>
         <li>
            <a href="#wizard-mode">Wizard mode</a>
         </li>
         <li>
             <a href="#advanced-mode">Advanced mode</a>
         </li>
         <li>
            <a href="#experiment-settings">Experiment settings</a>
         </li>
      </ul>
    </li>
    <li>
      <a href="#imaging-reconstruction-experiment">Imaging Reconstruction experiment</a>
      <ul>
        <li>
           <a href="#region-of-interest-(roi)">Region of Interest (ROI)</a>        
        </li>
         <li>
            <a href="#software-calibration">Software calibration</a>
        </li>
         <li >
           <a href="#start-the-data-acquisition">Start the data acquisition</a>
        </li>
         <li >
           <a href="#data-analysis">Data analysis</a>          
          <ul>
            <li>
            <a href="#reconstructed-image-section-[1]">RECONSTRUCTED IMAGE SECTION [1]</a>            
            </li>
          </ul>
        </li>
      </ul>
    </li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->
## About The Project

Welcome to [FLIM LABS STUDIO](https://www.flimlabs.com/flim-studio-software/), a software that aims at simplifying the data acquisition, reconstruction and analysis of fluorescence lifetime imaging experiments. The environment provides a user-friendly interface and intuitive tools that can be used by any user.




### Key features

* Real time imaging and fluorescence decay histogram data reconstruction
* Real time FLIM phasor-plot analysis (FLIM PHASORS)
* AI-driven phasor-plot analysis techniques (GMM)
* Double software configuration mode (Wizard, Advanced)
* Software calibration guided process (Scouting, Refrence, Data)
* Software API for data acquisition and reconstruction (Python)
* Supported platform: Windows

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- GETTING STARTED -->
## Getting Started
You can download our software latest version at this [link](https://www.flimlabs.com/setup/flimlabsstudio-installer-1.0.b6.exe). Or check our changelog for different versions at this [link](https://github.com/Federico-O-5bits/flimlabs.github.io/blob/main/products/flim-studio/changelog.md).

### Prerequisites
* Possess a [FLIM LABS acquisition card](https://www.flimlabs.com/products/data-acquisition-card/) to be able to acquire your data
* Windows OS

### Installation

Once the download is completed follow these steps to install FLIM STUDIO on your pc:

* Double click on the FLIM STUDIO installer, the installation process will start.
* Enter the serial number you have been provided, then click the "Next>" button.
* Read the license agreement, click the "I Agree" button in order to proceed with the installation process.
* Chose the installation folder or leave the default value, Then click the "Install" button.
* Once the installation is completed click the "Close" button.
* Now FLIM STUDIO is ready to run on your PC.

  
  <p align="right">(<a href="#readme-top">back to top</a>)</p>
<!-- HOME SECTION -->  
## Home section

The home section is the first view you'll see when starting FLIM STUDIO.

<div align="center">
    <img src="../../assets/flim-studio/flim-studio-home.PNG" alt="flim studio home section">
</div>

Here you can perform several actions:

* **Load a saved experiment**  
The "Last experiment saved" section shows a list of saved experiments, for each of them you can read the name on the top of the figure and the data at the bottom.
Click on a saved experiment to load it in FLIM STUDIO
Click the reload button to refresh the list.

* **Load a saved configuration**  
The "Last configuration used" section shows a list of the previous configurations saved, for each configuration you can read the name on the top of the figure and the data at the bottom.
Click on a saved configuration to load it in FLIM STUDIO
Click the reload button to refresh the list.

* **Manage settings** 
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Fusce non neque efficitur, lobortis neque facilisis, tempus est. Quisque dui arcu, hendrerit sit amet placerat id, tincidunt ac sapien. In interdum mi mi, vitae posuere nisl consectetur eget. Duis aliquet elit sit amet lacus malesuada lobortis. Ut gravida mauris ac quam egestas elementum. Curabitur vitae justo bibendum, vestibulum nibh vitae, auctor leo.

* **Start an experiment**  
Click the "Start" button to begin an experiment, the menu will require you to select the modality through execute it (Wizard, Advanced, From Local Folder)  
*Check the sections below for detailed information about each modality*
<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Start an experiment

<a name="experiment-configuration"></a>

### Configure an experiment
The first step to start an experiment is the configuration.
FLIM STUDIO provides two configuration modalities, **WIZARD MODE** and **ADVANCED MODE**.

### Wizard mode
In this mode, a graphical representation of the settings being configured is provided, along with a step-by-step process. This allows the user to benefit from a guided and simplified experience, optimizing the setup process.

### Advanced mode 
The advanced mode bring a comprehensive range of customization options and provides the ability to fine-tune and set additional parameters, offering an expanded suite of options in a single view.
<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Experiment settings

This table summarize the settings you will need to configure for both the Wizard and Advanced modes.

| Field name           | Value type         | Wizard mode | Advanced mode | Mandatory | Imaging | Spectroscopy |
|----------------------|--------------------|:-----------:|:-------------:|:---------:|:-------:|:------------:|
| Device               | Flim data acquisition card name | ✅ | ✅ | ✅ | ✅ | ✅ |
| Type of experiments  | Imaging \| Spectroscopy | ✅ | ✅ | ✅ | ✅ | ✅ |
| Sync in              | USB \| SMA         | ✅ | ✅ | ✅ | ✅ | ✅ |
| Sync out             | USB \| SMA         | ✅ | ✅ | ❌ | ✅ | ✅ |
| Channel (from 1 to 8)| USB \| SMA         | ✅ | ✅ | ✅ | ✅ | ✅ |
| Reconstruction mode  | Pixel,Line & Frame \| Line & Frame \| Pixel | ✅ | ✅ | ✅ | ✅ | ❌ |
| Pixel                | USB \| SMA         | ✅ | ✅ | ❌ | ✅ | ❌ |
| Line                 | USB \| SMA         | ✅ | ✅ | ❌ | ✅ | ❌ |
| Frame                | USB \| SMA         | ✅ | ✅ | ✅ | ✅ | ❌ |
| Pixel dwell time     | number(μs)         | ✅ | ✅ | ✅ | ✅ | ✅ |
| Pixel size           | number(μm)         | ✅ | ✅ | ✅ | ✅ | ✅ |
| Harmonic content     | number             | ❌ | ✅ | ✅ | ✅ | ✅ |
| Box width/height     | pixels (px)        | ✅ | ✅ | ✅ | ✅ | ✅ |
| Number of pixel on x/y line     | pixels (px)        | ✅ | ✅ | ✅ | ✅ | ✅ |
| Offset left/right/top/bottom     | pixels (px)        | ✅ | ✅ | ❌ | ✅ | ✅ |


<p align="right">(<a href="#readme-top">back to top</a>)</p>


This table provides a more in-depth explanation of what each field means. 

| Field name          | Explanation                                                                                   |
|---------------------|-----------------------------------------------------------------------------------------------|
| Device              | FLIM STUDIO require a FLIM DATA ACQUISITION CARD to connect in order to execute the experiment, select the DATA ACQUISITION CARD connected to your pc |
| Type of experiments | Choose the type of experiment to perform: <br><br> **Imaging**: Image reconstruction transforms raw data into visual representations. It uses a scanning system, including mirrors and a lens, to precisely move a laser beam over a sample, pixel by pixel. Alternatively, a motorized stage can move the sample instead. This precise control is crucial for collecting accurate spatial information. <br><br> **Spectroscopy**: Fluorescence Correlation Spectroscopy (FCS) studies molecular dynamics by analyzing fluorescence fluctuations. It observes fluorescent molecules diffusing in and out of a specific volume, identifying individual molecular properties. The technique involves statistically analyzing time-dependent intensity F(t) to understand the amplitude and frequency of these fluctuations. FCS calculates the correlation between F(t) and F(t+τ) over various delay times τ, yielding an autocorrelation function G(τ) that reveals details about the fluorescent molecules.                                                      |
| Sync in              | The Sync In port is responsible for accepting the input signal from the laser. Specify whether you will use a USB cable or SMA to connect to the Sync In port. |
| Sync out             | The Sync out port is responsible for activating and modulating a laser source. Specify whether you will use a USB cable or SMA to connect to the Sync out port. |
| Channel (from 1 to 8)| Indicate the number of channels to be utilized for fluorescence sampling and choose the connection method – either USB cable or SMA – for that channel. |
| Reconstruction mode   | Specify wich spatial coordinates will be provided for the data acquisition. <br>Image reconstruction involves the use of three fundamental spatial coordinates: Pixel clock, Line clock, and Frame clock. Each of these coordinates plays a crucial role in accurately mapping the spatial information necessary for reconstructing a detailed and coherent image from the collected data. <br><br> FLIM STUDIO allows for conducting experiments with excellent results even when not all three spatial coordinates are available. The experiment can be carried out even in the presence of only the line clock and frame clock coordinates, or just the frame clock coordinate alone. |
| Pixel                 | Specify whether you will connect to this port via SMA or USB cable (refer to port ref3). <br> This port is intended to receive data regarding the spatial coordinate Pixel clock. <br> The spatial coordinate Pixel clock dictate the exposure time of each pixel (dwell time). |
| Line                  | Specify whether you will connect to this port via SMA or USB cable (refer to port ref3). <br> This port is intended to receive data regarding the spatial coordinate Line clock. <br> Govern the readout speed of each pixel row (refer to port ref2). Specify whether you will connect to this port via SMA or USB cable. |
| Frame                 | Specify whether you will connect to this port via SMA or USB cable (refer to port ref3). <br> This port is intended to receive data regarding the spatial coordinate Frame clock. <br> Regulate the acquisition rate of the entire image (frame rate) (refer to port ref3).|
| Pixel dwell time      | Specify in microseconds the exposure time of each pixel to the scanner. |
| Pixel size            | Specify the size of each pixel in micrometers. |
| Harmonic content      | Setting the harmonic content value will enable you to find the right balance between resolution and accuracy in your measurements. <br>By increasing the Harmonic content value, you can enhance the resolution of your experiments, measuring even the shortest fluorescence lifetimes. <br>This field is configured during the Reference phase, and the value set at this stage will serve as a constant reference throughout the Scouting and Data phases, remaining unchanged. |
| Box width/height      | Specify the width/height of the frame to scan. |
| Number of pixel on x/y line        | Set the same value as made in Box width/Box height. |
| Offset left/right/top/bottom       | Specify the offset from the edges of the box from which to extract the images. <br> In advanced mode, check the helpfull visual representation at the bottom of the section. |

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## IMAGING RECONSTRUCTION EXPERIMENT
this section deals with more in-depth description of the imaging reconstruction experiment.

<div align="center">
    <img src="../../assets/flim-studio/imaging-experiment.png" alt="imaging-reconstruction-experiment-image">
</div>

The imaging reconstruction experiment section provides three operational modes (**REFERENCE**, ***SCOUTING***, ***DATA***), allowing a systematic approach to fine-tune experiments.

### SELECT THE REGION OF INTEREST (ROI)
 The **SCOUTING** mode allows you to explore your sample by acquiring images, enabling you to navigate through it to find your region of interest (ROI).

 You can use the scouting mode before and after the software calibration.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<a name="software-calibration"></a>

### SOFTWARE CALIBRATION

After completing the [experiment configuration](#experiment-configuration), the next step is the software calibration
(*the scouting mode is optional*).

Use the **REFERENCE** mode to calibrate the software and follow these steps:
* Place a sample with a known fluorescence lifetime on your microscope.  (ex. fluorescein, decay time: 3.6ms)
* Navigate to the upper-right corner of the interface and set the decay time in the "Decay time" input field. 
* In the same upper-right section, specify the number of frames to be captured (ex. 10) in the "Number of frame" input field.
* Begin the acquisition process by clicking the start icon, located at the top right of the interface.

The software will commence data acquisition, utilizing the predefined decay time for self-calibration. Data acquisition will automatically cease upon reaching the designated number of frames. Note that this calibration process is a one-time requirement and is not necessary for future data acquisitions.

After successful calibration, you are ready to proceed with.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### START THE DATA ACQUISITION

After completing the [software calibration](#software-calibration), the next step is the data acquisition.
Here is where effectively commence the imaging experiment by acquiring data from your sample (*replace the calibration phase sample with the sample that you want to analyze*).  

Navigate to the upper-right corner of the interface and set the number of frames to be captured (ex. 20) in the "Number of frame" input field.
Then begin the acquisition process by clicking the start icon, located at the top right of the interface.
The software will commence data acquisition and automatically cease upon reaching the designated number of frames.
When the acquisition is completed you can begin the data analysis.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### DATA ANALYSIS

Once the data acquisition is completed you can start analyzing the experiment records using the data visualization tools provided by FLIM STUDIO. (**Reconstructed image section [1]**, **TCSPC ISTOGRAMM [2]**, **Phasor plot and GMM (AI) [3]**)

<div align="center">
    <img src="../../assets/flim-studio/imaging-experiment-2-edited.png" alt="imaging-reconstruction-experiment-image">
</div>

#### RECONSTRUCTED IMAGE SECTION [1]

The section consists of four elements, listed from left to right:

1. **Photon Number Filter**: By vertically moving the two sliders, you can filter the image areas to display based on the minimum and maximum number of photons.
2. **Color Map Selector**: Clicking on the colored bar opens a selection menu where you can choose your preferred color map. The selected color map will be applied to the adjacent reconstructed image.
3. **Sample Image**: This displays the image reconstructed by the microscope, capturing photons emitted from the sample after excitation by the laser beam. The image enables visualization of the photon emission intensity in various areas of the sample.
4. **Toolbar**: From the top, you can use the following features:
      * **Magnify**: Transforms the mouse cursor into a magnifying glass. Select the magnification value and move the cursor over the reconstructed image to explore it.
      * **Zoom**: After selecting the zoom value, an enlarged version of the reconstructed image will be displayed.
      * **Unlock**: By clicking on a point of the reconstructed image, you can view its corresponding representation on the TCSPC HISTOGRAM[2]. To click on another point of the image, unlock the cursor by clicking on 'unlock'.
      * **Rectangle**: Analyzes a specific part of the image by selecting a rectangular area.
      * **Circle**: Analyzes a specific part of the image by selecting a circular area.
      * **Polyline**: Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
      * **Export**: Exports the experimental data, specifying the format (Matlab, HDF, Python, SVG).

#### TCSPC ISTOGRAMM [2]      
In this section a fluorescence intensity decay profile Istogramm is represented.  
The x-axis of the TCSPC histogram represents the time intervals following a laser pulse used to excite the sample. Each interval correlates with a certain delay after the excitation pulse, and it is within these slices of time that the photon counts are recorded.  
On the y-axis, you will find the number of photon events detected, which effectively measures the intensity of fluorescence at each time interval.  
The data plotted in the histogram spans across the period of the laser pulse. This means that the photon detection is synchronized with the periodicity of the laser.  
From the negative exponential curve of the histogram, you can deduce the fluorescence lifetime of the sample. 
By default the Istogramm represents the cumulative of each point in the sample, so the represented curve will be linear.  
<div align="center">
    <img src="../../assets/flim-studio/linear-istogramm.PNG" alt="imaging-reconstruction-experiment-image">
</div>

Otherwise moving the cursor over a specific point of the RECONSTRUCTED IMAGE[1] the graphic will show the acquired data for that specific part, resulting in a jagged line.
<div align="center">
    <img src="../../assets/flim-studio/jagged-istogramm.PNG" alt="imaging-reconstruction-experiment-image">
</div>




















