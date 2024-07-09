# Can neuroscientists understand a microprocessor? 
Week 1 paper reading, rough notes

Neuroscientists commonly assume that larger datasets will contribute to understanding of the brain, so they compete in gathering more and more data.

This hypothesis isn't necessarily testable (Since the brain is too complex!)

The authors propose analyzing a simple, well understood microprocessor using techniques commonly employed in neuroscience, as a test.

### Microprocessor analogy to the brain
Analogy: The processor can be used within different video games, analogy to animal brain to various types of animal behaviour. 

The MOS 6502 microprocessor being analyzed is used in the Apple I, Commodore 64, and Atari Video Game System. The study examines the processor's behavior through three different games: Donkey Kong, Space Invaders, and Pitfall.

This complexity, measured by the number of transistors, represents C elegans.

**Key differences**
- The processor is controllable and deterministic
- A biological system is not necessarily manipulatable. It is stochastic, meaning there is unpredictable noise. The system also has robustness and redundancy in the form of neuroplasticity.
Side note: random number generators are fascinating

**Key similarities**
- Organized into levels of analysis.
- Both systems operate on time scales
- Information can be routed with memory.

### What is the success criteria?
The team will reverse engineer the chip, simulate the chip with software with various controllable inputs. The simulation needs to be sufficiently detailed to run games.

### Defining "understanding a system"
Lazbnick, who tested if biologists can understand a radio suggests the intuition:
*When there is broken implementation, you can "fix" it.*

In other words: You can describe the inputs, transformation, outputs, such as a truth table

**Example:** This relates to the discussion on when to use AI-generated code. By the same line of reasoning, as long as you can implement the inputs (written code), transformation and outputs.

### Levels of analyses
A good understanding involves all levels of analysis.
This reminds me of an MLST discussion
There are roughly, physical, computational and algorithmic levels.

**Microprocessor**
- Silicon layout of each transistor
- How a logic gate is formed from the transistor with known truth tables
- Registers, arithmetic logic units
- Circuits e.g. adders

**Brain**
- Synapses
- Neurons
- Microcircuits
- Circuits
- Regions

Side note:
Dynamics (neuro people), behaviour (ml people) and function (psychologists)


### Techniques and results
**Lesion Studies** 
In a microprocessor context, this means leaving transistors on or off.

*"We measure the impact of a lesion by whether or not the system advances far enough to draw the first frame of the game. Failure to produce the first frame constitutes as a loss of function."*

Findings:
Researchers found a subset of 1506 transistors that made the game impossible to render. 

Caution:
One can perform hypothesis testing and find causal relationships, but conceptually, the transistor does not cause a particular aspect of the game, and does not generalize to other games (animal behaviour).

Rather, this transistor implements a simple function like adding within a register.

A subset of disruptive transistors doesn't help understand the processor mechanism in organisms with more neurons (more complexity than flies and C elegans)

Next steps: 
Researchers need to connect to more intermediary levels of analysis and make results generalizable across behaviours. 

---
Okay, here's when I started skimming and took less notes. Feel free to update this.

**Connectomics:** The study uses large-scale microscopy to reconstruct the processor's connectome. But anatomical insights don't lead to a functional understanding.
**Tuning Properties:** Analysis of individual transistor activity shows tuning to specific behaviors, but the apparent tuning is not directly insightful about transistor roles. (individual component lacks context)
**Correlational Structure:** Weak pairwise correlations but strong global correlations are observed, similar to neural systems.
**Local Field Potentials:** Analysis of averaged activity in localized regions shows brain-like signals, but their relation to underlying function is murky.
**Granger Causality:** Conditional Granger causality analysis shows high-level insights but is limited in understanding the processor functionally.
**Dimensionality Reduction:** Techniques like non-negative matrix factorization show underlying signals related to known processor functions, but the insights are context-dependent and seem to exist at a low level of analysis.


### Questions
- The analogy has obvious limitations. How can we know if the same approach for deterministic systems will produce understanding in neuroscience?
- How is the paper received by the broader research community?


### Takeaways
When neuroscientists apply techniques to analyze a microprocessor they reached less understanding than electrical engineering undergrads.

Neuro-research needs more levels of analysis, generalizability and context.