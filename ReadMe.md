### Configurator for [Branches of Study at TU Braunschweig][1]

The configurator is a runnable JAR file requiring Java 8 or newer.  
As it will need about 4.5min to load the configuration data, its window
will not be responsive during that startup time.

The `Undefined` list at the center contains all possible subjects of study, such as
courses, theses, labs, and the branches of study.
You can select or deselect subjects by clicking them and using the arrow buttons to push them into
the corresponding lists. Subjects below the dotted line (`-----`) are de-/selected automatically.

At the top left you will find the `Configuration Status`, indicating if all constraints
for a correct selection of subjects are fulfilled.
Your configuration becomes valid iff a master thesis and a seminar are chosen.
Furthermore, if a branch of study (e.g. `Studienrichtung IT-Security`...) is selected,
the configuration will not become valid before all necessary constraints for the branch are met, too.
For example, the [branch "Studienrichtung IT-Security"][2] has the following constraints
(the subjects are listed in german according to the websites and tools specification):

- Compulsory (Pflicht) (35 CP)
   - Seminar IT‐Sicherheit (5 CP)
   - Masterarbeit IT‐Sicherheit (30 CP)

- Compulsory Elective (Wahlpflicht) (35 CP)
   - Fortgeschrittene IT‐Sicherheit (5 CP)
   - Maschinelles Lernen in der IT‐Sicherheit (5 CP)
   - Praktikum IT‐Sicherheit (5 CP)
   - Praktikum Intelligente Systemsicherheit (5 CP)
   - Projektarbeit (15 CP)
   - Management von Informationssicherheit (5 CP)
   - Betriebssystemsicherheit (5 CP)

If this branch is chosen, "Seminar IT‐Sicherheit" and "Masterarbeit IT‐Sicherheit" will be selected automatically, as these are mandatory.
Additionally, you have to choose subjects from the compulsory elective pool such that at least 35 credit points are reached.

Thus, you can choose any subjects you are interested in or might already have attended and see if you could graduate in the branch you desire.

### Limitations

Currently, not all branches of study are supported.  
Suppored are:
  + Big Data Management
  + IT-Security
  + Visual Computing
  + Industrial Data Science
  + Robotik

The following branches are not yet supported and thus are deselected automatically:
  - Fahrzeuginformatik
  - Hardware-/Softwaresystementwurf und -analyse
  - Medizinische Informatik
  - Networked Systems.

### Implementation
For further information on implementation and model please visit https://github.com/PaulAtTUBS/BroT.

[1]: https://www.tu-braunschweig.de/informatik-msc/struktur/studienrichtungen
[2]: https://www.tu-braunschweig.de/informatik-msc/struktur/studienrichtungen/it-sicherheit