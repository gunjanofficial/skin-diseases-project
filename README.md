# skin-diseases-project
I have built is model with  the help of machine learning algorithms .where doctors can identify skin diseases at an early stage, allowing for prompt treatment initiation and better prognosis.
Businesscase:
Create a predictive model using machine learning techniques to predict the various classes of skin disease.

# Domain Analysis:
This database contains 34 attributes, 33 of which are linear valued and one of them is
nominal.

The differential diagnosis of erythemato-squamous diseases is a real problem in dermatology.

They all share the clinical features of erythema and scaling, with very little differences. 

The diseases in this group are psoriasis, seboreic dermatitis, lichen planus, pityriasis rosea, cronic dermatitis, and pityriasis rubra pilaris.

Usually a biopsy is necessary for the diagnosis but unfortunately these diseases share many
histopathological features as well. 

Another difficulty for the differential diagnosis is that a disease may show the features of another disease at the beginning stage and may have the characteristic features at the following stages.

Patients were first evaluated clinically with 12 features. Afterwards, skin samples were taken for the evaluation of 22
histopathological features. 

The values of the histopathological features are determined by an analysis of the samples under a microscope.

In the dataset constructed for this domain, the family history feature has the value 1 if any of these diseases has been
observed in the family, and 0 otherwise. 

The age feature simply represents the age of the patient. 

Every other feature (clinical and histopathological) was given a degree in the range of 0 to 3. Here, 0 indicates that the feature was not present, 3 indicates the largest amount possible, and 1, 2 indicate the relative intermediate values.

# Data Analysis Report
I have used 6 models for skin disorder prediction and we can see in model_dataframe where all models name have been listed with accuracy score ,f1 score and after hyperparameters accuracy score.In this model dataframe we can see Decision Tree Classification has got maximum accuracy score as 98.91% as compareed to other algorithms and the error rate is vey less as 1.09%.So we can say that decision tree classification model is performing very good for prediction and this moder will be best for skin diseases prediction of the patient at the earliest.¶
# Suggestions to the Doctors to identify the skin diseases of the patient at the earliest.
In Bivaraite analysis, I have analyzed the relationship between the independent features with target feature and some feature are very correrated with each other and Extract the insight from data which are very usedfull to undestand the skin disease class.

Below is the symptom wise analysis for diseases with clear symptoms based on clinical and histopathological data analysis.

class 1(PSORIASIS) : Above graph evaluation indicates higher intermediate value of features in patient with erythema, scaling,definite_borders,knee_and_elbow_involvement,scalp_involvement,pnl infiltrate,acanthosis,parakeratosis,clubbing and elongation of rete ridges thinning of suprapappilary epidermis,disappearance of granular layer,inflammatory mononuclearfiltrates. ALONGWITH DEGREE ZERO(0) means most without feature of itching,koebner phenomenon,polygonal papules,follicular papules,oral mucosal volvement, melanin incontinence and FAMILY HISTORY, perifollicular parakeratosis are more likely to have CLASS (1)disease i.e.PSORIASIS.

class 2(SEBOREIC DERMATITIS): Above graph evaluation indicates that patient with higher intermediate value of erythema,scaling,itchig,exocytosis, acanthosis and spongiosis alongwith ALONGWITH DEGREE (0) means most without feature of Koebner phenomenon,follcular papules,knee and elbow involvement,FAMILY HISTORY,scalp involvement,melanin incontinence etc are more likely to have CLASS (2)SEBOREIC DERMATITIS.

CLASS 3(LICHEN PLANUS): Above graph evaluation indicates that patient with higher intermdiate value of Erythema,Scaling, Definite Borders,itching, polygonal papules,oral mucosal involvememnt,acanthosis,inflammatory mononuclear filtrates ALONGWITH most Without any feature i.e.DEGREE(0) of follicular papules, knee and elbw involvement,scalp involvement,FAMILY HISTORY,hyperkeratosis,thinning of sprapappilary epidermis,spongiform pustule, munro microabscess are more likesly to have CLASS 3(LICHEN PLANUS)

CLASS 4(PITYRIASIS): Above graph evaluation indicates that patient with higher intermediate value of Erythema,Scaling,exocystosis,,Acanthosis,Spongiosis, Inflammatory Mononuclear Filtrate Alongwith most Without any feature of i.e.(DEGREE 0) of Itching,knee and elbow involvement,scalp involvement,FAMILY HISTORY,Pnl infiltrate,hyperkeratosis,clubbing and elongation of rete ridges, thinning of suprapappilary dermis are more likly to have CLASS 4(PITYRIASIS)

CLASS 5(CHRONIC DERMATITIS): Above graph evaluation indicates that patient with higher intermediate value of Erythema,Scaling, Itching,Acanthosis,Elongation of rete ridges alongwith most Without any feature i.e.(DEGREE 0) Of Koebner phenomenon,Knee and Elbow involvement,scalp involvement,FAMILY HISTORY,Pnl infiltrate,Clubbing of rete ridges,thinning of suprapappilary epidermis and disappearance of granular layer are more likely to have CLASS(5) CHRONIC DERMATITIS

CLASS 6(PITYRIASIS RUBRA): Above graph evaluation indicates patient with higher intermediate value of Erythema,Scaling, Exocystosis,Acanthosis,Parakertosis,knee and elbow involvement Follicular Horn plug,inflammatory Mononuclear Filtrate Alongwith most without any feature(DEGREE 0) of Koebner phenomenon, Polygonal papules,oral mucosa involvement, scalp involvement, eosinophils in filtrate,elongation of rete ridges and Thinning of suprappilary dermis are more likely to have CLASS 6 (PITYRIASIS RUBRA).

# Challenges faced Duraing implementation:
This dataset have 35 columns features and 366 rows,All the features are in integer execpt age feature.In this dataset there are 2 type of features clinical and histipathological features.The Class feature is the target variable in dataset, where diseases in this group are psoriasis, seboreic dermatitis, lichen planus, pityriasis rosea, cronic dermatitis, and pityriasis rubra pilaris.I have faced challenges during EDA and where we got insight from data.I spent lot's of time In bivariate analysis.I faced some error during hyperparameter tuning but I solved it.
