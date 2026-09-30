# Vowel Space Area Analyzer

Browser-based research tool for acoustic vowel analysis using F1/F2 measurements.

## Primary VSA protocol
The primary quadrilateral VSA uses the same four corner vowels in every context:
- /iː/ — high front
- /æ/ — low front
- /ɑː/ — low back
- /uː/ — high back

Contexts:
1. Isolated words
2. Carrier phrase
3. Proposed sentences

## Features
- Participant ID and proficiency group
- F1/F2 entry for all four corner vowels
- Separate VSA for each context
- Identical quadrilateral/shoelace calculation across contexts
- Substituted equation display
- F1–F2 vowel-space plots
- Centroid calculation
- CSV export
- Example dataset

## Formula
A = 1/2 | Σ(F2_i × F1_i+1 − F1_i × F2_i+1) |

Area is reported in Hz².

## Research note
The vowel set and ordering should match the approved study protocol. This tool is intended for educational/research use and is not validated diagnostic software.
