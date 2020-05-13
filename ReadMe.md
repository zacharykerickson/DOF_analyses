# DOF_analyses

In order to see the HTML rendered put the following at the beginning of the URL: https://htmlpreview.github.io/?
Example: https://htmlpreview.github.io/?https://github.com/zacharykerickson/DOF_analyses/blob/master/do_analysis_MODIS_Rrs_logged_2008.html
(Or follow the links below; note sometimes Firefox doesn't render them but in my experience Chrome always does)

Analyses done for MODIS and SeaWiFS data (at 9 km resolution). So far up here I have average 2008 values, and only for ocean depth >1 km. PC analysis is done for both raw and logged data (log10), note that for the GIOP analysis the backscatter power-law slope s is bounded between 0 and 2; for the logged version I used log10(2-s).

PC analysis is done after subtracting the mean for each variable and dividing by the (assumed) noise of each variable. I then use a method from Gavish and Donohe (2014) to compute the estimated noise on the final result, which includes information of the rank of the data matrix and the median singular value. Values of this estimated noise close to 1 means that this analysis suggests that the (assumed) noise already used appears to be correct; far from one means that this assumed noise does not appear to be correct.

Another option, for the Rrs data, is to subtract the mean for each spectrum and divide by the (assumed) noise, which in this case must be a constant value (not depending on wavelength). These are denoted by the "\_transpose" addition to the filename, or in the links below by "^T".

| Platform | Time | Data | Regular | Logged |
| --- | --- | --- | --- | --- |
| MODIS | 2008 | R_rs | [file](https://htmlpreview.github.io/?https://github.com/zacharykerickson/DOF_analyses/blob/master/do_analysis_MODIS_Rrs_2008.html) [file^T](https://htmlpreview.github.io/?https://github.com/zacharykerickson/DOF_analyses/blob/master/do_analysis_MODIS_Rrs_transpose_2008.html) | [file](https://htmlpreview.github.io/?https://github.com/zacharykerickson/DOF_analyses/blob/master/do_analysis_MODIS_Rrs_logged_2008.html) [file^T](https://htmlpreview.github.io/?https://github.com/zacharykerickson/DOF_analyses/blob/master/do_analysis_MODIS_Rrs_logged_transpose_2008.html) |
| MODIS | 2008 | GIOP | [file](https://htmlpreview.github.io/?https://github.com/zacharykerickson/DOF_analyses/blob/master/do_analysis_MODIS_giop_2008.html) | [file](https://htmlpreview.github.io/?https://github.com/zacharykerickson/DOF_analyses/blob/master/do_analysis_MODIS_giop_logged_2008.html) |
| MODIS | 2008 | chlor_a, pic, poc, Kd_490, flh | [file](https://htmlpreview.github.io/?https://github.com/zacharykerickson/DOF_analyses/blob/master/do_analysis_MODIS_anc_2008.html) | [file](https://htmlpreview.github.io/?https://github.com/zacharykerickson/DOF_analyses/blob/master/do_analysis_MODIS_anc_logged_2008.html) |
| SeaWiFS | 2008 | R_rs | [file](https://htmlpreview.github.io/?https://github.com/zacharykerickson/DOF_analyses/blob/master/do_analysis_SeaWiFS_Rrs_2008.html) | [file](https://htmlpreview.github.io/?https://github.com/zacharykerickson/DOF_analyses/blob/master/do_analysis_SeaWiFS_Rrs_logged_2008.html) |
| SeaWiFS | 2008 | GIOP | [file](https://htmlpreview.github.io/?https://github.com/zacharykerickson/DOF_analyses/blob/master/do_analysis_SeaWiFS_giop_2008.html) | [file](https://htmlpreview.github.io/?https://github.com/zacharykerickson/DOF_analyses/blob/master/do_analysis_SeaWiFS_giop_logged_2008.html) |
| SeaWiFS | 2008 | chlor_a, pic, poc, Kd_490 | [file](https://htmlpreview.github.io/?https://github.com/zacharykerickson/DOF_analyses/blob/master/do_analysis_SeaWiFS_anc_2008.html) | [file](https://htmlpreview.github.io/?https://github.com/zacharykerickson/DOF_analyses/blob/master/do_analysis_SeaWiFS_anc_logged_2008.html) |

