# Thorntonetal-2024
Code related to data analysis in the paper: Thornton, MA, Futia, GL, Stockton, ME, Budoff, SA, Ozbay, BN, Ramirez, AN, Tzang, O, Kilborn, K, Restrepo, D, Gibson, EA, and Hughes, EG (2024) Long-term in vivo three-photon imaging reveals region-specific differences in healthy and regenerative oligodendrogenesis. Nature Neuroscience 27(5): 846-861. 

The code requires three data columns: 1) imaging depth in microns, 2) the average power at the surface (mW) for each z-slice, and 2) an approximation of signal at each plane, for example the mean intensity of the top 1% of pixels in an ROI. The top n % pixels was measured using the ImageJ macro "mean_of_brightest_n_pixels_v105.ijm" that is available from the NYU Langone Imaging Core and Michael Cammer, at https://microscopynotes.com/imagej/. 

Open the three-photon image in Imagej, drag "mean_of_brightest_n_pixels_v105.ijm" macro to the toolbar, set “var topn = “ to whatever top percentage of pixels you want to measure. For a 256x256 ROI, 0.01 * (256x256) = 655. Draw an ROI, use the t-key to add to the ROI Manager, and then run the macro. The results file is saved in the directory of the original image. 

For the analysis code, set the rep rate of the laser, filepath, cortex_top, and white_matter_top in micron. Do not include any autofluorescent signal from the meninges / surface of the cranial window prep. 

An example data from a 1000 micron z-volume in 2 month-old mouse is included as "Example_data.xslx"

The plotted power vs. depth curve is a recommendation for initial settings only. Results / phototoxicity may vary by system for a number of different reasons. 


