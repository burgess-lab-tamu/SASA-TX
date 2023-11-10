# SASA-TX

input:
The general input format is in the third block of 'SASA-TX.ipynb', which can be opened by Jupyter Notebook.

Here shows the input format copied from the notebook:

hotspots,_ = sasa_selected_residues('pdb name + .pdb','chain name','start residue','end residue')
#input pdb path + target chain 
hotspots = pd.DataFrame(hotspots)
#save as pandas format
hotspots.to_csv('name of output +.csv')
#save as csv file with default name

output:
output is a csv file with three columns
column 1: residue ID
column 2: % buried for this residue
column 3: buired area for this residue

higher % buried (column 2) and higher buried ared (column 3) suggest a more important residue in the targeted protein-protein interactions.
