<h1 align="center" id="title">Predicitng Vibration from Pile Driving in Bangkok Subsoil</h1>

<p id="description">This is the inference part according to the paper 'Predicting Pile-Induced Vibrations in Bangkok Subsoil: A Neural Network Approach</p>

  
  
<h2>🧐 Features</h2>

Here are some of the project's best features:

*   Estimate the peak partial velocity of pile driving in Bangkok subsoil
*   The features of the model are - pile size, pile length, hammer weight, hammer height, distance to pile driving, location of the sensor, axis of sensor
  

<h2>🛠️ Installation Steps:</h2>

<p>1. installation</p>

```
git clone https://github.com/Sompote/pile_PPV
```

<p>2. Inference</p>

```
open notebook  pile_PPV_inference.ipynb
```
The feature of pile driving just input it in the Numpy array: 

'''
# input [pile length(m), weight (ton), drop height (m), distance (m), Location, trigger]
#location 1:on ground 2:on foundation 3: on building
#trigger 1: longitudinal 2:transverse 3:vertical)
'''

'''
X_t=np.array([300,18,4.2,0.5,30,1,1])
'''

<h2>🍰 Contribution Guidelines:</h2>

Additional data for pile driving are welcomed to train the model making it more efficient.

<h2>Acknowledgements:</h2>
Thanks, STS Co. Ltd for provide a testing data,
