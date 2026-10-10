# What we've tried

**Snapshot: 11 October 2026. No authenticated solution.**

This table groups related experiments rather than listing every script or run.
A negative result always belongs to a specific model. It does not eliminate a
whole theme such as clocks, rotation or masking.

| Result label | Meaning |
| :--- | :--- |
| **Excluded in scope** | An exact contradiction or completed exhaustive test rejects the stated construction. |
| **Catalog negative** | Every member of a declared finite catalog fails; other keys or constructions remain possible. |
| **No convincing text** | Fits exist, but their language or other evidence does not support a solution. This is not an impossibility proof. |
| **Open / limited** | A relaxation fits, a search lacks demonstrated recovery power, or an important case is untested. |

Evidence IDs below refer to [the evidence index](EVIDENCE.md#working-archive-index).
**ABC** is the ordinary alphabet; **KA** is `KRYPTOSABCDEFGHIJLMNQUVWXZ`.
A *crib* is a known piece of plaintext.
Unless explicitly stated otherwise, tests use the exact canonical ciphertext
and the 24 confirmed plaintext letters. The separate error-allowance checks
below do not alter that input.

## Reading order, grids and substitution

| Approach | What we tested | Result | What remains outside the result | Evidence |
| :--- | :--- | :--- | :--- | :--- |
| Pure rearrangement | A permutation of the 97 letters without changing them | **Excluded in scope:** the known plaintext alone needs three Es; the ciphertext contains two | Rearrangement combined with substitution | E01 |
| Keys read from panel edges | First/last letters of published rows, in both directions; ABC/KA alphabet choices and three repeating-key rules | **Catalog negative:** 5,568 settings, zero complete crib matches; independent forward and inverse implementations agree | Other extractions, arbitrary alphabets, layers and physical layouts absent from the published representation | E29 |
| Fixed substitution per row | A separate fixed letter permutation for each of K4's four physical rows | **Excluded in scope:** confirmed N/O in the same row both encrypt to Q; independent checkers agree | Substitutions that change within a row or an added transposition | E29 |
| Repeating shifts and keyword alphabets | Direct periodic models; finite word catalogs with one alphabet fixed and the other free; several ways of ranking key letters | **Catalog negative** in the documented models; a separate free-alphabet branch's 477,612 completions yield implausible best texts | Other alphabet/key relationships and extra layers | E02 |
| Generalised Quagmire | Two arbitrary alphabets and short periodic keys | **Open / limited:** crib fits remain; ordinary beams and a score using distant implied letters all recover 0/8 generated period-8 examples with public24 | Independently checked implementations still have weak recovery; no cipher-family exclusion follows | E03 |
| Periodic repetition structure | Forced-letter counts and same-residue matches to the public clues | **Descriptive comparison:** direct period-8 K4 implies six additional letters; only 1/1,000 matched literary-prose controls has as few, with all witnesses independently audited | This exposes a benchmark mismatch; the empirical fraction is not a p-value or an exclusion | E28 |
| Structured transposition routes | Millions of row/column, rotation, padded-grid and layered routes with periodic, Porta, interrupted-key and running-key tests | **No strong candidate:** specified screens are negative; some long-period fits remain underconstrained | Arbitrary permutations and untested compositions | E04 |
| Dial and counting routes | Decimation, Josephus-style counting in both directions, and a 24-column dial family | **No strong candidate** in the declared catalogs | Other counting instructions or justified starting rules | E04 |
| Compass routes | 864 integer-slope routes plus 224 exact off-axis compass projections, including the carved K4 layout | **No convincing text:** the strongest new substitution fit forces no additional plaintext beyond the cribs | Other source-motivated reading rules; approximate photo angles are not instructions | E05 |
| K3 as an operation key | Numerical streams extracted from the verified K3 rearrangement, with declared phases and mappings | **Catalog negative** | Other dependencies between the passages | E04 |
| Nicodemus | Five-row column reading plus substitution, any column order and independent column shifts | **Excluded in scope** for widths 1–19 with ABC/KA alphabets and either plaintext sign; 415,872 keywords × 64 settings also fail | Arbitrary other alphabets, other chunk heights, and unrestricted widths ≥20 | E06 |
| Amsco alternating cells + column shifts | Single/double-letter cells, arbitrary column order and a separate additive shift per original column | **Excluded in scope** through width17 in two implementations. Fixed 415,872-word conventions give zero matches in two complete enumerations | Wider arbitrary-column cases include fits and timeouts; letter-index keys and other rules are different models | E23 |
| Turning grille, short keys | A 10×10 rotating mask in either direction; row-major filling/reading; final three holes blank; periodic substitution in either layer order | **Excluded in scope** for periods 1–4, ABC/KA alphabets; independent quarter-interleaving methods agree | Other dimensions, blank conventions, alphabet orders and longer keys | E07 |
| Turning grille, word catalog | 415,872 keywords, all cyclic key phases and both key signs; 244,699,136 alphabet/sign/layer settings | **Catalog negative:** 2,190 weak passes reduce to nine interleavings, all rejected by exact geometry in both rotation directions | Other blank conventions, reading rules, alphabets and keys outside the catalog | E07 |

## Clock-driven and changing alphabets

| Approach | What we tested | Result | What remains outside the result | Evidence |
| :--- | :--- | :--- | :--- | :--- |
| Constant-speed rotor | Fixed wiring, declared input/output rotations, exact real-rate schedules and finite extensions | **Excluded in scope** | Irregular stepping, other state rules or added layers | E08 |
| Four 24-letter rings | Enumerated ring/spoke arrangements, rotations and a spare letter | **Excluded in scope** for the documented construction | Other physical arrangements | E08 |
| Coupled 24/26 wheels | Exact constant real speeds/phases; fixed, clue and dictionary alphabet variants | **Excluded in scope** for specified fixed/catalog alphabets; one complementary dictionary fit, CLOTHLIKE, forces implausible text patterns | Other free alphabets and mechanisms | E09 |
| Both alphabet orders free | Single-clock offset models with 24 or 26 sectors | **Mixed:** the direct 26-sector model is excluded; the 24-sector model admits fitted witnesses | The 24-sector fits are not recovered plaintext | E09 |
| Feedback and row resets | Letter-dependent stepping, before/after stepping, and resets at physical row boundaries | **Mixed:** several finite families are excluded; other fits show no useful advantage over random controls | More general stateful machines | E10 |
| Clock sectors select shifts | Arbitrary sector-to-shift tables at constant real rates; ABC/KA and finite clue/city/keyword alphabets | **No convincing text** after exact optimisation of the tested models | Different alphabets, stepping or interpretation | E11 |
| Omitted plaintext spaces | A clock advances through unknown spaces under six declared crib segmentations | **Catalog negative** with either tested alphabet fixed; arbitrary-alphabet fits remain | Other spacing conventions and alphabet relationships | E12 |
| Trigger-letter disks | Extra steps or resets after selected ciphertext letters | **Catalog negative** with tested keyword alphabets; arbitrary-alphabet witnesses exist | Those witnesses do not identify a meaningful key | E13 |
| Plaintext-trigger resets | Resetting before/after selected plaintext letters, constant steps and arbitrary alphabet orders | **Excluded in scope**, with independent complete enumerations | Other reset rules or state | E13 |
| Ciphertext as its own key material | Cyclic overlay interpreted as a lookup key | **Excluded in scope** for ABC/KA; 1,304 shared-keyword models yield implausible best texts | Other self-referential rules | E11 |
| Chaocipher | Classic cut/rotate alphabets, one keyword wheel and one arbitrary wheel; separate free-wheel pilot | **Catalog negative** for fixed-word constructions; unrestricted wheel recovery remains **open / limited** | The language pilot recovered only 5 of 8 held-out examples exactly | E14 |
| Move-to-front / move-to-back | Four direct index-output variants with a fixed free counterpart alphabet | **Excluded in scope** by repeated-index contradictions | Additional operations or layers | E14 |

## Other hand ciphers and running keys

| Approach | What we tested | Result | What remains outside the result | Evidence |
| :--- | :--- | :--- | :--- | :--- |
| Ragbaby word counters | Shared 26-letter alphabet, arbitrary word breaks and initial counter/phase | **Excluded in scope:** independent methods cannot fit both known passages | Separate input/output alphabets, reflected-plaintext forms and other counter rules | E15 |
| Common restart at each word | The same sequence of bijective substitutions restarts at declared EAST… and BERLIN… boundaries | **Excluded in scope:** their fourth plaintext letters differ but both encode to V | Word-dependent starts or different boundaries | E15 |
| Slidefair | Direct paper-strip rules, arbitrary alphabets/key sequences and both adjacent-pair alignments | **Excluded in scope** | Additional transposition or other constructions | E16 |
| Condi / short-memory feedback | Standard Condi and broader declared direct feedback functions | **Excluded in scope** by repeated-input contradictions | Extra internal state or longer memory | E16 |
| Wheatstone-style geared pointers | Declared 27/26 pointer model with arbitrary alphabets; related short-history additive motion | **Excluded in scope** | Other gearing, state or layers | E16 |
| Direct Portax | Paired sliding-strip substitution with shared alphabet relabeling | **Excluded in scope** when the known S at position 33 is paired; the rule never fixes a component | Unpaired pass-through exceptions, output swaps and other alphabets/layers | E16 |
| Direct reflector Enigma | Standard fixed-point-free letter mapping in the original positions | **Excluded in scope:** known plaintext and ciphertext share S and K at two positions | Extra layers or a different machine | E01 |
| Gromark / generated keys | Decimal/mod-26 additive recurrences, finite primer/tap bounds, plus free-alphabet and dictionary variants | **Mixed:** fixed ABC/KA-side cases fail within bounds; free/free fits are compatible with chance rates | Longer/different recurrences and reliably decoded free-alphabet fits | E17 |
| Bifid and Trifid | Exact fractionation constraints, alignments and alphabetic completions | **Open / limited:** many configurations are impossible, but 371 Trifid and 262 Bifid configurations remain feasible without authenticated text | Feasibility is not an English solution | E18 |
| Dictionary Trifid cubes | 339,164 bases × 8,424 layouts × six feasible standard periods | **Catalog negative:** 17.14 billion generated hypotheses, with duplicates included | Other cubes, alignments or layers | E18 |
| Fractionated Morse | Fixed injective trigram maps; specified homophonic and short-trit variants | **Excluded in scope** by coordinate, injectivity or length constraints | Changing maps, transposition and different length assumptions | E18 |
| Carter lecture running key | 38 declared readings derived from 14 ca.1924 lecture records, tested across placements and all 26 constant phases | **Catalog negative:** two complete methods agree | Untranscribed sources, different readings or running-key constructions | E19 |
| Historical keyword alphabet rules | Literal column-read and numbered-column constructions | **Catalog negative** in the four declared clock/trigger/Chaocipher screens | Using those alphabets in other models | E20 |

## Allowing a hypothetical copying or carving error

| Approach | What we tested | Result | What remains outside the result | Evidence |
| :--- | :--- | :--- | :--- | :--- |
| Pure rearrangement catalog with substitutions allowed | 43,707,615 stored/generated route entries, both directions; full independent recount | **Catalog negative:** every entry needs at least 15 substitutions to satisfy the known letters | Routes outside the catalog, insertions/deletions, genuine substitution layers | E25 |
| Ordinary single columnar with one wrong letter | Widths 2–24, arbitrary column order | **Excluded in scope** by independent tests; a reviewed exact solver also rejects two wrong letters | Wider columns and other reading conventions | E25 |
| Structural hand-cipher contradictions | Reflector, Slidefair and six word-reset segmentations | **Mixed:** some survive one edit; other necessary conditions admit repairs | Passing a necessary condition does not recover a cipher key | E25 |
| Constant-speed word reset after one edit | Both alphabets arbitrary; 50 structurally possible repairs, six declared word splits | **Open / limited:** 49 repairs admit fitted constructions; all 49 complete witnesses independently verified | No natural plaintext, justified correction or independently motivated alphabet has emerged | E25 |

## Source work and the human clues

| Investigation | What we established | What we did not establish | Evidence |
| :--- | :--- | :--- | :--- |
| The Berlin clock | The clue identifies the Alexanderplatz World Clock; its mechanism motivates concrete rotation hypotheses | A unique letter mapping, key or rotation schedule for K4 | E21 |
| Historical city labels | Dated photographs show changes in placement and ordering; the museum model is not an exact substitute for the actual clock | A complete verified 1989 roster | E21 |
| 1990 panel transcription | A clearer pre-installation photograph supports several readable panels; an initial band alignment error was corrected | That Sanborn used those labels; no scan used the erroneous alignment | E21 |
| City-panel alphabets | 13 explicit panel strings produced 39 alphabets, tested in declared clock/trigger/Chaocipher models | No convincing text; this does not reject every use of city names | E20–E21 |
| Archive photographs | Six public images show compass sketches, cipher vocabulary and layered materials | No new hard plaintext clue, calibrated angle or executable K4 rule | E22 |
| Egypt, Berlin and message delivery | These support historical, autobiographical and physical interpretations worth investigating | An itinerary, sentence or numerical key that can be imposed as fact | E22 |
| Copper-panel anomalies | Raised Y/A/R occur in K3's ciphertext; CIA graphics preserve ragged rows and an extra tableau L | The extra L has not been confirmed in a clear photograph; no decoding operation follows | E26 |
| Carter's reply as a proposed opening | All six variants fit a free-alphabet periodic model, but each has at least two English controls fitting at its minimum period; all 18 witnesses independently verified | The declared rarity criterion fails; this does not disprove the story or establish full control frequencies | E27 |
| East-northeast as a clock face | Provisional models of dated photographs leave the ray near a boundary between two city panels | No unique face, surveyed bearing or city-derived key is established | E21 |
| A shorter message with filler letters | Reviewed public accounts describe meaningful English and correctly placed clues; no positive evidence for null padding was found | This is a reason to lower its priority, not a proof excluding all filler schemes | E22 |

The large numbers describe work performed, not the probability that we are
close to solving K4. The useful progress is the smaller set of precise
possibilities each validated result removes.
