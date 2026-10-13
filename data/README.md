# Data provenance: cotton-fibre XRD pattern

**Status:** Day 1 record complete.

**Important:** This project analyses a published dataset. I did not collect these data or operate the instrument.

## 1. Source article

| Field | Record |
| --- | --- |
| Title | Open-source Rietveld refinement for cellulose crystallinity using a laboratory powder X-ray diffractometer: a hands-on tutorial |
| Authors | Sunghyun Nam, Alfred D. French, Md Nayeem Hasan Kashem |
| Journal | Cellulose (Springer Nature) |
| Year | 2026 (published online 16 September 2026) |
| DOI | https://doi.org/10.1007/s10570-026-07136-7 |
| Article page | https://link.springer.com/article/10.1007/s10570-026-07136-7 |
| Article licence | Open access, CC BY 4.0, as stated under "Rights and permissions" on the article page |
| Data availability statement | "Data is provided within the manuscript and supplementary information files." |

## 2. Source file

| Field | Record |
| --- | --- |
| File used | Supplementary file 1 (TEXT; the article page lists 15 KB) |
| Original filename | 10570_2026_7136_MOESM1_ESM.txt |
| Name used in the article text | cotton.txt |
| Download date | 2026-10-12 |
| Size on disk | File size | 14.5 KB (16.0 KB allocated on disk) |
| Expected local location | data/raw/10570_2026_7136_MOESM1_ESM.txt |
| Other supplementary files | Files 2 to 6 (two CIF files, a PAR analysis file, a PDF guide, an XLSX of refinement output) were not used. File 6 contains computed refinement output, not the raw measurement. |

## 3. Sample and measurement (article-reported, not stored in the data file)

| Item | Article-reported |
| --- | --- |
| Sample | Cotton fibres grown at the USDA Southern Regional Research Center (New Orleans), ground in a Wiley mill with a 40-mesh screen. The pattern comes from ground cotton powder, not intact fibres. |
| Instrument | Empyrean diffractometer (Malvern Panalytical) |
| Radiation | Cu K-alpha, average wavelength 1.5418 Å, nickel filter |
| Scan reported in the article | 2θ from 5 to 80 degrees, step 0.039 degrees, spinning holder, variable divergence slits, room temperature |
| Instrument calibration | The article states that no separate instrument calibration was performed for this tutorial. |

## 4. What I observed in the file itself

| Item | Observation |
| --- | --- |
| Number of columns | 2 |
| Column order | First column looks like 2θ angle (degrees), second like intensity. This matches the article's statement that input files are two columns: 2θ and intensity. |
| Header line | No. The first line is already data. |
| Delimiter | Whitespace between the two values |
| First three lines | 9.88213312	6539 / 9.92152397	6739 / 9.96091482	6593 |
| Last three lines | 41.78872002	7622 / 41.82811087	7618 / 41.86750172	7661 |
| Number of data rows | 813 |
| Angle range in file | 9.88213312 to 41.86750172 |
| Approximate step | 0.03939 |
| Intensity format | Integers only, no decimals, no scientific notation. Magnitude: thousands to tens of thousands (6,539 to 47,186) |
| Intensity range | Minimum 6539 and maximum 47186, as observed in file (maximum near 2θ 22.68°) |
| Intensity units | Not stated in the file; scaling status unknown |
| Encoding / line endings | UTF-8; Windows (CRLF) line endings (read from the Notepad status bar) |
| Anything unusual | Nothing noted |
| Agreement with article | Partial. The article-reported scan is 5-80° 2θ with a 0.039° step. The step agrees (0.03939° rounds to 0.039°). The range does not: the file covers 9.88° to 41.87° only |

## 5. Licence and redistribution decision

- What the article page states: The article is open access under CC BY 4.0, which allows sharing and adapting with attribution. A data availability statement says the data are in the article and its supplementary files. The page also carries a notice that the article is a U.S. Government work, not under copyright in the US, with foreign copyright possibly applying.
- Separate licence for the supplementary files: Not stated on the page.
- **Decision (Day 1):** The raw file is NOT committed to this repository. It is kept locally in `data/raw/`, which is listed in `.gitignore`.
- To be revisited on Day 4 before the v0.1 release.

## 6. How to obtain the file

1. Open https://doi.org/10.1007/s10570-026-07136-7
2. Scroll to "Supplementary Information".
3. Download "Supplementary file1" (TEXT).
4. Place it at `data/raw/10570_2026_7136_MOESM1_ESM.txt`, keeping the original filename.

## 7. Citation

Nam, S., French, A. D., & Kashem, M. N. H. (2026). Open-source Rietveld refinement for cellulose crystallinity using a laboratory powder X-ray diffractometer: a hands-on tutorial. Cellulose. https://doi.org/10.1007/s10570-026-07136-7