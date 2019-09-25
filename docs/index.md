# Getting Started

To train a simple model with a standard training loop with **Kerosene** you'll need to define two things: 

- A Pytorch model
- A config file

For more complex use cases, like multiple models, or fancy architecture with complex training strategy, a 
<b>Trainer</b> should be provided. 

## Model Trainer

Kerosene supports standard Pytorch model (i.e. ```torch.nn.Module```). There is **no need to extend any class 
or add any logging dependencies to your model**. We believe that your model should only contain model related code. It should be clean
and lean. 

Instead, the model is wrapped in a ```kerosene.training.trainers.ModelTrainer``` class which handles 

## Trainer

The trainer object can be seen as the training orchestrator. The trainer handles the following:

- Main training and validation loops;
- Data loading (from the data loaders) and the distribution to the good device (GPU/CPU);
- Training event handling

For a simple use case where a single model is used with standard forward and backward passes, the predefined
```kerosene.training.trainers.SimpleTrainer``` can be used. It will handle all the training and validation process for you.



## Configuration

## 
```python 

class Python(object):
    def __init__(self):
        pass
```
