alpine-rdkit
===

RDKit on alpine linux with Anaconda


Install [Anaconda3](https://www.continuum.io/downloads) and latest version of RDKit from https://anaconda.org/rdkit/rdkit .

## Login with bash

```
docker -it run kubor/alpine-rdkit bash
```

## Example

```
bash-4.3# python
Python 3.6.0 |Anaconda 4.3.1 (64-bit)| (default, Dec 23 2016, 12:22:00)
[GCC 4.4.7 20120313 (Red Hat 4.4.7-1)] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> from rdkit import Chem
>>> m = Chem.MolFromSmiles('Cc1ccccc1')
>>> m.GetNumAtoms()
7
```
