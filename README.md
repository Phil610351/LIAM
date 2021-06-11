# Local Information Agent Modelling (LIAM)

Source code of our LIAM implementation in the double speaker-listener environment.
The code is written in python 3, using Pytorch for the implementation of the deep networks. Other important packages are OpenAI Baselines, OpenAI gym, and the Multi-agent Particle Environment.
## Installation
```
virtualenv -p python3 LIAM_ENV
cd LIAM_ENV
source bin/activate
pip install torch
pip install tensorflow
git clone https://github.com/openai/baselines.git
cd baselines
pip install -e .
cd ..
git clone https://github.com/shariqiqbal2810/multiagent-particle-envs.git
cd multiagent-particle-envs
pip install -e .
cd ..
pip install gym==0.9.4
pip install seaborn
git clone git@github.com:uoe-agents/LIAM.git
cd LIAM
cp tasks/simple_reference.py ../multiagent-particle-envs/multiagent/scenarios/.
```
## Execution
```
python run_tests.py 0
```
