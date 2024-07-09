# EEG analysis with MNE

## Available Information/Courses: 
The best comprehensive online course for EEG neuroimaging is https://neuraldatascience.io/intro.html. 
It is accompanied by a YouTube page with incredible explanatory videos: https://www.youtube.com/playlist?list=PLtfEWMIgWS22MMZjPIzBRE2cHhMcvEKwp 

![Example Video](https://www.youtube.com/playlist?list=PLtfEWMIgWS22MMZjPIzBRE2cHhMcvEKwp)

## Other Neuroimaging online courses (some reference fMRI) 
- https://neuroimaging-data-science.org/root.html  
- https://dartbrains.org/content/intro.html  
- https://web.mitsgwalior.in/academics/quality-initiatives/mits-moocs?view=article&id=767&catid=2 A video course on EEG analysis  
- https://github.com/TUIlmenauAMS/ADSP_Tutorials 
* https://andysbrainbook.readthedocs.io/en/latest/ is a comprehensive neuroimaging handbook for MRI/fMRI analysis.
----------------------------

# Some Notes on EEG:
## EEG: What is EEG? 
Scalp electroencephalography (EEG) was invented around 100 years ago by Hans Berger and has provided a great method of inspecting the electrical signatures of neural activity, more on its history is found in Stone & Hughes, 2013 [1]. Topical overviews of the tool can be found at https://info.tmsi.com/blog/what-is-eeg and https://en.wikipedia.org/wiki/Electroencephalography. A more technical perspective with a wealth of resources can be found here http://www.scholarpedia.org/article/Electroencephalogram. Take a deep dive into what the EEG signal means, what is the signal we are recording, and where it comes from in Cohen, 2017 [2] and considerations of confounding factors are found in Burle et al., 2015 [3]. A Nature review article detailing the major electrophysiological recordings can be found in Buszaki et al., 2012 [4]. 

A great video on the matter can be found here: 

![EEG Video](https://www.youtube.com/watch?v=Bmt89hHyxuM&lc=UgxtrqTbC1Mb3w8VtbN4AaABAg&ab_channel=MikeXCohen)

## EEG Preprocessing  
A mind map of EEG neuroimaging processing can be found here (https://artemis.incf.org/). It is debated how much cleaning or processing should be performed on EEG signals. Raw EEG is confounded by many artifacts, listed above, that bias our signal (intended activity to capture) and can introduce noise (unintended signal). This can be eye movements, head movements, heartbeat, surrounding electrical noise, and much more. On the other hand, we do not want to over-clean our signal and inadvertently remove the signal we intended to inspect. A list of methods of reducing noise in EEG signals can be found here: https://mentalab.com/reduce-noise-in-eeg-recordings/. A great article on this can be found in Delorme, 2023 [7].

## Common Terms 	 
Common EEG terms like frequency, frequency bands (delta, theta, alpha and beta), voltage, morphology, synchrony, periodicity, electrodes, impedance, positions, montage, artifacts and filtering can be found here: https://www.medicine.mcgill.ca/physio/vlab/biomed_signals/eeg_n.htm

## Waveforms 
Information from EEG is presented as a time series, a sequence of points indexed over time, and it represents a collection of waves (segmented patterns in time series) that reflect typical and non-typical brain activity, also called morphology. A non-exhaustive list of waves/waveforms can be found in Nayak & Anilkumar, 2023 [6],  

- To explore: Burst Suppression, GDP: Giant Depolarizing Potential, N2, P3 waveforms...
  
# Signal Considerations  
For the brain, an electrochemical communicating system, EEG is a tool that provides a good balance between temporal and spatial resolutions, given the EEG has enough channels to map the cerebral cortex for its spatial capabilities. Scalp EEG captures activity from the cerebral cortex. An interesting stack exchange discusses the accepted physiological models of the cortex in which this signal originates https://biology.stackexchange.com/questions/29759/is-the-six-layer-cortex-model-of-the-mammalian-cortex-still-the-most-accepted-mo (this can be complemented by the consideration of Buzsaki et al., 2012. Spatial resolution of EEG signal can be augmented using multimodal imaging with MRI where one can perform **source localization**. This technique uses structural images from MRI to map the electrodes on the brain to infer the spatial origins of the signals, more can be found in Eom, 2023 [5]. 

# References 
[1] Stone, J. L., & Hughes, J. R. (2013). Early history of electroencephalography and establishment of the American Clinical Neurophysiology Society. Journal of Clinical Neurophysiology, 30(1), 28-44.   

[2] Cohen, M. X. (2017). Where does EEG come from and what does it mean?. Trends in neurosciences, 40(4), 208-218 

[3] Burle, B., Spieser, L., Roger, C., Casini, L., Hasbroucq, T., & Vidal, F. (2015). Spatial and temporal resolutions of EEG: Is it really black and white? A scalp current density view. International journal of psychophysiology: official journal of the International Organization of Psychophysiology, 97(3), 210–220. 

[4] Buzsáki, G., Anastassiou, C. A., & Koch, C. (2012). The origin of extracellular fields and currents--EEG, ECoG, LFP and spikes. Nature reviews. Neuroscience, 13(6), 407–420. https://doi.org/10.1038/nrn3241 

[5] Eom T. H. (2023). Electroencephalography source localization. Clinical and experimental pediatrics, 66(5), 201–209. https://doi.org/10.3345/cep.2022.00962 

[6] Nayak, C. S., & Anilkumar, A. C. (2023). EEG Normal Waveforms. In StatPearls. StatPearls Publishing. 

[7] Delorme, A. EEG is better left alone. Sci Rep 13, 2372 (2023). https://doi.org/10.1038/s41598-023-27528-0 

[8] Lynn, S. K., & Barrett, L. F. (2014). "Utilizing" signal detection theory. Psychological science, 25(9), 1663–1673. https://doi.org/10.1177/0956797614541991 
