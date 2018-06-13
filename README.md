
$$a^2 + b^2 = c^2$$


## AI Pacman (Reinforcement learning)
<p align="center">
  <img src="http://ai.berkeley.edu/images/pacman_game.gif" alt="pacman_gif"/>
</p>


### Introduction

**Reinforcement learning (RL)** is a machine learning area to find the optimal way to achieve a goal. 
**RL** is different from supervised and unsupervised machine learning because there is no "supervisor" to tell the system the right action to take. In order to perform its tasks, **RL** interacts with its environment through trial and error.
It is a sequential decision making process. One step after an other, the **agent** gets to make decision, picks action, see how much rewards it gets and optimizes those rewards to obtain the best possible outcome. 

There is many exemple of **RL** that range from managing an investment portfolio to ,and more importantly, playing video/board games better than humans such as Atari games. :video_game: :space_invader: :trophy:

### Project Learn RL with Pacman

We are a group of fellows from the BootCamp DataScientest egear to learn a bit about **reinforcement learning** and we have followed mainly the online ressource of [UC Berkeley's introductory artificial intelligence course, CS 188](http://ai.berkeley.edu/home.html) to achieved our goal: Create an agent to play _Pacman_!

This website has the purpose to summarize our knowledge on **RL** and to show our progress to our other Fellows at the BootCamp.

### Reinforcement Learing

As said previously, **RL** is about creating an agent that interact with its environment, gets feedback signals (observation and rewards) and makes decision to find the potimal way to achieve a Goal.
In our case, we want Pacman to eat all the dots and avoid to be caught by the ghosts. The decision making of Pacman, our **RL agent**, can be ~~formalized~~ as a **Markov Decision Process (MDP)**.

<p align="center">
  <img src="https://cdn-images-1.medium.com/max/1600/1*Z2yMvuQ1-t5Ol1ac_W4dOQ.png" alt="Principe"/>
  </p>
  
From [Medium](https://medium.com/@m.alzantot/deep-reinforcement-learning-demystified-episode-0-2198c05a6124/)

#### Markov Decision Process

**MDP** encompass a liste of parameters:
1. the possible position of Pacman in the gridworld, termed **states**
2. a group of possible action, here _North_, _South_, _East_ and _West_
3. a ~~set of probabilites that link starting position to other possible position~~, named **transition states**
4. ~~**reward** associated with each transition~~
5. ~~a **Discount factor :gamma:** that quantifies the difference in importance between immediate rewards and future rewards~~

>Life is a Markov Decision Process.

### Q-Learning

Avantage/ incovénient Q-Learning

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
