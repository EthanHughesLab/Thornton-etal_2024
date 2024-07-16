# Thorntonetal-2024
Code related to data analysis in the paper: Thornton, MA, Futia, GL, Stockton, ME, Budoff, SA, Ozbay, BN, Ramirez, AN, Tzang, O, Kilborn, K, Restrepo, D, Gibson, EA, and Hughes, EG (2024) Long-term in vivo three-photon imaging reveals region-specific differences in healthy and regenerative oligodendrogenesis. Nature Neuroscience 27(5): 846-861. 

The code requires three data columns: 1) imaging depth in microns, 2) the average power at the surface (mW) for each z-slice, and 2) an approximation of signal at each plane, for example the mean intensity of the top 1% of pixels in an ROI. The top n % pixels was measured using the ImageJ macro "mean_of_brightest_n_pixels_v105.ijm" that is available from the NYU Langone Imaging Core and Michael Cammer, at https://microscopynotes.com/imagej/. An example data from a 1000 micron z-volume in 2 month-old mouse is included as "Example_data.xslx"

The plotted power vs. depth curve is a recommendation for initial settings only. Results / phototoxicity may vary by system for a number of different reasons. 
