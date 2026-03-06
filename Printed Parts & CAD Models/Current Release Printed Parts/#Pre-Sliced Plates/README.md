# Pre-Sliced Plates
Hey, these plates aren't updated as often as the other folders are.

While these are here for convenience, we ask that you read through the other folders and update your parts accordingly.

Thank you.

# Before Printing - CALIBRATION
ABS and similar materials are prone to shrinking, changing the dimensions of the printed part from the original design.  If you have too much shrinkage, holes may not line up for screws, and parts may interfere with others.

We strongly recommend first printing the Calibration Test piece `calibration_test_200x30mm.stl` (Printed Parts & CAD Models\Calibration\) at 100% scale in the recommended print settings.

Measure the printed part (ideally with at least inexpensive calipers).  Input the length of the part into the formula below to get your shrinkage scale percentage:

Scale Percentage = (200 / measured_length) * 100

Example: 
Printed calibration piece measured 198.2mm in length.
Scale Percentage = (200 / 198.2) * 100
Scale Percentage = 100.9%

**Use this updated scale for the rest of the printed parts. Scale all other printed parts for this project in X/Y/Z by this value.  This applies to THIS filament on THIS printer!  You may want to repeat this test if you're using a different filament brand or type for the accent pieces.**

NOTE: The 3mf files in the **\#Pre-Sliced Plates folder** default to 101% scale.  This may or may not be appropriate for your printer!  Select all the parts and change the scale to the scale percentage you determined above before slicing.