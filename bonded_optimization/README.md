QM data as well as MM data obtained using partial charges from CGenFF v2.5.1 (inital) and CGenFF v5 (retrained), and two cycles of charge optimization (optimized and reoptimized). Second cycle of optimization was only performed for 108 molecules. Bonded terms are compared for v2.5.1 (inital), optimized bonded terms and generated with CGenFF v5.

For bonded terms optimization target data included:
 - QM minimized geometry
 - If available, QM minimized geometries and energies after identifying additional minima with CREST.
    During optimization of bonded terms, restraints on rotatable dihedrals were applied.
 - QM bonded term equilibrium value
 - QM Potential Energy Surface Scans with restrains on rotatable bonds if needed

| Filename                                   | Units      | Description                                                                                                 | 
|--------------------------------------------|------------|-------------------------------------------------------------------------------------------------------------| 
| min_geom_cons.dat                          | Angs       | All-Atom RMSD comparing QM and MM minimal energy geometries                                                 |                    
| min_geom_no_cons.dat                       | Angs       | Same as min_geom_cons.dat, where during MM minimization no restraints/constraints were used                 |
|                                            |            |                                                                                                             |
| B_eq_values.dat                            | Angs       | Optimized bond equilibrium value from minimized geometry                                                    |
| A_eq_values.dat                            | Deg        | Optimized angle equilibrium value from minimized geometry                                                   |
| D_eq_values.dat                            | Deg        | Optimized dihedral torsion equilibrium value from minimized geometry                                        |
| I_eq_values.dat                            | Deg        | Optimized improper angle equilibrium value from minimized geometry                                          |
|                                            |            |                                                                                                             |
| bond_ener_all.dat                          | kcal/mol   | PES scans energy points for bonds                                                                           |
| angle_ener_all.dat                         | kcal/mol   | PES scans energy points for angles                                                                          |
| dihe_ener_rigid_all.dat                    | kcal/mol   | PES scans energy points for non-rotatable dihedrals                                                         |
| dihe_ener_soft_all.dat                     | kcal/mol   | PES scans energy points for rotatable dihedrals                                                             |
| in-ring_ener_all.dat                       | kcal/mol   | PES scans energy points for non-rigid dihedrals inside rings                                                |
| impr_ener_all.dat                          | kcal/mol   | PES scans energy points for improper angles                                                                 |
|                                            |            |                                                                                                             |
| pes_scans_bonded_terms.pdf                 | kcal/mol   | Graphical repesentations of PES scans                                                                       |
|                                            |            |                                                                                                             |
| energy_multi_conf.dat                      | kcal/mol   | Relative energies for CREST geometries                                                                      |
| energy_multi_conf_no_cons.dat              | kcal/mol   | Same as energy_multi_conf.dat, where during MM minimization no restraints/constraints were used             |
|                                            |            |                                                                                                             |                          
| energy_multi_conf_rmsd_mol.dat             | kcal/mol   | RMSD compared to QM for relative energies for CREST geometries calculated for each molecule                 |
| energy_multi_conf_rmsd_mol_no_cons.dat     | kcal/mol   | Same as energy_multi_conf_rmsd_mol.dat, where during MM minimization no restraints/constraints were used    |
|                                            |            |                                                                                                             |
| multi_conf_atom_rmsd.dat                   | Angs       | All-Atom RMSD comparing QM and MM CREST geometries                                                          |
| multi_conf_atom_rmsd_no_cons.dat           | Angs       | Same as multi_conf_atom_rmsd.dat, where during MM minimization no restraints/constraints were used          | 
|                                            |            |                                                                                                             | 
| multi_conf_atom_rmsd_per_mol.dat           | Angs       | Average computed for each compound using all-atom RMSD comparing QM and MM CREST geometries                 |
| multi_conf_atom_rmsd_per_mol_no_cons.d     | Angs       | Same as multi_conf_atom_rmsd_per_mol.dat,  where during MM minimization no restraints/constraints were used |

For the entire dataset, MAE, RMSD, R^2 are contained in files with "summary" in the filename:
energy_multi_conf_no_cons_summary.dat
eq_values_summary.dat
energy_multi_conf_summary.dat
min_geom_summary.dat
pes_scaled_energy_summary.dat
pes_energy_summary.dat
multi_conf_atom_rmsd_summary.dat
