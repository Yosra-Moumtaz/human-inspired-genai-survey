# Supplementary material: Human-Inspired Generative AI: A Critical Review of Sequential and Structured Generation Approaches (2016-2026)

Authors: Yosra Moumtaz (1, corresponding author, y.moumtaz@mundiapolis.ma), Mohamed-Amine Chadi (2), Samar Mouchawrab (1)

(1) Research, Development, and Innovation Laboratory, Mundiapolis University, Casablanca, Morocco  
(2) Laboratory of Computer Science and Intelligent Systems, Faculty of Sciences Semlalia, Cadi Ayyad University, Marrakech, Morocco

This dataset accompanies the conference paper above. It documents the corpus, the screening decisions and the coding of the reviewed generative approaches, so that every count reported in the paper can be recomputed.

## Files

| File | Content |
|---|---|
| `S1_coding_generative_works.xlsx` | Coding of the 50 generative approaches (sheet `Coding_generative_works`), coding rules (`Coding_rules`) and aggregate counts (`Summary_counts`) |
| `S2_corpus.xlsx` | The 74 candidate records with status, origin, metadata and verification status (`Corpus`), the 58 unique Consensus records with screening decisions (`Consensus_screening`), legend (`Legend`) |
| `S3_systematic_search_and_screening.xlsx` | Systematic search of arXiv and OpenAlex run on 2026-11-15: exact queries and hit counts (`Queries`), screening of every arXiv and OpenAlex record with decision and reason (`arXiv_screening`, `OpenAlex_screening`), the 162 new generative approaches and 10 other new inclusions (`Included_new`), PRISMA counts (`Counts`), criteria and notes (`Legend`) |
| `*.csv` | The same sheets in CSV (UTF-8) |

## Systematic search (S3)

- Sources: arXiv API and OpenAlex API (field Computer Science, publication years 2016-2026), run on 2026-11-15 with four Boolean queries (exact strings in `S3_Queries.csv`).
- 2,122 hits (496 arXiv, 1,626 OpenAlex); 1,790 unique records after removing duplicates within and across sources; 55 already in the core corpus; 1,735 screened on title and abstract by one author.
- Decisions: 1,539 excluded, 24 unresolved (no usable abstract), 172 included (162 generative approaches, 10 other works). A reason is recorded for every record.
- Level 1 maps 212 generative approaches (50 core + 162 new); Level 2 codes the 50 core approaches (S1).
- Scopus, Web of Science and IEEE Xplore were not queried; ready-to-run queries are in `search_protocol/Search_log.xlsx`.
- `search_protocol/raw/` holds the raw API results (arXiv Atom entries and OpenAlex records) used for screening.

## Exploratory search and core corpus (S2)

- Three Consensus searches on (1) foundational sequential and human-inspired generation, (2) handwriting, motor behaviour, trajectory and program-based generation, (3) evaluation methodologies: 60 records, 58 unique (18, 20, 20). The exact query strings were not archived.
- Screening: 31 retained, 27 excluded (reason per record in `Consensus_screening`).
- Targeted searches of proceedings, publisher sites and DBLP, and backward/forward snowballing: 43 records.
- 74 candidates; 1 excluded after verification (game imitation, outside scope); final corpus of 73 records: 50 coded generative approaches and 23 other records (surveys, evaluation methods, datasets, cognitive studies).

## Coding dimensions (S1)

| Column | Values | Meaning |
|---|---|---|
| Eval. target | O, S, P | output, structure, process |
| Human data used for TRAINING | none, outputs, process, ? | human process = stroke sequences, trajectories or videos of making |
| D | Y, N, ? | explicit cognitive, perceptual or motor inspiration in the design |
| J | Y, N, ? | humans rate, prefer or classify generated outputs |
| P | Y, N, ? | generated order, trajectory, kinematics or temporal progression compared quantitatively with recorded human data |
| B | Y, N, ? | model compared with a population of human participants (accuracy patterns, errors, variability, choices) |

D, J, P and B are independent dimensions, not a scale. `?` means not determinable from the consulted sources. Codes were assigned from abstracts and official pages and revised by full-text reading where available; the evidence for revised codes is in column `Basis / note`. Coding was done by a single coder.

## Main counts (n = 50)

Trained on human process data 29; D 13; J 15; P 10; B 5; no J, P or B confirmed 26; J, P and B all coded N 24; entries with at least one `?` 7; preprints 5.

## Licence

CC BY 4.0.

## How to cite

Moumtaz, Y., Chadi, M.-A., Mouchawrab, S.: Human-Inspired Generative AI: A Critical Review of Sequential and Structured Generation Approaches (2016-2026). Submitted to ICBDAIA'27. Dataset DOI or repository link: TODO once assigned.
