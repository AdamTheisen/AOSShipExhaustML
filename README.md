# AOSShipExhaustML
Python script for downloading and aplying a machine learning technique with scikit-learn to the Atmospheric Radiation Measurement User Facility (ARM) MARCUS CPC data in order to detect ship exhaust.  This script uses the ARM Live Data Web Service to automatically download all the MARCUS CPC data.

An account with the ARM Live Data Web Service is required and a token.json file with the structure of 

{
    "username": "your_username",
    "token": "your_token"
}
