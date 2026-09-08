A Unit of thinking

- could be a linear unit
![[Pasted image 20260908183214.png]]
multi inputs
y = b(w0) + w1 * x1 + w2 * x2 + w3 * x3


# Linear Units in Keras

```
from tensorflow import keras
from tensorflow.keras import layers

# Create a network with 1 linear unit
model = keras.Sequential([
    layers.Dense(units=1, input_shape=[3])
])
```

With the first argument, `units`, we define how many outputs we want. In this case we are just predicting `'calories'`, so we'll use `units=1`.

With the second argument, `input_shape`, we tell Keras the dimensions of the inputs. Setting `input_shape=[3]` ensures the model will accept three features as input (`'sugars'`, `'fiber'`, and `'protein'`). 

`object.attribute`

w, b = model.weights 