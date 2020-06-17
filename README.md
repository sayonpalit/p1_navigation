## Navigation
<p>Deep Q Network based Project Submission for Udacity Deep Reinforcement Learning Nanodegree <a href = "github.com/sayonpalit2599">By Sayon Palit</a></p>
<h1>Project Environment</h1>
<div>
<p>For this project, we will train an agent to navigate (and collect yellow bananas!) in a large, square world.</p>
     				 <img src="https://video.udacity-data.com/topher/2018/June/5b1ab4b0_banana/banana.gif" alt="" width="400px">
<p>A reward of +1 is provided for collecting a yellow banana, 
	and a reward of -1 is provided for collecting a blue banana. 
	Thus, the goal of your agent is to collect as many yellow bananas as possible while avoiding blue bananas.
</p>
<p>The state space has 37 dimensions and contains the agent's velocity, 
	along with ray-based perception of objects around the agent's forward direction.
	Given this information, the agent has to learn how to best select actions. 
	Four discrete actions are available, corresponding to:
</p>
<ul>
<li><strong><code>0</code></strong> - move forward.</li>
<li><strong><code>1</code></strong> - move backward.</li>
<li><strong><code>2</code></strong> - turn left.</li>
<li><strong><code>3</code></strong> - turn right.</li>
</ul>
<p><strong>The task is episodic, 
	and in order to solve the environment,
	your agent must get an average score of +13 over 100 consecutive episodes.</strong>
</p>
</div>

## Requirements
To run the codes, follow the next steps:
* Create a new environment:
	* __Linux__ or __Mac__: 
	```bash
	conda create --name dqn python=3.6
	source activate dqn
	```
	* __Windows__: 
	```bash
	conda create --name dqn python=3.6 
	activate dqn
	```
* Perform a minimal install of OpenAI gym
	* If using __Windows__, 
		* download swig for windows and add it the PATH of windows
		* install Microsoft Visual C++ Build Tools
	* then run these commands
	```bash
	pip install gym
	```
* Install the dependencies under the folder python/
```bash
	cd python
	pip install .
```
* Create an IPython kernel for the `dqn` environment
```bash
	python -m ipykernel install --user --name dqn --display-name "dqn"
```
* Download the Unity Environment specific to your operating system
	* [Linux](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
	* [Mac OSX](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
	* [Windows (32-bits)](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
	* [Windows (64 bits)](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)

* Start jupyter notebook from the root of this python codes
```bash
jupyter notebook
```
* Once started, change the kernel through the menu `Kernel`>`Change kernel`>`dqn`
* If necessary, inside the ipynb files, change the path to the unity environment appropriately


## Results
<img src = "https://github.com/sayonpalit2599/p1_navigation/blob/master/plot.jpg" alt = "result">
The current model solves the environment in 700-750 epsiodes on average.
