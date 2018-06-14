
## AI Pacman (Reinforcement learning)
<p align="center">
  <img src="http://ai.berkeley.edu/images/pacman_game.gif" alt="pacman_gif"/>
</p>


### Project Learn RL with Pacman

We are a group of fellows from the BootCamp DataScientest egear to get familiarize ourselves with **reinforcement learning**.  We have followed mainly the online ressource of [UC Berkeley's introductory artificial intelligence course CS 188](http://ai.berkeley.edu/home.html) with the support of the book [Reinforcement Learning: An introduction](http://incompleteideas.net/book/bookdraft2017nov5.pdf) of R. S. Sutton and A. G. Barto to achieved our goal: Create an agent to play _Pacman_!

This website has the purpose to summarize our knowledge on **RL** and to show our progress to our other Fellows at the BootCamp.

### Reinforcement Learning

**Reinforcement learning (RL)** is a machine learning area to find the optimal way to achieve a goal. 
**RL** is different from supervised and unsupervised machine learning because there is no "supervisor" to tell the system the right action to take. In order to perform its tasks, **RL** interacts with its environment through trial and error.

It is a sequential decision making process. One step after an other, the **agent** gets to make decision, picks action, see how much rewards it gets and optimizes those rewards to obtain the best possible outcome. 

There is many exemple of **RL** that range from managing an investment portfolio to playing video/board games better than humans such as Atari games. :video_game: :space_invader: :trophy:

As said previously, **RL** is about creating an agent that interact with its environment, gets feedback signals (observations and rewards) and makes decision to find the potimal way to achieve a Goal.
In our case, we want Pacman, throught our **RL agent**, to eat all the dots and avoid to be caught by the ghosts. The decision making of Pacman can be visualized as a **Markov Decision Process (MDP)**.

<p align="center">
  <img src="https://cdn-images-1.medium.com/max/1600/1*Z2yMvuQ1-t5Ol1ac_W4dOQ.png" alt="Principe"/>
 </p>
  
From [Medium](https://medium.com/@m.alzantot/deep-reinforcement-learning-demystified-episode-0-2198c05a6124/)

#### Markov Decision Process

**MDP** encompass a liste of parameters:
1. the possible position of Pacman in the gridworld, termed **states** and its value **_s_**
2. the possible **action _a_** and its value **_Q_**, _North_, _South_, _East_ and _West_
3. the probabilities that link starting to other position depending of the action taken, named **transition states probabilities _P_**
4. the **rewards _r_**  associated with each transition
5. the **gamma factor**, which is a discount factor to promote immediate or long-term rewards

The objective of the **agent** is to maximize the sum of rewards in long-term by taking the best action in each state.

### Q-Learning

At the beginning, the **agent** has a representation of the environement that are the **states** and possible **actions** in those states but doesn't know the values of thoses parameters. It is during training that the **agent** will explore the environment and learn the value of each of those actions in each of those states. After it took an action from the **state s** and arrived to the **state s+1**, it evaluates the **state s** by updating the **action value _Q_** depending if it is a desirable state or not.

The **_Q_ value** is updated following this equation :
<p align="center">
  <img src="https://cdn-images-1.medium.com/max/800/0*q8Dnp4guvDD230if." alt="q value update"/>
 </p>

Let's says that the **learning rate** is set to 1, which means that the old value is replaced by the updated value, and that the **discount factor** is set to 1 (no discount). So the updated value is equivalent to the sum of the **reward** obtained and the estimated future rewards.
After a number of iteration (number of times the agent try the games), there is an estimated value for each state-action pairs, which will converge eventually to the optimal value after a certain number of iterations. The **agent** will select which action to take according to a **policy**, for example a **greedy policy** that will always to the action with the highest **_Q_ value**.

Finally, all the **state-action values** are stored in a table of size **N** * **M**, where **N** is the number of possible states and **M** is the number of possible actions. To get the optimal policy, which get the maximum rewards, the **agent** needs to perform a lot of iteration process. This is fine for small gridworld but when the **agent** evolves in a medium or large gridworld, it needs a huge numbers of iteration taking a long time to train.

### Approximate Q-Learning

Avantage/incovénients

### Application Réseaux de neurones

Intérêt du RN.

### to add 

The most fundamental quantity in RL is the rewards that is a scalar feedback signal, here name R_{t}.
Sometimes, the **agents** makes a decision now and gets to see if it was a good decision or bad decision only many steps later. 

## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/MevaeR/MevaeR.github.io/edit/master/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/MevaeR/MevaeR.github.io/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
