## HW6

![bad plot](https://github.com/bflaggs/DSPS_BFlaggs/blob/main/HW6/wavefront_badplot_original.jpg "Original Bad Plot")

![good plot](https://github.com/bflaggs/DSPS_BFlaggs/blob/main/HW6/wavefront_gootplot_updated.jpg "Updated Good Plot")

The original plot suffers from both an odd color scaling map for the SNR values and an odd scaling of the SNR in general since the SNR values are quite large. To fix this issue I changed the color scaling map from the default `viridis` color map (which is a color map looping through several colors with different shades) to the `Blues` color map (which is a color map on shaowing a blue gradient). Applying this change makes it easier to see which antennas have larger SNR values compared to other antennas.

Additionally, I changes the color map to show the log base 10 of the SNR values rather than just the plain SNR values. This change was made because the SNR values were large making the color map labels not pleasant to look at since the values on the tick marks ranged from about 10000 to 40000. Applying this change improves the readability of the color map.

Furthermore, I also changed the legend to be more specific in describing what each data point represents and updated the font size of everything. Here a single data point represents data for a single antenna which was not clear in the original plot but is much more explicit in the updated plot. Also, updating the font size should improve readability (especially if these plots were to be published in a paper or on a poster).

## Questions
1. This homework was used to show how to look at a plot and see what could be improved to make the plot follow the plotting best practices. This homework also showed students how to implement some of these best plotting practices for future use.
2. The hardest part of this homework for me was trying to find a plot of mine to improve (my advisor typically likes to have presentation worthy plots immediately so I did not have many "bad" plots).
3. The easiest part of this homework for me was making the plots look better/cleaner.
4. One new thing I learned was that the keyword `cmap` in the `plt.scatter` function will allow you to change the color scaling map for the color map.
