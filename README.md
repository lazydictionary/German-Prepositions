# German-Prepositions

# German Prepositions Anki Deck

This repository contains the source file for an Anki flashcard deck designed to practice German prepositions and their required cases.

## Overview

The deck is designed to build intuition for which case (Accusative, Dative, or Genitive) follows specific prepositions. To ensure effective learning and prevent "meta-gaming"—where a user guesses the answer based on visual cues rather than grammatical knowledge—the cards utilize specific formatting strategies.

## Features

### Anti-Meta-Gaming Strategy
Standard Anki cards often split the article and noun into separate clozes (e.g., `[...] [Noun]`). This allows users to subconsciously identify Genitive cases simply by counting the number of boxes. This deck solves that issue by:

1.  **Merged Clozes:** The article and the noun are wrapped in a single cloze deletion.
    * *Standard:* `abseits [...] [...]` (Visual cue implies Genitive)
    * *This Deck:* `abseits [...]` (Indistinguishable from Dative/Accusative)
2.  **Lemmatized Hints:** Dative plural nouns often add an `-n` ending (e.g., *Kindern*). To prevent this from giving away the answer, the hint text inside the cloze displays the base plural form.
    * *Example:* `{{c1::den Kindern::Kinder}}`

### Grammatical Coverage
- **Cases:** Covers Prepositions requiring Dative, Accusative, and Genitive cases.
- **Genders:** Rotates through Masculine, Feminine, Neuter, and Plural nouns to ensure coverage of all declension patterns.
- **Word Order:** Correctly handles post-positioned prepositions (e.g., *entlang*, *zufolge*, *zuliebe*) to reflect standard German usage.

## File Format

The file `German Prepositions.txt` is a Tab-Separated Value (TSV) file containing the following columns:

| Column | Content | Description |
| :--- | :--- | :--- |
| 1 | ID | Unique identifier for the card/note. |
| 2 | Preposition | The preposition being tested. |
| 3 | Case | The grammatical case required (Dativ, Akkusativ, Genitive). |
| 4 | Gender | The grammatical gender of the noun used (Masculine, Feminine, Neutrum, Plural). |
| 5 | Sentence | The full sentence with Anki-formatted cloze deletions. |

## Usage

1.  Download `German Prepositions.txt`.
2.  Open Anki and create a new deck (optional).
3.  Go to **File > Import**.
4.  Select the text file.
5.  In the import settings:
    * Set **Note Type** to "Cloze".
    * Set **Field Separator** to "Tab".
    * Ensure the columns map correctly to your note type fields (e.g., ID, Preposition, Case, Gender, Text).

## Contributing

Corrections to grammar or sentence naturalness are welcome. Please ensure any changes to the text file maintain the tab-separated structure and the merged cloze format described above.
