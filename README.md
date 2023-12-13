# Enhancing-By-Subtasks-Components

This project presents an experimental approach to tackle the challenge of data scarcity in a specific NLP task by exploring the utilization of existing annotated datasets from related tasks. Our experiment involves training a single base model, such as BERT, with multiple heads that are each dedicated to a specific task, and running them simultaneously during training. We term these additional tasks as "supporting tasks." The goal is to leverage shared knowledge across different domains and by that enhance the model's performance.

See the full report in the following pdf: ```Advanced_NLP_Project.pdf```

**Branches:**
- Medical tasks can be found in the `main` branch.
- The GLUE (General Language Understanding Evaluation) tasks can be found in the `glue_tasks` branch.

The multi-head model can be viewed in ```models/multiHeadModel.py```<br/>  The multi-head training can be viewed at ```train.py```

## Multi-Head Model Architecture 

![Advanced NLP Project](https://github.com/NivAm12/Enhancing-By-Subtasks-Components/assets/68702877/d672ae7a-e7ee-4443-88d7-3b8481e225ad)


# Install
``` pip install -r requirements.txt ```

# Train
Run:

``` python train.py  --batch_size <batch size> --epochs <number of epochs> --device <device>```<br/>

For the rest of the arguments, please see ```train.py```

