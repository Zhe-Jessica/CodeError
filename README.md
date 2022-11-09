# CodeError
The question of my Julia code


I am trying to use sciml_train in Flux to train a neural network model using the data from an engineering system. The data contains many groups of measurements with different initial states. I gave these initial states to the neural network individually and calculated the loos function by summing the mean squared error of all measurements. It is easier for me to use for loop when I have many groups of measurements. However, I got an error like this:

```
ERROR: MethodError: no method matching (::var"#5#7")(::Vector{Float32}, ::Float32)
Closest candidates are:
(::var"#5#7")(::Any, ::Any, !Matched::Any; doplot)
```

When I didn’t use for loop, I did not have the error. I doubt that I might use the for loop in a wrong way. However, I need for loop in this work, as I need to calculate the output of the neural network separately. 
I demonstrate two groups of measurements here. Hope it makes my question clear.

