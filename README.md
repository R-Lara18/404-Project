# 404-Project

Full CSV that we are using. Cannot be uploaded into github due to large size. 
https://www.kaggle.com/datasets/jasperan/league-of-legends-1v1-matchups-results?resource=download&select=matchups.csv


### Individual Teams Perceptron:
  
  * Train Score:  0.6974409727131344
  * Test Score:  0.7024390243902439
  * Recall Score (Test): 0.8963380281690141
  * F1 Score (Test): 0.754207158094335 
  
### Match Perceptron:

- Dataset with joined teams(x = team 1, y = team 2):
matchID, WIN, GOLDEARNED_x, TOTALMINIONSKILLED_x, KILLS_x, ASSISTS_x, DEATHS_x, VISIONSCORE_x, TOTALDAMAGEDEALTTOCHAMPIONS_x, 
GOLDEARNED_y, TOTALMINIONSKILLED_y, KILLS_y, ASSISTS_y, DEATHS_y, VISIONSCORE_y, TOTALDAMAGEDEALTTOCHAMPIONS_y

  * Train Score:  0.959705923936095
  * Test Score:  0.9595408895265424
  * Recall Score (Test): 0.9325084364454443
  * F1 Score (Test): 0.9592131906277119
  
- Dataset with joined teams(x = team 1, y = team 2) and ratio features(21 total features):
matchID, WIN, GOLDEARNED_x, TOTALMINIONSKILLED_x, KILLS_x, ASSISTS_x, DEATHS_x, VISIONSCORE_x, TOTALDAMAGEDEALTTOCHAMPIONS_x, 
GOLDEARNED_y, TOTALMINIONSKILLED_y, KILLS_y, ASSISTS_y, DEATHS_y, VISIONSCORE_y, TOTALDAMAGEDEALTTOCHAMPIONS_y
GOLDEARNED_ratio, TOTALMINIONSKILLED_ratio, KILLS_ratio, ASSISTS_ratio, DEATHS_ratio, VISIONSCORE_ratio, TOTALDAMAGEDEALTTOCHAMPIONS_ratio
  
  * Train Score:  0.968
  * Test Score:  0.9669373549883991
  * Recall Score (Test):  0.9821634062140391
  * F1 Score (Test):  0.967687074829932
  
### Match Decision Tree:

- Dataset with joined teams(x = team 1, y = team 2):
matchID, WIN, GOLDEARNED_x, TOTALMINIONSKILLED_x, KILLS_x, ASSISTS_x, DEATHS_x, VISIONSCORE_x, TOTALDAMAGEDEALTTOCHAMPIONS_x, 
GOLDEARNED_y, TOTALMINIONSKILLED_y, KILLS_y, ASSISTS_y, DEATHS_y, VISIONSCORE_y, TOTALDAMAGEDEALTTOCHAMPIONS_y

  * Train Score:  1.0
  * Test Score:  0.959106728538283
  * Recall Score(test):  0.9313835770528683
  * F1 Score(test):  0.928771733034212
  
- Dataset with joined teams(x = team 1, y = team 2) and ratio features(21 total features):
matchID, WIN, GOLDEARNED_x, TOTALMINIONSKILLED_x, KILLS_x, ASSISTS_x, DEATHS_x, VISIONSCORE_x, TOTALDAMAGEDEALTTOCHAMPIONS_x, 
GOLDEARNED_y, TOTALMINIONSKILLED_y, KILLS_y, ASSISTS_y, DEATHS_y, VISIONSCORE_y, TOTALDAMAGEDEALTTOCHAMPIONS_y
GOLDEARNED_ratio, TOTALMINIONSKILLED_ratio, KILLS_ratio, ASSISTS_ratio, DEATHS_ratio, VISIONSCORE_ratio, TOTALDAMAGEDEALTTOCHAMPIONS_ratio
  
  * Train Score:  1.0
  * Test Score:  0.9588167053364269
  * Recall Score(test):  0.9585730724971231
  * F1 Score(test):  0.9594010941549093

### Match Logistic Regression:

