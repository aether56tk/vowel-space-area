# Vowel Space Area Analyzer

Browser-based F1/F2 acoustic vowel-space analysis tool for research and educational workflows.

## What you enter

The intended workflow is simple:

**Paste a participant row from Excel/Google Sheets → Import → inspect the automatic quadrilateral vowel graph and VSA.**

The analyzer accepts the research-table structure:

1. Sl. no
2. Name
3. Gender
4. LEAP score
5. Proficiency
6. Ten vowel groups, each containing **F1, F2, VD**

The application uses **F1 and F2 only**. VD and the preceding metadata are ignored for VSA calculation.

## Vowel order

The 10-vowel order is:

1. /iː/
2. /ɪ/
3. /ɛ/
4. /æ/
5. /ʌ/
6. /ɑː/
7. /ɔː/
8. /ʊ/
9. /uː/
10. /ɝ/

## Quadrilateral VSA

VSA automatically uses the four predefined corner vowels in this order:

**/iː/ → /æ/ → /ɑː/ → /uː/**

Formula:

`VSA = 1/2 | Σ(F2ᵢ × F1ᵢ₊₁ − F1ᵢ × F2ᵢ₊₁) |`

Area is reported in **Hz²**.

The graph uses F2 on the horizontal axis and F1 on the vertical axis. The four corner vowels form the quadrilateral; the remaining six vowels are plotted as additional acoustic points.

## Automatic outputs

- Quadrilateral VSA
- Substituted shoelace equation
- F1–F2 quadrilateral graph
- All supplied vowel points
- Centroid
- Perimeter
- FCR
- Context-wise comparison
- CSV export

## Contexts

The interface supports:

- Isolated words
- Carrier phrase
- Proposed sentences

The same four-vowel VSA protocol is used in every context.

## Data handling / security

This is a static browser application. Calculations and pasted-data processing happen in the user's browser; the project does not provide a database or application-server upload endpoint.

For research ethics and privacy, use participant IDs or de-identified data where appropriate and follow the approved study protocol. Do not paste unnecessary personally identifying information.

## Important research note

This tool is an analysis aid, not validated diagnostic software. Confirm the vowel order, acoustic measurement procedure, and VSA protocol against the approved research protocol before using results in a thesis, paper, or clinical report.
