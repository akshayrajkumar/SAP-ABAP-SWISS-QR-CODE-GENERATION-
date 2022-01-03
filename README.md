# SAP-ABAP-SWISS-QR-CODE-GENERATION-
To Create QR code for SWISS Market with Swiss Cross by superimposing the Swiss Cross Image with  QR Image in Smartforms
create a global class with the methods that is shown in the image CLASS_METHODS.
Use the method GET_QR_STRING to GEnerate the Data that is supposed to be displayed in the QR and then pass it to the method GET_QRIMAGE as input.
Create the methods with Parameters as shown in the images with _PARAMS in the upload sections
once the qr string is generated pass it to METHOD GET_QRIMAGE where you get the QR CODE with the data generated is converted as Image and uploaded into BDS with the name that is mentioned inside the CONSTRUCTOR.
the placement of the logic should be before calling the Smartforms and after the smartform call the method DELETE_QR_BITMAPS_BDS is called to delete the uploaded image to avoide unwanted memory that is stored in the system
And in the smartform create two windows as secondary window for QR image and SWISS CROSS image respectively.
Follow the dimensions and positioning of the images as provided in the Screenshot swiss_qr_image and Swiss_cross and superimpose the image swiss_cross on swiss QR.
