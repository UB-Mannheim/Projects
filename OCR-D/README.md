# OCR-D Projektdokumentationen

Dieses Repository dokumentiert Projektergebnisse der _Koordinierten Förderinitiative zur Weiterentwicklung von Verfahren der Optical Character Recognition_ ([OCR-D](https://ocr-d.de/)), an der die [Universitätsbibliothek Mannheim](https://www.bib.uni-mannheim.de/) mit  Modul- und Implementierungsprojekten beteiligt gewesen ist. 

OCR-D wird durch die [Deutsche Forschungsgemeinschaft (DFG)](https://www.dfg.de/) gefördert.

-------------------------

## Workflow für werk­spezifisches Training auf Basis generischer Modelle mit OCR-D sowie Ground-Truth-Aufwertung
**Modulprojekt | Laufzeit: 2021–2023**

*[WIP]* In diesem Modulprojekt wurden sowohl Ground-Truth-Korpora als auch softwaretechnische Werkzeuge zur bearbeitung von Ground Truth erstellt. Darüber hinaus wurde eine werkspezifischer Trainingsworkflow auf Basis von eScriptorium erstellt.

### 1. Software
- [PagePlus](https://github.com/UB-Mannheim/PagePlus)
- [eScriptorium](https://github.com/UB-Mannheim/eScriptorium)
- [OCR-D format converters](https://github.com/OCR-D/format-converters/)
  - [page2img](https://github.com/OCR-D/format-converters/blob/master/page2img.py)

### 2. Ground-Truth-Korpora
Die im Projekt erstellten und überarbeiteten Ground-Truth-Korpora wurden auf Basis der [OCR-D GT Guidelines](https://ocr-d.de/de/gt-guidelines/trans/) im [Level 2](https://ocr-d.de/de/gt-guidelines/trans/level_2_2.html) erstellt.

- [GT4HistOCR](https://code.bib.uni-mannheim.de/ocr-d/GT4HistOCR)
- [digi-gt](https://github.com/UB-Mannheim/digi-gt)
- [Fibeln](https://github.com/UB-Mannheim/Fibeln)
- [digitue-gt](https://github.com/UB-Mannheim/digitue-gt)
- [Weisthuemer](https://github.com/UB-Mannheim/Weisthuemer)
- [dach-gt](https://github.com/UB-Mannheim/dach-gt)
- [reichsanzeiger-gt](https://github.com/UB-Mannheim/reichsanzeiger-gt)
  - Schmidt, T., Kamlah, J., Weil, S., & Shigapov, R. (2023). UB-Mannheim/reichsanzeiger-gt: 1.1.0 - Fix for baselines and some typos (1.1.0). Zenodo. [https://doi.org/10.5281/zenodo.10144095](https://doi.org/10.5281/zenodo.10144095)
- [hkb-gt](https://github.com/UB-Mannheim/hkb-gt)
- [charlottenburger-amtsschrifttum](https://github.com/UB-Mannheim/charlottenburger-amtsschrifttum)
- [AustrianNewspapers v2.0.0](https://github.com/UB-Mannheim/AustrianNewspapers)
- [NZZ-black-letter-ground-truth v2.0.0](https://github.com/UB-Mannheim/NZZ-black-letter-ground-truth)
  - Ströbel, P., Clematide, S. & Weil, S. (2022). impresso/NZZ-black-letter-ground-truth: Im-proved Test Set. Zenodo. [https://doi.org/10.5281/zenodo.7053264](https://doi.org/10.5281/zenodo.7053264)

### 3. Dokumentationen, Anleitungen und Guides
#### 3.1. Trainings-Dokumentationen 
- [kraken](https://github.com/UB-Mannheim/kraken/)
  - [Training german_newspapers](https://github.com/UB-Mannheim/kraken/wiki/Training-German-Newspapers)
- [Training mit Tesseract DE](https://github.com/th-schmidt/docs4training-ocr/blob/main/Training-mit-Tesseract.md)
- [Training mit Tesseract EN](https://github.com/th-schmidt/training-with-tesseract/blob/main/Training-with-Tesseract.md)
- [Training with Charlottenburger Amtsschrifttum](https://github.com/UB-Mannheim/charlottenburger-amtsschrifttum/wiki/Work-specific-training-with-Charlottenburger-Amtsschrifttum)
- [Tesseract Training with AustrianNewspapers](https://github.com/UB-Mannheim/AustrianNewspapers/wiki/Training-with-Tesseract)
- [Kraken Training with AustrianNewspapers](https://github.com/UB-Mannheim/AustrianNewspapers/wiki/Training-with-Kraken)
- [Calamari Training with AustrianNewspapers](https://github.com/UB-Mannheim/AustrianNewspapers/wiki/Training-with-Calamari)
- [Training with digi-gt](https://github.com/UB-Mannheim/digi-gt/wiki/Training)
- [Kraken Training with digitue-gt](https://github.com/UB-Mannheim/digitue-gt/wiki/Training-with-Kraken)

#### 3.2. eScriptorium Dokumentationen
- [eScriptorium Dokumentation](https://github.com/UB-Mannheim/eScriptorium_Dokumentation/)
- [Training with eScriptorium (a step-by-step guide)](https://github.com/UB-Mannheim/eScriptorium_Dokumentation/blob/main/Training-with-eScriptorium.md)

### 4. OCR/HTR-Modelle
Im Projekt wurden neue generische Modelle mit verschiedenen OCR-Engines trainiert.

#### 4.1. Generische OCR/HTR-Modelle
- Weil, S. (2021). Tesseract OCR models for historic prints based on Latin script.
Zenodo. https://doi.org/10.5281/zenodo.10125246
- Weil, S. (2023). Fraktur model trained from enhanced Austrian Newspapers dataset.
Zenodo. https://doi.org/10.5281/zenodo.6891851
- Weil, S. (2023). HTR model for German manuscripts trained from several datasets.
Zenodo. https://doi.org/10.5281/zenodo.7933463
- Weil, S., Kamlah, J., & Schmidt, T. (2023). OCR model for German prints trained from several datasets.
Zenodo. https://doi.org/10.5281/zenodo.10519595

#### 4.2. Modelle zum GT-Korpus *AustrianNewspapers*
- [Tesseract AustrianNewspapers-20230426](https://ub-backup.bib.uni-mannheim.de/~stweil/tesstrain/calamari/AustrianNewspapers-20230426/)
- [Tesseract AustrianNewspapers-20230502](https://ub-backup.bib.uni-mannheim.de/~stweil/tesstrain/tesseract/austriannewspapers/20230502/)
- [Kraken AustrianNewspapers](https://ub-backup.bib.uni-mannheim.de/~stweil/tesstrain/kraken/austriannewspapers/)

#### 4.3. Modelle zum GT-Korpus *Reichsanzeiger-GT*
- [Kraken Reichsanzeiger-GT](https://ub-backup.bib.uni-mannheim.de/~stweil/tesstrain/kraken/reichsanzeiger-gt/)

#### 4.4. Weitere Modelle
- [Tesseract-Modelle auf Basis der digi-gt](https://ub-backup.bib.uni-mannheim.de/~stweil/tesstrain/kraken/digi-gt/)
- [Tesseract-Modelle auf Basis der digitue-gt](https://ub-backup.bib.uni-mannheim.de/~stweil/tesstrain/kraken/digitue-gt/)
- [Calamari-Modelle](https://ub-backup.bib.uni-mannheim.de/~stweil/tesstrain/calamari/)

### 5. Publikationen, Präsentationen und Arbeitspapier
#### 5.1. Präsentationen
- Kamlah, J., & Schmidt, T. (2023). Hands-on Lab Ground Truth-Erstellung und Modelltraining mit eScriptorium, 111. BiblioCon Hannover 2023
- Kamlah, J., & Schmidt, T. (2022). Der Weg zum nutzbaren Volltext. Werkspezifisches Trai-ning als Baustein der OCR-Volltexterkennung für Alte Drucke. 8. Bibliothekskongess Leipzig 2022: #FreiräumeSchaffen, BID, Leipzig, Germany. https://opus4.kobv.de/opus4-bib-info/frontdoor/index/index/docId/17861
- Kamlah, J. & Schmidt, T. (2022). Finetune your OCR! Improving automated text recognition for early printed works by finetuning existing Tesseract models. ELAG 2022, Riga, Latvia. https://dom.lndb.lv/data/obj/file/33561874.pdf

#### 5.2. Arbeitspapiere
- Kamlah, J., & Schmidt, T. (2023). Transkriptionsregeln und Guidelines zur Layoutbearbeitung im DFG-Projekt "Workflow für werkspezifisches Training auf Basis generischer Modelle mit OCR-D sowie Ground-Truth-Aufwertung". Zenodo. https://doi.org/10.5281/zenodo.10203335

-------------------------

## Integration von Kitodo und OCR-D zur produktiven Massendigitalisierung
**Implementierungsprojekt | Laufzeit: 2021–2023**
...
