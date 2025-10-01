# Explanation-Driven Self-Adaptations (XDA) Replication Package

## Our papers
[Efficient Self-Adaptation through Explanation-Driven White-Box Optimization](https://dl.acm.org/doi/10.1145/3737648)
[Explanation-driven Self-adaptation using Model-agnostic Interpretable Machine Learning](https://dl.acm.org/doi/10.1145/3643915.3644085)

## Install Requirements
```pip install -r requirements.txt```

### For macOS and Linux Users
```chmod +x MDP_Dataset_builder/evaluate_adaptations.sh```

## Generate Dataset (Optional)

Inside MDP_Dataset_builder/run.sh and MDP_Dataset_builder/run.bat:
* MAX_SAMPLES: number of samples to generate
* TOTAL_THREADS: number of threads to use for the generation

### For macOS and Linux Users
```
chmod +x MDP_Dataset_builder/run.sh
./run.sh
```

### For Windows Users
```.\run.bat```

## Run Adaptation Tests
Inside main/main.py:
* line 43: you can specify the path to your dataset
* line 61: you can specify the list of requirements to consider
* line 64: you can specify the size of the neighborhood
* line 65: you can specify the number of starting solutions to consider
* line 68: you can specify the target success probabilities for each requirement
* line 120: you can specify the number of tests to do

```python main/main.py```

## Generate Plots
```python main/makeAllPlots.py```
