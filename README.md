# Amine-Lignocellulose Interaction Atlas

Interactive atlas of amine interactions with lignocellulose monomers: non-covalent docking and DLPNO-CCSD(T)/LED energies, proton-transfer paths, a reaction network, and nucleophilic reaction paths.

**Live site:** `https://<your-username>.github.io/<repo-name>/`

## Files
| File | Role |
|---|---|
| `index.html` | Main page (tabs: Overview, Interaction Atlas, Proton Transfer, Reaction Network, Nucleophilic Reactions) |
| `atlas.html`, `proton.html`, `nucleophilic.html` | Embedded views |
| `library.json` | 72 complexes: geometry, contacts, docking and LED energies |
| `overview.json`, `network.json`, `reactions.json` | Overview table, reaction network, proton-transfer paths |

## Run locally
The pages load JSON with `fetch`, so open them through a server, not by double-click:
```
python -m http.server 8000
```
then visit http://localhost:8000.

## Notes
- DLPNO-CCSD(T) interaction energies are available for 49 of 72 pairs, CCSD-only for 16, none yet for 7. Unfinished jobs are being rerun; the atlas will be updated.
- Network and NEB paths: GFN2-xTB with ALPB(water).
- Licence: data CC BY 4.0 (see `.zenodo.json`, `CITATION.cff`). Add a LICENSE file with the code licence you prefer.

Author: Taiwo Zacchaeus Adesanya, University of Illinois Chicago.
