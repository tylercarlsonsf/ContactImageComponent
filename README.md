# Contact Image Component

Lightning component to add a nice looking contact image and contact name to lightning record page, useful for story driven demos where the contact is a defined persona with an image.

[![Deploy](https://deploy-to-sfdx.com/dist/assets/images/DeployToSFDX.svg)](https://deploy-to-sfdx.com/)


### Instructions:

- Add the component to the Lightning record page for contact
- The component will default to blank "placeholder image", there is a picker attribute called "Contact Image URL Override" that can be used to choose from some sample images, selecting “none” will use the Contact_Picture_URL__c field from each contact to display the img
- Sample Images are included, if you select any of these in the override drop down it will override the Picture_URL__c field and hard code the image for all contact records, these are mostly there to test, but the static resource links can be used for individual contacts too, more on that below.
    * Blank - static resource url: /resource/LightningContactImage/LightningContactImage/Blank.png
    
    * Male1 - static resource url: /resource/LightningContactImage/LightningContactImage/Male1.png
 
    * Male2 - static resource url: /resource/LightningContactImage/LightningContactImage/Male2.png
   
    * Male3 - static resource url: /resource/LightningContactImage/LightningContactImage/Male3.png

    * Female1 - static resource url: /resource/LightningContactImage/LightningContactImage/Female1.png
 
    * Female2 - static resource url: /resource/LightningContactImage/LightningContactImage/Female2.png


* To add a custom image for individual contacts, add the Contact_Picture_URL__c field to the contact page layout and enter the URL you would like to use. This is where the resource links above come in handy, you can copy paste these into Picture URL fields for a few contacts you will use in your demo instead of having to get your own images

* you can use any image URL you want in this field, but the image should be have a 1x1 (square) aspect ratio
* If you want to use a custom image url then make sure you set the attribute "Contact Image URL Override"  in the lightning component to "none”



