# Obtain Molecule Graph Attributes For GNN

## Inputs: List of SMILES String

<p align="center"> <img width="800"  src="https://user-images.githubusercontent.com/47986787/168453938-80d5413f-c6ab-4fdf-82b9-5909c41c7c71.png"> </p>


## Outputs: 
## 1. Annotaion of molecules

<p align="center"> <img width="400"  src="https://user-images.githubusercontent.com/47986787/168453803-13b4c809-3828-418b-9154-95e575d7075b.png"> </p>


## 2. Get Morgan Substrctures

<p align="center"> <img width="900"  src="https://user-images.githubusercontent.com/47986787/168453822-20f5a344-26b4-428c-89c3-cbd09f12d509.png"> </p>


## 3. Molecule-Graph-Attributes-For-GNN
    #1. Atom_Attributes             size: (n_node, n_attr)               type: numpy.array
        1.1 Attributes are Morgan encodings of molecule substructures centered around each atom.
    #2. Atom_RXN_Portion            size: (n_rxn_portion)                type: List
        2.1 Reaction portion are extracted through pattern matching of the molecule structures with reaction rules.
    #3. Bond_Adjacency_Matrix       size: (n_node, n_node)               type: numpy.array
        3.1 Bond information can be easily obtained using RDKit python libraries.
    #4. Bond_Attributes             size: (n_node, n_node, dim_attr)     type: numpy.array
        4.1 Bond Energy is obtained using -Alfabet-.
        4.2 Bond Length is obtained using RDKit.
