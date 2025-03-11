# A liquid-state NMR database for small molecules 

___This is a draft, details will follow ...___

The strategy we will follow for the creation of a liquid-state NMR database for small molecules is:

1. Create an identifyer of chemistry-relevant files found in a zip file (find .mnova files, bruker file trees, .mol files, gaussian calculation files, _etc._)

2. Find chemistry-relevant files in common open repositories (upload content of repositories, find chemistry-relevant file (see 1) and add authorship metadata). 

3. Connect molecules with spectra and register the molecule-spectrum pairs on this github repository using a pull request
   - if a .mol file is found in the NMR spectra file tree
   - by exporting .mnova file content into .json and combine the molecule.json with the nmr.json data
   - _any other mecanism ..._

4. Add information supporting the assignement of the molecule(s) to set of spectra 
   - add multiplet assignment and coupling constants (can be found in the Mnova json files)
   - add validation flags (compatibility with chemical shift prediction, uniquness of structure with respect to logic for structure determination of 2D spectra), _etc._
   - add NMReDATA
   - _add any other relevant information ..._

Initially, the registration and addition of supporting information would be done using pull requests on this repository, but a more rebust mecanism can easily be introduced. The point of this project is to separate the steps in the spirit of the CHEMaDATA initiative:

- Identify chemistry files 
- Extract metadata from the chemistry files and create CHEMeDATA objects for spectra, molecules and assigned spectra.

This mecanism is flexible allowing anybody to contribute at by 
- adding identifyer of chemistry-relevant archives (see point 1)
- adding repository extractor for chemistry-relevant archives (see point 2)
- adding mecanism for the formation of pairs (see point 3)
- add metadata to existing pairs (assignment, validation, etc. see point 4)


