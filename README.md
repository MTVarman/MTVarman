# Michael Varman

Independent structural bioinformatics · Wasilla, Alaska

I audit public protein-structure data for errors that carry into the models trained on it: mutations recorded as wildtype, conformational labels that don't match the deposited structure, and protein–ligand covalent bonds that are in the coordinates but missing from the connectivity records. When the error is in someone's dataset, I report it to the maintainers with a reproducer.

I run [Morphogenesis Analytics](https://morphalytica.com), a structural bioinformatics platform, on my own.

## Public record

| Date | What | Where |
|---|---|---|
| Nov 2026 | *Undeclared substitutions in PDB entries do not track source organism; reference curation does* (preprint): across 44,607 entities from eight organisms, undeclared point substitutions do not track organism, but 70% of pig, 37% of dog, 20% of cat and 5% of horse entities have no same-species reviewed UniProt record to check a wildtype label against | [Zenodo 10.5281/zenodo.24194208](https://doi.org/10.5281/zenodo.24194208) |
| Nov 2026 | *Anchor bonds of heme c and light-sensing pigments that are missing from Protein Data Bank connectivity records, and the 2.0 Å line that decides most of them* (technical note): 1,049 of 9,251 heme c and 3,885 of 13,972 phycobilin anchor bonds have no bond record, including 999 of the 1,004 heme c bonds modelled at 2.0 Å or more | [Zenodo 10.5281/zenodo.24153068](https://doi.org/10.5281/zenodo.24153068) |
| Nov 2026 | At default settings, cctbx gives a lysine NZ within 2.20 Å of an ATP oxygen a bond restraint at 1.297 Å, sigma 0.01 (fragments, script and output) | [pdb-data-audits: n-o-link](https://github.com/MTVarman/pdb-data-audits/tree/main/release-audit/default-values/n-o-link) |
| Nov 2026 | 78 of 191 Top-1-correct entries put the warhead beyond any covalent bond distance in the benchmark's own ground truth | [hf1s/CoFD-Bench #1](https://github.com/hf1s/CoFD-Bench/issues/1) |
| Nov 2026 | Any zinc with fewer than four Cys/His ligands is restrained to 2.30 Å by default (222 of 723 cryo-EM entries with such a site carry it; high-resolution X-ray says 2.03 Å) | [cctbx/cctbx_project #1301](https://github.com/cctbx/cctbx_project/issues/1301) |
| Nov 2026 | Chlorophyll Mg–His is linked by default and restrained to 1.895 Å, then 2.300 Å after a June 2024 change, sigma 0.01 (X-ray: 2.20 Å) | [cctbx/cctbx_project #1300](https://github.com/cctbx/cctbx_project/issues/1300) |
| Nov 2026 | *Two default metal restraints in cctbx/PHENIX and their exact-value fingerprints in the Protein Data Bank* (technical note): zinc restrained to 2.30 Å and chlorophyll magnesium to 1.895 Å by default settings, traced to the code, run on twelve builds, and counted across the archive | [Zenodo 10.5281/zenodo.24150338](https://doi.org/10.5281/zenodo.24150338) |
| Nov 2026 | Weekly audit of each PDB release: heme c bond-record parity, atoms closer than any real bond, unrecorded contacts, distances on a software default | [pdb-data-audits: release-audit](https://github.com/MTVarman/pdb-data-audits/tree/main/release-audit) |
| Nov 2026 | Ligand-induced set: 188 of 350 pairs have different substitutions on the two sides | [seoklab/promise-bench #13](https://github.com/seoklab/promise-bench/issues/13) |
| Oct 2026 | `ligand_is_covalent` is False for 256 of 266 entries whose coordinates carry a protein–ligand bond with no bond record | [plinder-org/plinder #136](https://github.com/plinder-org/plinder/issues/136) |
| Oct 2026 | *Co-folding models execute covalent bonds they do not propose, and pose RMSD certifies the difference away* (preprint) | [Zenodo 10.5281/zenodo.23763023](https://doi.org/10.5281/zenodo.23763023) |
| Oct 2026 | Audit tables archived as a citable dataset (current version v1.4.0, Nov 2026) | [Zenodo 10.5281/zenodo.23441847](https://doi.org/10.5281/zenodo.23441847) |
| Oct 2026 | Audit tables and reproducers: 485-site strict cut of unrecorded covalent bonds, LP-PDBBind cross-check, benchmark overlap, corrected Rascore table | [MTVarman/pdb-data-audits](https://github.com/MTVarman/pdb-data-audits) |
| Oct 2026 | Identical ligand on the same protein labelled both covalent and non-covalent, 11 entries | [THGLab/LP-PDBBind #8](https://github.com/THGLab/LP-PDBBind/issues/8) |
| Oct 2026 | Mutation status defaults to wildtype when the mutated residue isn't modeled (38 chains, mostly KRAS Q61H) | [mitch-parker/rascore #2](https://github.com/mitch-parker/rascore/issues/2) |
| Oct 2026 | *Silent Mutation Misclassification and Unrecorded Covalent Bonds in the Protein Data Bank* (preprint) | [Zenodo](https://doi.org/10.5281/zenodo.23380304) |

## Elsewhere

- ORCID: [0009-0001-9453-0226](https://orcid.org/0009-0001-9453-0226)
- LinkedIn: [Michael Varman](https://www.linkedin.com/in/michael-varman-595563130)
