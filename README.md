# AOSShipExhaustML
Python script for downloading and aplying a Random Forest Classifier with scikit-learn to the Atmospheric Radiation Measurement User Facility (ARM) MARCUS CPC data in order to detect ship exhaust.  A time-series difference is applied to the CPC concentration before training the ML algorithm on data manually flagged as good/bad using time periods identified as ship exhaust with the DQ Zoom tool.  This script uses the Atmospheric data Community Toolkit (ACT) and the ARM Live Data Web Service to automatically download all the MARCUS CPC data.

An account with the ARM Live Data Web Service is required and a token.json file with the structure of 

{
    "username": "your_username",
    "token": "your_token"
}

NOTE: A majority of the AOS instruments were tested as part of the devlopment of this ML effort.  The CPC alone provided the best results when inspecting the data.  It is not perfect, but the user can adjust the settings to tailor it to their needs/preferences.
