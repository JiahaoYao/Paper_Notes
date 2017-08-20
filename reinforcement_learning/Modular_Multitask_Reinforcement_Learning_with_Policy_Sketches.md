# Modular Multitask Reinforcement Learning with Policy Sketches

This uses the multi-task idea because the value of the RL can be sparse. The multitask RL is really impressive and effective. Rollout [^Rollout]  just means sampling according to the policy. [^Curriculum]Curriculum learning judges the difficulty of the tasks according to the length. I think the very smart thing is that the paper uses augmented state space adding the stop sign into the state space.

[^Rollout]: https://www.quora.com/What-is-rollout-in-machine-learning	"Rollout means unfolding"
[^Curriculum]: https://ronan.collobert.com/pub/matos/2009_curriculum_icml.pdf	"It still has some abstract level meaning."