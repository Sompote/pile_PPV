<h1 align="center" id="title">Predicitng Vibration from Pile Driving in Bangkok Subsoil</h1>

<p id="description">This is the inference part according to the paper 'Predicting Pile-Induced Vibrations in Bangkok Subsoil: A Neural Network Approach' by Sompote Youwai						
and Anuwat Pamungmoon
</p>

  
  
<h2>🧐 Features</h2>

Here are some of the project's best features:

*   Estimate the peak partial velocity of pile driving in Bangkok subsoil
*   The features of the model are - pile size, pile length, hammer weight, hammer height, distance to pile driving, location of the sensor, the axis of the sensor
  
    
<h2>Abstract:</h2>
This study presents a deep learning model designed to assess ground vibrations resulting from pile driving, a critical aspect of construction. Utilizing data from 1,034 sensors deployed throughout Bangkok, the model incorporates variables such as pile size, length, sensor proximity, hammer mass, and drop height. Analysis revealed that the most significant factors influencing vibration levels were the distance to the driving location, hammer weight, and pile length, as determined by mutual information. The model, trained on a broad range of datasets representing different environmental conditions, predicts peak particle velocity levels with a Mean Absolute Percentage Error (MAPE) of 8.9%. Notably, this model surpasses traditional empirical approaches that often overpredict peak particle velocity in Bangkok’s subsoil, which is attributed to the high damping properties of Bangkok Clay. Access to the model’s inference is provided through a GitHub repository



<h2>🛠️ Installation Steps:</h2>

<p>1. installation</p>

```
git clone https://github.com/Sompote/pile_PPV
```

<p>2. Inference</p>

```
open notebook  pile_PPV_inference.ipynb
```

<p>3. Changing features</p>

The feature of pile driving just input it in the Numpy array: 


input [pile length(m), weight (ton), drop height (m), distance (m), Location, trigger]
#location 1:on ground 2:on foundation 3: on building
#trigger 1: longitudinal 2:transverse 3:vertical)

```

X_t=np.array([300,18,4.2,0.5,30,1,1])
```

<h2>🍰 Contribution Guidelines:</h2>

Additional data for pile driving are welcomed to train the model making it more efficient.

<h2>Acknowledgements:</h2>
Thanks, STS Co. Ltd for providing a testing data.
