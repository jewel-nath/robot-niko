# CAD — the team's working 3D models

The working STL files for every printed part of Niko, as used for the build —
343 files, ~121 MB, organized by body part. Folder names carry the piece
numbers from the build plan; file names carry the part name and version
(`V2`, `V4`, ...), so earlier iterations sit next to the final prints.

| Folder | Body part |
|---|---|
| `1-31 Head` | skull, face plates, jaw |
| `21-26, 121-127 Eye Mechanism` | eyes and lids |
| `29-66 Neck` | neck segments |
| `44-60 83-87 RH` / `67-82 Left Hand` | right and left hands |
| `88-93, 128-131 Fore arm servo bed` | forearm servo beds |
| `94-117 187-204 Bicep` | biceps |
| `119-120 Ear` | ear pieces |
| `132-135 Rotational Wrist` | wrist rotation |
| `136-158 215-222 Shoulder` | shoulders |
| `159-186 Back` | back frame |
| `205-213 Torso` / `223-250 Top Stomach` / `251-260 Mid Stomach` / `Low Stomach` | torso and stomach stack |
| `Chest` | chest plates |
| `Legs Ankle` / `Legs Knee` / `Legs Thigh` / `Legs Tibia` | legs |
| root | `Niko.stl` (full assembled model), TFT display frames, round servo arm |

The body took about 11 months and 329+ printed pieces; see the
[technical report](../docs/report/robot-niko-report.pdf)
([doi:10.5281/zenodo.23719561](https://doi.org/10.5281/zenodo.23719561)) for
print settings, orientation and the assembly order.

## License

Niko is based on [InMoov](https://inmoov.fr/), Gaël Langevin's open-source
robot, whose parts are released under Creative Commons BY-NC-SA — the derived
parts here carry that license, with credit to InMoov. The team's custom parts
(Niko's head design, servo beds, TFT frames and body panels) are the team's
own work.
