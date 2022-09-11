This project aimed at building an interpretable framework to integrate toxic language annotations. Most data sets address only one aspect of the complex relationship in toxic communication and are inconsistent with each other. Enriching annotations with more details and information is, however, of great importance in order to develop high-performing and comprehensive explainable language models. Such systems should recognize and interpret both expressions that are toxic as well as expressions that make reference to specific targets to combat toxic language. We, therefore, create a crowd-annotation task to mark the spans of words that refer to target communities as an extension of the HateXplain data set. We presented a quantitative and qualitative analysis of the annotations. We also fine-tuned RoBERTa-base on our data and experimented with different data thresholds to measure their effect on the classification. The F1-score of our best model on the test set is 79%. The annotations are freely available and can be combined with the existing HateXplain annotations to build richer and more complete models. For more information, you can refer to our paper via the link below:<br>
example_link<br><br>
Colab notebooks contain the codes for fine-tuning RoBERTa-base langauge models with different threholds on the training set and obtaining the predictions on the test set that have been created with a fixed UQS threshold (50)<br>
-UQS threshold = 50: https://colab.research.google.com/drive/143tvkcNAPd7bbr4vVAIznHc1lBHy6G-q?usp=sharing<br>
-UQS threshold = 60: https://colab.research.google.com/drive/1J4av7UrmIIUUA5-WG4jEYH6UMy4xPJS0?usp=sharing<br>
-UQS threshold = 70: https://colab.research.google.com/drive/1b7hVVTxA67cGiTKaae9VrrUrq5vR4NEG?usp=sharing<br><br>
Fine-tuned models on Hugging Face:<br>
-UQS threshold = 50: BBarbarestani/RoBERTa_HateXplain_Target_Span_Detection_UQS_Threshold_50_2_Previous_Hyperparameters<br>
-UQS threshold = 60: BBarbarestani/RoBERTa_HateXplain_Target_Span_Detection_UQS_Threshold_60_2<br>
-UQS threshold = 70: BBarbarestani/RoBERTa_HateXplain_Target_Span_Detection_UQS_Threshold_70_2<br><br>
Files needed for designing the annotation task on LingoTURK (Please visit https://github.com/FlorianPusse/Lingoturk for more information.):<br>
1- /app/views/ExperimentRendering/TargetSpanDetectionbExperiment/TargetSpanDetectionExperiment_render.html<br>
2- /public/javascripts/ExperimentRendering/TargetSpanDetectionbExperiment/TargetSpanDetectionExperiment_render.js<br>
3- /app/models/Questions/ExperimentRendering/TargetSpanDetectionbExperiment/experiment.properties<br>
4- /app/models/Questions/ExperimentRendering/TargetSpanDetectionbExperiment/fields.json<br>
5- /app/models/Questions/ExperimentRendering/TargetSpanDetectionbExperiment/resultQuery.sql<br><br>
