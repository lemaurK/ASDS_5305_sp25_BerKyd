# ASDS 5303 Final Project 
## Group Name: sp25_BerKyd
## Group Members:
### Henry Berrios #1001392315
### LeMaur Kydd #1001767382

# Dataset Title: Drug SMILES Strings and Classifications

**Source:** Research Paper Supporting Information [SMILES LINK](https://pubs.acs.org/doi/suppl/10.1021/acs.jcim.9b00236/suppl_file/ci9b00236_si_003.xlsx)

The SMILES Strings and Drug Classification dataset sourced from a paper is a compilation of a few different datasets, namely **PubChem** and **ZINC**. It contains SMILES Strings, which will function as the basis of our training data, and **drug classifications**, which will be our target variable. There are 6 other chemical features that can help classification performance if necessary.

## Features in the Dataset:
- **IsomericSMILES Strings**
- **De-salted SMILES Strings**
- **Drug Classification** *(Target)*
- **XLogP**
- **Molecular Weight**
- **CID (PubChem Molecular ID#)**
- **HBondAcceptorCount**
- **HBondDonorCount**

---

## Defining the ML Problem

- **Supervised Learning Task:** Classification  
- **Modality:** Text (character-based SMILES strings)  
- **Goal:** Predict the Drug Classification of a given SMILES String using only the SMILES String data  
- **Potential Use:** Molecular structures can have their medicinal value estimated without costly lab research based on its SMILES String  
- **Target Variable:** Drug Classification (categorical variable)  
- **Output Modeling:** Model outputs class probabilities via softmax and selects the class with the highest probability as prediction  

---

## Why It's Challenging:
SMILES strings encode complex molecular structures as linear text, making it difficult for traditional models to interpret chemical meaning.

## Why It Matters:
Accurate predictions could accelerate drug discovery by reducing reliance on costly lab experiments through in-silico molecular screening.
