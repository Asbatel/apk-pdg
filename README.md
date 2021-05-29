# Welcome to Apk-pdg

An Androguard-based framework to create a Program Dependence Graph (PDG) of an Android application (apk).

# Program Dependence Graph

- A graph that considers both data and control dependences. The data dependence represents the program’s appropriate data flow whereas the control dependence illustrates the program’s control flow relationships.
- The combination of both dependences covers all the program’s computational parts.

# PDG Topology 

- The Program Dependence Graph’s nodes represent the *Basic Blocks* and the edges represent both the data values and control conditions necessary to the execution of the node’s operations.
- The PDG is constructed from the *Androguard Analysis Object* and then converted into a *Networkx DiGraph*. 
- The current supported format is *gpickle*.

# Requirements

The construction process uses the following tool:

   - **Androguard**: It is used for statically analyzing the target APK and extracting its contextual and structural data. (https://github.com/androguard/androguard)
    
# Installation and Usage

   1. Download or clone the repo (git clone https://github.com/Asbatel/apk-pdg.git)
   2. Install **Androguard** (latest version)
   3. Navigate to the main directory: `cd pdg/`
   4. Run the following command: `python get_graph.py <apk_path>`
  



