# Evidence and research method

This repository is a **summary snapshot**, not the full computational archive.
It is intended to be easy to read on GitHub. Code, large catalogs, downloaded
research images and raw logs remain in the separate working directory
`../kryptos`.

The file paths below are relative to that working archive, not links to files
bundled in this repository. [The manifest](data/evidence-manifest.json) records
SHA-256 hashes and sizes for selected source notes and results at the time of
this snapshot. A hash identifies a file; it does not prove its claims correct.

## What a result means

We separate four kinds of evidence:

1. **A contradiction:** the known letters cannot satisfy a specified rule.
2. **A finite exhaustive test:** all declared settings were checked, with the
   boundary stated explicitly.
3. **A feasible construction:** a setting fits the known letters, possibly with
   many arbitrary choices still free.
4. **A language-search result:** a heuristic finds a text that scores well.

Only the first two can support a scoped exclusion. The latter two need further
evidence. A timeout means UNKNOWN. A search that recovers generated examples
demonstrates some capability, but does not prove it covers all possible keys.

Our usual checks include published known-answer examples, generated 97-letter
messages containing the same public clues, independent implementations, exact
re-encryption and comparisons with shuffled or random controls where a language
score is used. Validation varies by experiment; the detailed notes give the
actual coverage rather than a blanket “verified” label.

## Working archive index

| ID | Topic | Principal notes or records in the working archive |
| :--- | :--- | :--- |
| E01 | Input, simple invariants and early tests | `data/k4.json`; `RESEARCH.md` |
| E02 | Periodic keywords and free alphabet completions | `experiments/periodic_keyword_models.md`; `results/free_key_completion_enumeration.json` |
| E03 | Quagmire feasibility and recovery limits | `experiments/quagmire_free_periods.md`; `experiments/quagmire_graph_search.md`; `results/quagmire_graph_audit.json`; `results/quagmire_graph_reproduction/manifest.json`; `experiments/quagmire_plaintext_beam.md`; `experiments/quagmire_sparse_beam.md`; `results/quagmire_sparse_audit.json`; `results/quagmire_sparse_peer_output_audit.json`; `RESEARCH.md` |
| E04 | Routes, counting and K3-derived operations | `BLUE_SKY.md`; `RESEARCH.md` |
| E05 | Compass reading orders | `experiments/bearing_routes.md`; `results/exact_compass_weak_fit.json` |
| E06 | Nicodemus | `experiments/nicodemus.md`; `results/nicodemus_hall.json`; `results/nicodemus_subset.json`; `results/nicodemus_actual.json` |
| E07 | Turning grilles | `experiments/turning_grille.md`; `results/grille_periodic_recount.json`; `results/grille_quarter_shuffle.json`; `results/grille_dictionary.json`; `results/grille_orbit_solver.json`; `results/grille_orbit_peer_audit.json`; `results/grille_keyword_phases.json`; `results/grille_phase_geometry.json`; `results/grille_phase_peer_audit.json`; `results/grille_counterclockwise.json` |
| E08 | Single rotors and ring layouts | `experiments/clock_rotor_exact.md`; `experiments/clock_rings.md` |
| E09 | Coupled wheels and free alphabets | `experiments/clock_continuous_pair.md`; `experiments/clock_full97_exact.md`; `experiments/clock_two_alphabets.md` |
| E10 | Feedback, row resets and controls | `experiments/feedback_rotor.md`; `experiments/feedback_rotor_rows.md`; `experiments/feedback_rotor_prestep.md`; `experiments/clock_feedback_model_competition.md`; `experiments/clock_column_reset.md` |
| E11 | Sector lookup tables and ciphertext overlays | `experiments/clock_label_table.md`; `experiments/ciphertext_overlay.md` |
| E12 | Unknown spaces | `experiments/clock_omitted_spaces.md` |
| E13 | Trigger disks and resets | `experiments/trigger_disk_dictionary.md`; `experiments/trigger_reset.md`; `experiments/plaintext_trigger_reset.md` |
| E14 | Changing alphabets | `experiments/chaocipher_keyword_left.md`; `RESEARCH.md` |
| E15 | Word counters and common restarts | `experiments/ragbaby_obstruction.md`; `results/common_word_reset_obstruction.json` |
| E16 | Other direct hand mechanisms | `experiments/slidefair.md`; `experiments/condi.md`; `experiments/wheatstone.md`; `experiments/portax_obstruction.md` |
| E17 | Gromark | `k4/bluesky/README.md`; `results/gromark_dictionary.json` |
| E18 | Fractionation and Morse | `BLUE_SKY.md`; `RESEARCH.md`; `k4/cube_check/README.md` |
| E19 | Carter lecture running keys | `experiments/carter_lecture.md` |
| E20 | Keyword alphabet constructions | `experiments/column_keywords.md`; `experiments/clock_city_panel_alphabets.md` |
| E21 | Historical World Clock evidence | `experiments/clock_historical_sources.md`; `experiments/clock_orientation_review.md`; `k4/clock_orientation/README.md`; `HUMAN_CLUES.md` |
| E22 | Archive photographs and human interpretations | `experiments/archive_photo_review.md`; `experiments/null_padding_source_review.md`; `HUMAN_CLUES.md` |
| E23 | Amsco with shifts attached to grid columns | `experiments/amsco.md`; `results/amsco_columns.json`; `results/amsco_geometry_audit.json`; `results/amsco_dictionary.json`; `results/amsco_peer_audit.json` |
| E24 | Original clue letter and current archive sources | `experiments/sanborn_letter_review.md`; `k4/sanborn_letter_2025_11_12/`; `experiments/paradigm_source_review.md`; `data/paradigm_archive/manifest.json` |
| E25 | Sensitivity to hypothetical ciphertext substitutions | `experiments/error_budget_review.md`; `results/columnar_one_error_audit.json`; `results/structural_error_bounds.json`; `results/transposition_error_recount.json`; `results/word_reset_one_error/results.json`; `k4/error_audit/`; `k4/fable/` |
| E26 | Physical panel versus published representation | `experiments/cia_panel_layout.md`; `experiments/cia_panel_transcription.py`; `data/cia_panels/manifest.json`; `k4/panel_sources/README.md` |
| E27 | Conditional Carter openings and English controls | `experiments/carter_conditional.md`; `experiments/carter_discrimination_audit.py`; `results/carter_discrimination_audit.json`; `experiments/quagmire_linear_filter.py`; `results/quagmire_linear_filter.json`; `k4/error_audit/verify_carter_witnesses.py`; `k4/fable/b2/frozen.json` |
| E28 | Forced-letter projection and periodic repetition controls | `experiments/quagmire_projection_controls.md`; `experiments/quagmire_projection_controls_plan.md`; `results/quagmire_projection_controls.json`; `results/quagmire_projection_audit.json`; `results/periodic_coincidence_audit.json`; `results/periodic_coincidence_peer_audit.json`; `k4/quagmire_beam_ref/projection_audit.json` |
| E29 | Published-row edge keys and fixed substitution per row | `experiments/panel_edge_keys.md`; `experiments/panel_edge_key_audit.py`; `results/panel_edge_key_audit.json`; `k4/fable/b6/edge_keys.py`; `k4/rowwise_mono/README.md`; `k4/rowwise_mono/rowwise_mono.json` |

