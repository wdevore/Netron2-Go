# Netron2-Go
The second iteration of the network simulation -- Not yet started

# Overview
This simulation (sim) uses the a neuron called "Deuron" from the Deuron8 simulation. At each sim step we perform two passes of the network.

## First pass
In this pass the **post-synaptic** neurons are *evaluated* at the *Soma* based on the current output of the **pre-synaptic** axon. The soma's output is placed into the input gate of axon where the spikes will propagate towards the post-synapse on the second.

## Second pass
In this pass each neuron is *stepped*. This means each axon is internally shifted 1 unit **towards** its output, then the soma's gate in placed into the axon.

Then Inputs are sampled and routed to the input synapses of the input neurons.

# Running the simulation
Just run: ```go run .``` inside the *Netron1-Go* directory


# Dependencies
