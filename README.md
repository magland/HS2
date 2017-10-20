# HerdingSpikes
## Spike detection, localisation and sorting for high density MEAs

This class provides a simple interface to the detection, localisation and
clustering of spike data from dense multielectrode arrays according to the
methods described in the following papers:

Muthmann, J. O., Amin, H., Sernagor, E., Maccione, A., Panas, D.,
Berdondini, L., ... & Hennig, M. H. (2015). Spike detection for large neural
populations using high density multielectrode arrays.
Frontiers in neuroinformatics, 9.

Hilgen, G., Sorbaro, M., Pirmoradian, S., Muthmann, J. O., Kepiro, I. E.,
Ullo, S., ... & Murino, V. (2017). Unsupervised spike sorting for
large-scale, high-density multielectrode arrays.
Cell reports, 18(10), 2521-2532.

## Compilation of Cython code
```
cd detection_localisation
python3 setup.py build_ext --inplace
cd ..
```
Yes, you need to `cd`.


## Examples

Example data for the NeuroPixel array are on theia:
* A short sample is here: ``/disk/scratch/mhennig/neuropixel/data/rawDataSample.bin``
* This is a whole 60 minute recording: ``/disk/scratch/mhennig/neuropixel/data/Hopkins_20160722_g0_t0.imec.ap_CAR.bin``

Example data for the 3Brain Biocam array are on theia in:
``/disk/scratch/mhennig/P29_16_07_14/P29_16_05_14_retina02_left_stim3_fullarray_fullfieldHDF5.brw``

A tutorial on how to reproduce the workflow is in the localised_spikes_clustered Jupyter notebook.
