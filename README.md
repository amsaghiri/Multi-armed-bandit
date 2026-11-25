# Multi-armed Bandit

Notebooks on the **multi-armed bandit** problem, for teaching and self-study. They are used as course
material by Dr. Ali Mohammad Saghiri ([homepage](https://amsaghiri.github.io/)).

In a multi-armed bandit problem an agent repeatedly chooses one of several actions ("arms"), each with
an unknown average reward. It has to balance **exploration** (trying arms to learn about them) against
**exploitation** (pulling the arm that looks best so far).

## Notebooks

| Notebook | What it shows |
| --- | --- |
| `MAB.ipynb` | A single ε-greedy agent on a Gaussian bandit, with action-value updates `q ← q + α(reward − q)`. |
| `MABgame.ipynb` | Several bandit agents playing a cooperative game through a shared environment. |
| `MABgame2.ipynb` | The same game with the code commented line by line. Start here if you are reading the code. |

Each notebook has an **Open in Colab** badge at the top, so nothing needs to be installed. To run
locally you need Python 3 with NumPy, Matplotlib, and Jupyter.

## Things to try

- Change `epsilon`. What happens with 0 (never explore) and with 1 (always explore)?
- Change the learning rate `alpha`. When is a small value better?
- Increase the number of arms and see how many steps the agent needs.

## Related repositories

- [Learning-Automata](https://github.com/amsaghiri/Learning-Automata) – the same problem solved with a learning automaton
- [Goore-Game](https://github.com/amsaghiri/Goore-Game) – the cooperative game, played by learning automata
