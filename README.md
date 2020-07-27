# SM2RAIN-Tool
Python code for reading SM2RAIN dataset (global daily precipitations between 2007 and 2019)
Extraction of time serie for N points.

https://zenodo.org/record/3635932#.XoWskagzZhG

The original code is amended and completed (LDU) for ...
- work with python 3.x
- process several pixels instead of just one (but also works for 1 single point)
- modify the start and end years, and allow a simple copy and paste of the file name in Windows format (otherwise backslash is interpreted as a check character)
- calculate monthly totals
- extract daily and monthly data into a text file
- (for fun) lengthen the time axis of the graphics and improve their aesthetics using the "seaborn" library (and add an interactivity menu to them, but does not work)

Tutorial:
- place consecutive SM2RAIN annual files in the same folder (1 file per year from 2007 to 2019)
- rename the files if necessary when the version number varies depending on the year, which is not dealt with in the code
- copy-paste the name of the working folder in the "path" variable of the code
- enter the start and end year in the year_start and year_end variables
- enter the geographic coordinates of the pixels to extract in the lonlat_.txt file
- Launch the script and wait until the end of the processing which takes about ten seconds or more depending on the number of pixels
