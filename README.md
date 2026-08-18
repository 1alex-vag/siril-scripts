# siril-scripts
Siril Scripts by ag_astrophotography

A collection of custom Siril processing scripts and tools for astrophotography.

Built and tested for Siril 1.4.x / 1.4.4 Stable.

Included tools

2xDrizzle Mono

Automated mono preprocessing with true 2× HST Drizzle.

Includes calibration, registration, drizzle and final stacking.

Typical folder structure:

biases/
darks/
flats/
lights/

A version using already existing master calibration files is also available.

⸻

2xDrizzle OSC

Automated preprocessing for One Shot Color / Bayer CFA cameras with true 2× CFA Drizzle.

Important:

The OSC data stays undebayered until the drizzle step.

Includes:

* Bias calibration
* Dark calibration
* Flat calibration
* CFA-aware cosmetic correction
* 2-pass registration
* 2× Bayer Drizzle
* Final RGB stack

Both a Full and a FromMasters version are included.

⸻

Astro Channel Processor

A Siril-native Python tool for automatically registering and combining mono channels.

Supported channels:

* L
* R
* G
* B
* Ha
* OIII
* SII

Features:

* Native Drag & Drop
* Automatic or manual registration reference
* Save all registered channels
* Create RGB
* Create LRGB
* Create SHO
* Create HOO
* Save luminance separately
* Open finished results directly in Siril
* Dark PyQt6 interface
* Color-coded channel panels

⸻

OSC Channel Extractor

A Siril-native tool for extracting channels from a finished RGB image.

Available functions:

* Extract L
* Extract R
* Extract G
* Extract B
* Extract RGB
* Extract ALL

Output example:

Extracted/
├── L_extracted.fit
├── R_extracted.fit
├── G_extracted.fit
├── B_extracted.fit
└── RGB_original.fit

Extracted files can also be opened directly in Siril.

⸻

Installation

SSF scripts

Copy the .ssf file into:

C:\Program Files\Siril\scripts

Administrator privileges may be required.

Restart Siril afterwards.

The script should then appear under:

Scripts
→ SIRIL Script Files

Python scripts

The provided ZIP packages include:

INSTALL_TO_SIRIL.bat

Extract the ZIP and run the installer.

The installer copies the script to:

C:\Program Files\Siril\scripts

Restart Siril afterwards.

The tool should then appear under:

Scripts
→ Python Scripts

Requirements

* Siril 1.4.x
* Tested primarily with Siril 1.4.4 Stable
* Windows

Python tools use Siril’s own Python environment and sirilpy.

PyQt6 is automatically installed into Siril’s Python environment if required.

Notes about Drizzle

Drizzle works best with properly dithered data.

For 2× drizzle, the output image contains approximately four times as many pixels as the original frame, so RAM and disk usage increase significantly.

Current drizzle settings use:

Scale:   2×
Pixfrac: 0.7
Kernel:  square

These settings are intended as a robust general-purpose starting point.

Author

Created by ag_astrophotography

Astrophotography, software experiments and custom Siril workflows.

Feedback

Testing, bug reports and suggestions are welcome.

If you encounter a problem, please include:

* Siril version
* Script/tool version
* Screenshot of the error
* Relevant Siril console output

Disclaimer

These scripts are provided as experimental astrophotography tools.

Always keep backups of your original data.

Original FITS files are not intentionally modified by the Python tools; temporary working copies are used during processing.
