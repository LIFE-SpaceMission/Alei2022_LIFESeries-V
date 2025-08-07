# Large Interferometer For Exoplanets (LIFE) V. Diagnostic potential of a mid-infrared space interferometer for studying Earth analogs


  
Cloud- and cloud-free spectra of the Earth in time used as input for the retrievals in LIFE IV  (Alei et al. 2022;A&A 665, A106). 

Link to paper: 		https://doi.org/10.1051/0004-6361/202243760

  
Original spectra are from Rugheimer and Kaltenegger (2019). Spectra were then scaled at the observer's distance and ran through LIFEsim. 

All spectra assume the Earth to orbit a G2V star (Sun-like) on a circular 1AU orbit   
at a distance of 10pc from the observer.  
  
  
## Description of the directory:  
  
  
- `NoisySpectra/`  
	Contains the 8 cloudy and cloudfree LIFEsim spectra used in the retrievals (Figure 1 in publication) at R=50 and SNR=10.

  

## Structure of the filenames:  
     
  
```  
Sun_<Epoch>_TOA_<cloud-coverage>_10pc_R50_SNR10_wlen4_18.5_3exo.txt  
```  
  
  
- **Epoch**   
   Epoch of the model. Possible values:  
      - `Prebiotic_3.9Ga`: Prebiotic Earth at 3.9 Ga.  
      - `GOE_2.0Ga`: Earth at the Great Oxygenation Event (GOE) at 2.0 Ga.  
      - `NOE_0.8Ga`: Earth at the Neoproterozoic Oxygenation Event (NOE) at 0.8 Ga.  
      - `Modern`: Modern Earth.
- **cloud-coverage**  
   Cloud coverage of the model. Possible values:  
      - `clearsky`: cloudfree model.   
      - `cloudsky`: cloudy model.
  
  
## Structure of the files:  
  
Each file contains the following 3 columns:  
  
  
``` 
	First Column      Second Column         Third Column           
	Wavelengths      Flux at 10 pc       Noise on Flux at 10 pc  
	[micron]       [erg s-1 Hz-1 m-2]     [erg s-1 Hz-1 m-2]
      
```