- Dataset with joined teams(x = team 1, y = team 2):
matchID, WIN, GOLDEARNED_x, TOTALMINIONSKILLED_x, KILLS_x, ASSISTS_x, DEATHS_x, VISIONSCORE_x, TOTALDAMAGEDEALTTOCHAMPIONS_x, 
GOLDEARNED_y, TOTALMINIONSKILLED_y, KILLS_y, ASSISTS_y, DEATHS_y, VISIONSCORE_y, TOTALDAMAGEDEALTTOCHAMPIONS_y

  Train Score:  0.9746924925774071
  Test Score:  0.9704447632711621
  * Recall Score(test):  0.9707536557930259
  * F1 Score(test):  0.9707536557930259

- Dataset with joined teams(x = team 1, y = team 2) and ratio features(21 total features):
matchID, WIN, GOLDEARNED_x, TOTALMINIONSKILLED_x, KILLS_x, ASSISTS_x, DEATHS_x, VISIONSCORE_x, TOTALDAMAGEDEALTTOCHAMPIONS_x, 
GOLDEARNED_y, TOTALMINIONSKILLED_y, KILLS_y, ASSISTS_y, DEATHS_y, VISIONSCORE_y, TOTALDAMAGEDEALTTOCHAMPIONS_y
GOLDEARNED_ratio, TOTALMINIONSKILLED_ratio, KILLS_ratio, ASSISTS_ratio, DEATHS_ratio, VISIONSCORE_ratio, TOTALDAMAGEDEALTTOCHAMPIONS_ratio
  
  * Train Score:  1.0
  * Test Score:  0.959106728538283
  * Recall Score(test):  0.9585730724971231
  * F1 Score(test):  0.9594010941549093
  


### Match Pytorch:

- Dataset with joined teams(x = team 1, y = team 2):
matchID, WIN, GOLDEARNED_x, TOTALMINIONSKILLED_x, KILLS_x, ASSISTS_x, DEATHS_x, VISIONSCORE_x, TOTALDAMAGEDEALTTOCHAMPIONS_x, 
GOLDEARNED_y, TOTALMINIONSKILLED_y, KILLS_y, ASSISTS_y, DEATHS_y, VISIONSCORE_y, TOTALDAMAGEDEALTTOCHAMPIONS_y

    Epoch [1/10], Loss: 0.0250
    Epoch [2/10], Loss: 0.0186
    Epoch [3/10], Loss: 0.0025
    Epoch [4/10], Loss: 0.0026
    Epoch [5/10], Loss: 0.0052
    Epoch [6/10], Loss: 0.0008
    Epoch [7/10], Loss: 0.0012
    Epoch [8/10], Loss: 0.0005
    Epoch [9/10], Loss: 0.0015
    Epoch [10/10], Loss: 0.0006
    
    Accuracy: 99.95%
    Recall on the validation set: 1.0000

- Dataset with joined teams(x = team 1, y = team 2) and ratio features(21 total features):
matchID, WIN, GOLDEARNED_x, TOTALMINIONSKILLED_x, KILLS_x, ASSISTS_x, DEATHS_x, VISIONSCORE_x, TOTALDAMAGEDEALTTOCHAMPIONS_x, 
GOLDEARNED_y, TOTALMINIONSKILLED_y, KILLS_y, ASSISTS_y, DEATHS_y, VISIONSCORE_y, TOTALDAMAGEDEALTTOCHAMPIONS_y

    Epoch [1/10], Loss: 0.0250
    Epoch [2/10], Loss: 0.0186
    Epoch [3/10], Loss: 0.0025
    Epoch [4/10], Loss: 0.0026
    Epoch [5/10], Loss: 0.0052
    Epoch [6/10], Loss: 0.0008
    Epoch [7/10], Loss: 0.0012
    Epoch [8/10], Loss: 0.0005
    Epoch [9/10], Loss: 0.0015
    Epoch [10/10], Loss: 0.0006
    
    Accuracy: 99.81%
    Recall on the validation set: 1.0000

```python

```
