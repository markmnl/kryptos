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
| E03 | Quagmire feasibility and recovery limits | `experiments/quagmire_free_periods.md`; `experiments/quagmire_graph_search.md`; `results/quagmire_graph_audit.json`; `results/quagmire_graph_reproduction/manifest.json`; `experiments/quagmire_plaintext_beam.md`; `experiments/quagmire_sparse_beam.md`; `experiments/quagmire_full_certify.md`; `results/quagmire_full_certify_audit.json`; `experiments/quagmire_parity_obligations.md`; `experiments/quagmire_projective_certify.md`; `results/quagmire_projective_audit.json`; `RESEARCH.md` |
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
| E21 | Historical World Clock evidence | `experiments/clock_historical_sources.md`; `experiments/clock_orientation_review.md`; `experiments/clock_film_sources_review.md`; `k4/clock_orientation/README.md`; `HUMAN_CLUES.md` |
| E22 | Archive photographs and human interpretations | `experiments/archive_photo_review.md`; `experiments/archive_photo_review_addendum.md`; `results/archive_photo_review_addendum/`; `experiments/null_padding_source_review.md`; `HUMAN_CLUES.md` |
| E23 | Amsco with shifts attached to grid columns | `experiments/amsco.md`; `results/amsco_columns.json`; `results/amsco_geometry_audit.json`; `results/amsco_dictionary.json`; `results/amsco_peer_audit.json` |
| E24 | Original clue letter and current archive sources | `experiments/sanborn_letter_review.md`; `k4/sanborn_letter_2025_11_12/`; `experiments/paradigm_source_review.md`; `data/paradigm_archive/manifest.json` |
| E25 | Sensitivity to hypothetical ciphertext substitutions | `experiments/error_budget_review.md`; `results/columnar_one_error_audit.json`; `results/structural_error_bounds.json`; `results/transposition_error_recount.json`; `results/word_reset_one_error/results.json`; `k4/error_audit/`; `k4/fable/` |
| E26 | Physical panel versus published representation | `experiments/cia_panel_layout.md`; `experiments/cia_panel_transcription.py`; `data/cia_panels/manifest.json`; `k4/panel_sources/README.md` |
| E27 | Conditional Carter openings and English controls | `experiments/carter_conditional.md`; `experiments/carter_discrimination_audit.py`; `results/carter_discrimination_audit.json`; `experiments/quagmire_linear_filter.py`; `results/quagmire_linear_filter.json`; `k4/error_audit/verify_carter_witnesses.py`; `k4/fable/b2/frozen.json` |
| E28 | Forced-letter projection and periodic repetition controls | `experiments/quagmire_projection_controls.md`; `experiments/quagmire_projection_controls_plan.md`; `results/quagmire_projection_controls.json`; `results/quagmire_projection_audit.json`; `results/periodic_coincidence_audit.json`; `results/periodic_coincidence_peer_audit.json`; `k4/quagmire_beam_ref/projection_audit.json` |
| E29 | Published-row edge keys and fixed substitution per row | `experiments/panel_edge_keys.md`; `experiments/panel_edge_key_audit.py`; `results/panel_edge_key_audit.json`; `k4/fable/b6/edge_keys.py`; `k4/rowwise_mono/README.md`; `k4/rowwise_mono/rowwise_mono.json` |
| E30 | Word boundaries and lexical support of recovery benchmarks | `experiments/quagmire_word_support.md`; `experiments/quagmire_wordbench.md`; `results/quagmire_word_support.json`; `results/quagmire_word_probe_audit.json`; `results/quagmire_wordbench_audit.json`; `k4/wordbench/fixtures.json`; `k4/quagmire_beam_ref/word_support_check.json` |
| E31 | Word decoder implementation review | `experiments/wordbeam_engine_review.md`; `experiments/wordbeam_v21_engine_audit.py`; `results/wordbeam_v21_engine_audit.json`; `results/wordbeam_fixed_text_audit.json`; `results/wordbeam_stage1_audit.json`; `results/wordbeam_development_summary.json`; `experiments/wordbeam_pruning_trace.md`; `results/wordbeam_recombination_counterexample.json`; `k4/fable/b8_wordbeam_audit/audit.json` |
| E32 | Binary-key and global parity capacity checks | `experiments/quagmire_parity_capacity.md`; `results/quagmire_parity_capacity_audit.json`; `results/quagmire_parity_capacity_prefix.json`; `k4/fable/b9_ewi/parity_capacity_check.py` |
| E33 | Actual pruning traces and exact competitor classification | `experiments/wordbeam_pruning_trace.md`; `results/wordbeam_pruning_traces/dev0/audit.json`; `results/wordbeam_pruning_traces/dev4/audit.json`; `results/wordbeam_pruning_traces/dev0/refined_cap2944.json`; `results/wordbeam_pruning_traces/dev0/witness_crosscheck.json`; `k4/wordbeam/refine_check/check_refined.py`; `k4/fable/b12_dev0_r46/README.md` |
| E34 | Exact-pruning audits and wider control | `experiments/wordbeam_exact_prune.md`; `experiments/wordbeam_exact_component_audit.py`; `experiments/wordbeam_exact_integration_audit.py`; `results/wordbeam_exact_component_audit/audit.json`; `results/wordbeam_exact_integration_audit/audit.json`; `results/wordbeam_wide_pilot/dev0/audit.json`; `results/wordbeam_wide_pilot/dev0/comparison.json`; `results/wordbeam_exact_pilot/dev0/disabled/audit.json`; `k4/wordbeam_exact_prune/README.md` |
| E35 | Original press-event recording lead | `experiments/sanborn_press_recording_review.md`; `k4/fable/b13_spy_museum_event_sources.md` |
| E36 | Enabled-run pruning diagnosis and reverse-first contract | `experiments/wordbeam_exact_prune.md`; `results/wordbeam_exact_pilot/dev0/audit.json`; `results/wordbeam_exact_pilot/dev0/peer_crosscheck.json`; `results/wordbeam_exact_pruning_trace/dev0/audit.json`; `results/wordbeam_exact_pruning_trace/dev0/competitor_audit.json`; `results/wordbeam_exact_pruning_trace/dev0/score_anatomy_root.json`; `experiments/wordbeam_reverse_plan.md`; `k4/fable/b15_reverse_first_contract.md` |
| E37 | Reverse-first component and scheduling controls | `experiments/wordbeam_reverse_plan.md`; `results/wordbeam_reverse_components_audit.json`; `results/wordbeam_reverse_small_audit/audit.json`; `results/wordbeam_reverse_small_audit/score_audit.json`; `results/wordbeam_reverse_scalar_crosscheck.json`; `results/wordbeam_reverse_cli_audit/audit.json`; `k4/fable/b16_reverse_scalar/reference.py`; `k4/fable/b16_reverse_scalar/comparison.json` |
| E38 | Reverse pilot and retained-context pair diagnostic | `experiments/wordbeam_reverse_plan.md`; `results/wordbeam_reverse_pilot/dev0/audit.json`; `results/wordbeam_reverse_pilot/dev0/peer_crosscheck.json`; `experiments/wordbeam_gap_pair_results.md`; `results/wordbeam_gap_pair_diagnostic/audit.json`; `results/wordbeam_gap_pair_diagnostic/peer_crosscheck.json`; `results/wordbeam_gap_pair_diagnostic/projection_summary.json`; `results/wordbeam_gap_pair_diagnostic/exact_audit.json`; `experiments/wordbeam_lexical_bridge_plan.md` |
| E39 | Lexical bridge controls, affordability and conditional gap | `experiments/wordbeam_bridge_component_review.md`; `results/wordbeam_bridge_component_audit/audit.json`; `results/wordbeam_bridge_driver_audit/audit.json`; `results/wordbeam_bridge_component_audit_v2/audit.json`; `results/wordbeam_bridge_driver_audit_v2/audit.json`; `experiments/wordbeam_bridge_results.md`; `results/wordbeam_bridge_trial50/audit.json`; `results/wordbeam_bridge_true_context/observer.json`; `results/wordbeam_bridge_true_context/certify_audit.json` |
| E40 | Conditional full-message completion and all-context pilot contract | `experiments/wordbeam_middle_completion_plan.md`; `experiments/wordbeam_middle_completion_results.md`; `results/wordbeam_middle_completions/catalog_audit.json`; `results/wordbeam_middle_completions/audit.json`; `results/wordbeam_middle_completions/go_word_score_audit.json`; `results/wordbeam_middle_completions/observer.json`; `experiments/wordbeam_bridge_all_contexts_plan.md` |
| E41 | All-context development recovery and fixed-gap coverage limit | `experiments/wordbeam_bridge_all_contexts_results.md`; `results/wordbeam_bridge_all_contexts/terminal.json`; `results/wordbeam_bridge_all_contexts/sample_replay.json`; `results/wordbeam_bridge_all_contexts/final_audit.json`; `results/wordbeam_bridge_all_contexts/go_word_score_audit.json`; `results/wordbeam_bridge_gap_representability.json` |
| E42 | Crossing-word coverage and language-only bound checks | `experiments/wordbeam_crossing_bridge_plan.md`; `experiments/wordbeam_crossing_bridge_coverage.py`; `results/wordbeam_crossing_bridge_coverage.json`; `experiments/wordbeam_crossing_bound.py`; `experiments/wordbeam_crossing_bound_audit.py`; `results/wordbeam_crossing_bound_audit.json` |
| E43 | Crossing search controls and same-cap domain comparison | `experiments/wordbeam_crossing_search_results.md`; `results/wordbeam_crossing_search_audit/audit.json`; `results/wordbeam_crossing_real_bound/audit.json`; `results/wordbeam_crossing_domain_audit/audit.json`; `results/wordbeam_crossing_pilot334/terminal.json`; `results/wordbeam_crossing_domain_pilot334/audit.json`; `results/wordbeam_crossing_domain_pilot334/exact_audit.json` |
| E44 | Character-boundary controls and development parent retention | `experiments/wordbeam_boundary_results.md`; `results/wordbeam_boundary_baseline_recount.json`; `results/wordbeam_boundary_audit/audit.json`; `results/wordbeam_boundary_development/failure_audit.json`; `results/wordbeam_boundary_development_v2/terminal.json`; `results/wordbeam_boundary_development_v2/audit.json`; `results/wordbeam_boundary_development_v2/observer.json`; `experiments/wordbeam_joint_growth_design.md` |
| E45 | Joint inward growth, exact middles and finite full completion | `experiments/wordbeam_joint_results.md`; `results/wordbeam_joint_audit/audit.json`; `results/wordbeam_joint_layer_audit/audit.json`; `results/wordbeam_joint_layer_development/audit.json`; `results/wordbeam_joint_layer_development/completion_catalog_audit.json`; `results/wordbeam_joint_layer_development/full_completions/audit.json`; `results/wordbeam_joint_layer_development/observer.json` |
| E46 | Full-system projection audit, corrected cost test and unit-token coverage | `experiments/wordbeam_projection_results.md`; `results/wordbeam_projection_linear_audit/audit.json`; `results/wordbeam_projection_cost/failure.json`; `results/wordbeam_projection_cost_v2/audit.json`; `results/wordbeam_joint_unit_coverage/audit.json`; `results/wordbeam_joint_review_recount.json` |
| E47 | Optimal middle scores and native balanced path reachability | `experiments/wordbeam_middle_score_results.md`; `results/wordbeam_middle_score_bound/audit.json`; `results/wordbeam_middle_path_reach/manifest.json`; `results/wordbeam_middle_path_reach/result.json`; `results/wordbeam_middle_path_reach/terminal.json`; `results/wordbeam_joint_layer_development/audit.json` |
| E48 | Correct-path pruning trace and projection component closure | `experiments/wordbeam_joint_trace_results.md`; `results/wordbeam_joint_trace_controls/audit.json`; `results/wordbeam_joint_trace_controls/witness_audit.json`; `results/wordbeam_joint_trace_dev10/equivalence.json`; `results/wordbeam_joint_trace_dev10/witness_audit.json`; `results/wordbeam_joint_trace_dev10/summary.json`; `results/wordbeam_projection_closure.json` |
| E49 | Gap-lookahead design and junction diagnostics | `experiments/wordbeam_joint_lookahead_results.md`; `experiments/wordbeam_joint_junction_diagnostic.py`; `experiments/wordbeam_joint_gap_junction_diagnostic.py`; `results/wordbeam_joint_junction_diagnostic/audit.json`; `results/wordbeam_joint_gap_junction_diagnostic/audit.json`; `results/wordbeam_joint_lookahead_review/` |
| E50 | Full gap bounds and exact language relaxation | `experiments/wordbeam_gap_language_results.md`; `results/wordbeam_gap_bound_reference_v2/`; `results/wordbeam_gap_language_exact/`; `results/wordbeam_gap_language_witness/`; `results/wordbeam_gap_peer_audit/`; `results/wordbeam_joint_gap_junction_diagnostic_v2/` |
| E51 | Reusable language tables and first-token bounds | `experiments/wordbeam_gap_table_results.md`; `results/wordbeam_gap_unforced_tables/`; `results/wordbeam_gap_first_token_v2/`; `results/wordbeam_gap_first_fixed/`; `results/wordbeam_gap_table_peer_review/`; `results/wordbeam_gap_peer_provenance_restored/` |
| E52 | Native exact language kernel and fixed-stream cache feasibility | `experiments/wordbeam_gap_native_results.md`; `results/wordbeam_gap_go_audit/`; `results/wordbeam_gap_native_review/`; `results/wordbeam_cache_observer_controls/`; `results/wordbeam_cache_observer_dev10/` |
| E53 | Exact suffix-row caching and lookahead integration contract | `experiments/wordbeam_gap_cache_results.md`; `experiments/wordbeam_gap_integration_plan.md`; `results/wordbeam_gap_cache_audit/`; `results/wordbeam_gap_cache_rows_audit/`; `results/wordbeam_gap_cache_review/`; `results/wordbeam_gap_tiny_baseline/` |
| E54 | Lookahead trial monitoring and independent verification adapters | `experiments/wordbeam_lookahead_preflight.md`; `results/wordbeam_lookahead_monitor_controls/`; `results/wordbeam_lookahead_reference_cases/`; `results/wordbeam_lookahead_audit_control/`; `results/wordbeam_lookahead_witness_controls/` |
| E55 | Lookahead integration, capped development pilot and conditional prefilter design | `experiments/wordbeam_lookahead_integration_results.md`; `experiments/wordbeam_prefilter_design_review.md`; `experiments/wordbeam_prefilter_integration_plan.md`; `results/wordbeam_lookahead_integration_audit/`; `results/wordbeam_lookahead_dev10/`; `results/wordbeam_prefilter_rounding_envelope/` |
| E56 | Independent prefilter reference tables and witness-auditor controls | `experiments/wordbeam_prefilter_preflight.md`; `experiments/wordbeam_prefilter_reference.py`; `experiments/wordbeam_prefilter_witness_audit.py`; `experiments/wordbeam_prefilter_witness_controls.py`; `results/wordbeam_prefilter_reference/`; `results/wordbeam_prefilter_witness_controls/` |
| E57 | Prefilter implementation verification and bounded pilot launch | `experiments/wordbeam_prefilter_initial_results.md`; `experiments/wordbeam_prefilter_integration_results.md`; `results/wordbeam_prefilter_native_tables/`; `results/wordbeam_prefilter_integration_audit/`; `results/wordbeam_prefilter_dev10/input.json`; `results/wordbeam_prefilter_dev10/manifest.json`; `results/wordbeam_prefilter_dev10/process.json` |
| E58 | Terminal prefilter pilot, cap diagnosis and frontier-observer contract | `experiments/wordbeam_prefilter_pilot_results.md`; `experiments/wordbeam_frontier_observer_plan.md`; `results/wordbeam_prefilter_dev10/`; `results/wordbeam_prefilter_cost_controls/`; `results/wordbeam_partial_feasibility_diagnostic/` |
| E59 | Verified frontier observer and terminal replay confirming earlier path loss | `experiments/wordbeam_frontier_results.md`; `results/wordbeam_frontier_root_controls/`; `results/wordbeam_frontier_dev10/`; `results/wordbeam_frontier_adapter_review/` |
| E60 | Exact feasibility of the full terminal frontier and next diagnostic contract | `experiments/wordbeam_frontier_feasibility.py`; `experiments/wordbeam_frontier_feasibility_plan.md`; `results/wordbeam_frontier_feasibility/`; `experiments/wordbeam_layer_history_plan.md`; `experiments/wordbeam_global_priority_assessment.md` |
| E61 | Entered-layer-history verification and bounded diagnostic launch | `experiments/wordbeam_layer_history_results.md`; `results/wordbeam_layer_history_controls/`; `results/wordbeam_layer_history_root/`; `results/wordbeam_layer_history_adapter_review/`; `results/wordbeam_layer_history_dev10/input.json`; `results/wordbeam_layer_history_dev10/manifest.json`; `results/wordbeam_layer_history_dev10/process.json` |

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

Early film lead: the [DHM programme sheet](https://www.dhm.de/assets/Zeughauskino/Download/Filmbl%C3%A4tter_Berlin.Dokument/BD72_Stadtumbau.pdf) names World Clock footage in *Berlin – Hauptstadt der DDR I*. The film has not been viewed; no additional city lettering or cipher instruction is established.
