# zebra-mussel-ai

Zebra mussels (Dreissena polymorpha) are an invasive species that have spread through the Great Lakes via shipping vessels and caused enviornmental damage. The goal of this model is to be able to detect zebra mussels on ships and identify vessels that may be unwittingly spreading the invasive species. Since there are no major dataset on zebra mussels, I've replaced them with barnacles as a proof of concept. 

This project is based on two datasets:

* For the barnacles: Cortlandd/barnacle-images on github https://github.com/Cortlandd/barnacle-images

* Other marine life: Sea animals image dataset: https://www.kaggle.com/datasets/vencerlanz09/sea-animals-image-dataste 

The goal is to train a model to differentiate between barnacles and other sea life. If it can do this, it will likely be able to identify similarly shaped zebra mussels once the data is available. 

The data has been uploaded to FiftyOne and inspected for quality. The next steps are to segment the data into train/test/validate segments and train the model. 

I chose to use the YOLOv8n-cls classification model from Ultralytics because it should be able to classify the different types of marine life successfully. 
