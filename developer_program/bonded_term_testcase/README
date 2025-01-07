# Testcase to perform MM calculation for optimized bonded parameters and compare to QM
# ((5aS,9aR)-3-nitro-5a,6,7,8,9,9a-hexahydro-1H-1,5-benzodiazepine) (CGenFF: 2300P8) from Figure 6 & 7

# To run charmm executable has to be added to the PATH
# To run use:
../developer_bonded.exe intra.inp > intra.out

# intra.inp contains all the settings for optimization

# MM structures will be created in "results" directory
# QM structures and PES energies for both QM and MM will be created in "bond" directory
# all pes scans points are in "bond/energy.results.dat" 

# opt1.pdb = QM minimized geometry
# emp.pdb and emp.woconstr.pdb  = empirical minimized geometies with and without constraints on rotatable dihedrals

# If CREST was used to create additional conformations, their geometries have to be minimized with QM and output files should be copied to bond/target-structures