Some older running-status paragraphs in the working notebooks are historical
entries. The latest completed result takes precedence over an earlier plan.
This summary does not infer that a job is alive from an old assignment.

## Sources worth starting with

| Source | What it contributes | Caution |
| :--- | :--- | :--- |
| [CIA: Kryptos sculpture](https://www.cia.gov/legacy/headquarters/kryptos-sculpture/) | Official background, physical features and transcription | Historical status language is not a live global solve registry |
| [Richard Bean's research](https://kryptos.richardbean.id.au/) and [2021 paper](https://ecp.ep.liu.se/index.php/histocrypt/article/download/153/109) | Prior cryptanalysis, public clues and methods to compare against | Reproducing earlier work is validation, not a new discovery |
| [Sanborn's original November 2025 letter](https://s3.documentcloud.org/documents/26229389/adobe-scan-nov-12-2025.pdf) | Both scanned pages independently read: plaintext influences, World Clock identification and K5 description | OCR corrupts reading order; the letter's 1988/1989 chronology remains inconsistent |
| [Scientific American clue report](https://www.scientificamerican.com/article/cia-kryptos-puzzle-creator-releases-final-clues/) | Reporting on the World Clock and later contextual clues | Keep event reporting distinct from the author's original text |
| [Paradigm's announcement](https://www.paradigm.xyz/writing/kryptos) and [archive gallery](https://www.paradigm.xyz/kryptos/archive) | Current stewardship, verification system and public photographs | Some gallery captions misidentify the images; read the originals, not just their labels |
| [Sanborn interview, Wired](https://www.wired.com/2005/01/questions-for-kryptos-creator/) | The artist's account of his process | Visual/manual language does not specify an algorithm |
| [Scheidt interview, Wired](https://www.wired.com/2005/01/inside-info-on-kryptos-codes/) | Cryptographic context and masking discussion | Do not assume a particular extra layer from the word “masking” |
| [Smithsonian oral history](https://www.aaa.si.edu/collections/interviews/oral-history-interview-jim-sanborn-15700) | First-person historical context | References to already solved sections cannot silently become K4 instructions |
| [PBS NOVA transcript, July 2007](https://www.pbs.org/wgbh/nova/transcripts/3411_sciencen.html) | Identifies speakers and links the graph-paper demonstration to K3 | Vowel removal and phonetic spelling are the correspondent's examples, not Sanborn naming K4's method |
| [Kunsch clock mechanism](https://kunsch-metallbau.de/referenzen-/weltzeituhr-berlin-alexanderplatz/) | Mechanical background for the Alexanderplatz clock | Physical rates do not themselves define letter operations |
| [Kinemathek photograph, 3 October 1990](https://wwsf.deutsche-kinemathek.de/index.php/Detail/Object/Show/object_id/1612/lang/en_US) | Dated evidence for actual clock lettering | Partial view; not a complete 1989 roster |
| [ACA cipher descriptions](https://www.cryptogram.org/resource-area/cipher-types/) | Explicit hand-cipher definitions and known-answer examples | A historical mechanism's existence is not evidence Sanborn selected it |
| [RR Auction's archival-discovery account](https://content.rrauction.com/kryptos-k4-discovered-not-solved-heres-what-actually-happened/) | Distinguishes recovering text from deriving the cryptographic method | The auction house was an interested participant in the sale |

## Reproducing a particular claim

Use the evidence ID to locate the detailed experiment note in the working
archive. Check its definition, input hashes, search boundary and validation
records before running its documented command. Compare saved output with the
manifest for this snapshot. Do not assume the summary repo alone contains the
inputs needed to repeat a multi-million-setting search.

The long-term target is a compact reproducible package for the decisive result:
the input, key, explicit algorithm, all 97 recovered letters, exact re-encryption
and an independent verifier. That package does not exist yet because the
objective has not been achieved.
