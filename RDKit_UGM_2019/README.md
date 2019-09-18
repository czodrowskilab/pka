# Open Source p*K*<sub>a</sub> Predictions

## Prerequisites to Run the Notebook

In addition to Jupyter, IPython and Python 3.6 (or higher) the following libraries are required:
- Matplotlib
- Numpy
- Pandas
- RDKit
- Scikit-Learn
- Seaborn

## Dataset

The [monoprotic p*K*<sub>a</sub> dataset](monoprotic_chembl_datawarrior.sdf) was derived from the raw data of 
*[ChEMBL25](https://www.ebi.ac.uk/chembl/)* and *[DataWarrior](http://www.openmolecules.org/datawarrior/)*. 
The p*K*<sub>a</sub> calculator plugin of *Marvin*<sup>[1]</sup> was used for p*K*<sub>a</sub> prediction and for the
determination of the titratable groups.

Every SDF entry has four properties:
- *ID* - A unique identifier over this dataset
- *pKa* - The p*K*<sub>a</sub> value retrieved from *DataWarrior* and *ChEMBL25* (may be averaged)
- *pKa_CX* - The p*K*<sub>a</sub> value predicted by *Marvin*<sup>[1]</sup>
- *atom* - The atom index of the titratable group

## Author

**Marcel Baltruschat** - [GitHub](https://github.com/mrcblt), [E-Mail](mailto:marcel.baltruschat@tu-dortmund.de)

## License

The content of this folder is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## References

[1] *Marvin* 19.15.0, 2019, ChemAxon, [http://www.chemaxon.com](http://www.chemaxon.com)
