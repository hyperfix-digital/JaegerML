# Deck Model

The left and right Deck will each have individual models developed based off of two sets of moves:

|left|right|
|---|---|
|<div><ui><li>left stance jab<li>left stance small hook<li>right stance punch<li>right stance large hook<ui></div>|<div><ui><li>right stance jab<li>right stance small hook<li>left stance punch<li>left stance large hook<ui></div>|

# Data Collection
  
The data will be collected first by recording for each device 50 observations of the 4 moves corresponding to that device. For initial testing, each observation will consist of 119 samples, each sample consisting of 6 values from the accelerometer and gyroscope.
After each punch is recorded the 'puncher' will rotate random amounts to add variety in rotational direction for each punch.
  
Because the developers and thus the data gatherers are few in this project, we can make use of some math to synthesize new punch sequences for our dataset. Because the 'puncher' is to randomly rotate after each punch, we can synthesize more punches by taking the punch data we already have and rotating it around a center axis to create new 'punch trails' like so:
  
  
