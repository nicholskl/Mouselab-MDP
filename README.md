# Mouselab-MDP
Mouselab-MDP is a [JsPsych](https://github.com/jodeleeuw/jsPsych/) plugin that renders Markov decision processes (MDP) for participants to navigate through. Optionally, information about the environment can be presented only when the participant asks for it, thus creating a record of the information considered. Try out the live demo mouselab-demo [here](http://cocosci.dreamhosters.com/webexpt/mouselab-demo/).

# Abstract
Below is the abstract for our submission to Reinforcement learning and decision making: "Mouselab-MDP: A new paradigm for tracing how people plan".

Planning is a latent cognitive process that cannot be observed directly. This makes it difficult to study how people plan. To address this problem, we propose a new paradigm for studying planning that provides experimenters with a timecourse of participant attention to information in the task environment. This paradigm employs the information-acquisition mechanism of the Mouselab paradigm, in which participants click on options to reveal the outcome of choosing those options. However, in contrast to the original Mouselab paradigm, our paradigm is a sequential decision process, in which participants must plan multiple steps ahead to achieve high scores. We release Mouselab-MDP open-source as a plugin for the JsPsych online Psychology experiment library. The plugin displays a Markov decision process as a directed graph, which the participant navigates to maximize reward. To trace the the process of planning, the rewards associated with states or actions are initially occluded; the participant has to click on a transition to reveal its reward. Thus, the participant makes explicit the states she considers in her information gathering behavior. We illustrate the utility of the Mouselab-MDP paradigm with a proof-of-concept experiment in which we trace the temporal dynamics of planning in a simple environment. Our data shed new light on people’s approximate planning strategies and on how people prune decision trees. We hope that the release of Mouselab-MDP will facilitate future research on human planning strategies. In particular, we hope that the fine-grained time course data the paradigm generates will be instrumental in specifying algorithms, tracking learning trajectories, and characterizing individual differences in human planning

# Usage
A basic description of how to use the plugin can be found in our RLDM paper. If you don't have access to the paper, email fredcallaway@berkeley.edu and ask for a copy. There is also a limited amount of inline documentation in [jspsych-mouselab-mdp.coffee](/jspsych-mouselab-mdp.coffee). Pay special attention to the constructor of `MouselabMDP`, around line 90.

# Example experiment
The code for the demo can be found in [experiment/](/experiment/). The stimulus specifications are in [experiment/json/trials.json](/experiment/json/trials.json)