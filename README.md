# Baylor-Competition
Code used for the preliminary round of the 2023 AXS NCSAC hosted by Baylor University

In this code, I cleaned a dataset of BIG12 CBB tracking data provided by competition organizers. 

I then attempted to create multiple models to find out if shot outcome could be predicted by play components and game state data. 

After attempting, many logit, ordered logit models, and random forest models, I settled on a random forest model (called last_rf_model) 
to predict made 2 pointer, missed 2 pointer, made 3 pointer, and missed 3 pointer. Upon training and testing this model, this random forest had an accuracy 
of about 53.5% which was interesting because the model did not take shot location, player or team talent into account. Model diagnostics such as ROC curves and 
variable importance charts were also created for this model.
