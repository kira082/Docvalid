#Documents  Validation
Python backend API to extract text information from a Passport,Visa and Emirates image file.
#IMPORTANT NOTICE
SCANNING IDENTITY DOCUMENTS IS IN MOST CASES RESTRICTED BY LAW. OBSERVE THE APPLICABLE LAWS USING THIS TOOL. THE COPYRIGHT HOLDER IS NOT IN ANY WAY LIABLE FOR UNLAWFUL USAGE OF THIS TOOL. 
#Prerequisite
First of all, make sure you have  SAP Cloud foundry Command line and python   installed in your system.
Required Packages
Opencv-python
Flask
Passporteye
Pytesseract
Tesseract-OCR
 
#Quickstart
Just clone the repo and build the app with cloud foundry.
Install the require packages using python requirements.txt
For Running the application 
python app.py
For Deploy  the application on SAP Cloud Platform 
cf push app_name
 
Endpoint http://0.0.0.0:4000
This is the only one endpoint of this app and accept one POST parameter :
imagefiles : An image files of the passport,visa and emirates.
A sample response:
{
    "country": "Madagascar",
    "country_code": "MDG",
    "first_name": "Patrick",
    "last_name": "RANDRIA",
    "nationality": "Madagascar",
    "number": "X00X00000",
    "sex": "M"
}
 

