Dataset Header Explanations 

1. SentenceId: 
A unique identifier assigned to each row/sentence in the dataset (e.g., "TE_MAIN_0001"). Useful for tracking and referencing specific examples.

2. Language: 
The standard two-letter ISO code representing the language of the sentence (see Part 2 for the full list of codes).

3. Sentence: 
The text containing the coreference challenge. It features two entities (professions) and a pronoun that needs to be resolved to the correct entity.

4. Label: 
The ground truth indicator showing which entity the pronoun refers to. In this sample, a "0" consistently indicates that the pronoun resolves to the "target" entity rather than the "distractor".

5. target: 
The correct entity (profession) that the pronoun in the sentence refers to based on the context (e.g., "మెకానిక్" / Mechanic).

6. distractor: 
The secondary entity (profession) mentioned in the sentence that serves as a distractor for the NLP model (e.g., "నర్స్" / Nurse).

7. bias: 
Indicates the stereotypical alignment of the sentence. 
- "pro-stereotype": The gender of the pronoun matches the traditional gender stereotype of the target profession (e.g., Male Mechanic).
- "anti-stereotype": The gender of the pronoun contradicts the traditional gender stereotype of the target profession (e.g., Female Mechanic).

8. target_stereotype: 
The traditional or statistically prevalent gender stereotype associated with the target profession (e.g., Mechanic = Male).

9. distractor_stereotype: 
The traditional or statistically prevalent gender stereotype associated with the distractor profession (e.g., Nurse = Female).

10. gender in sentence: 
The actual gender of the pronoun used in the specific sentence (e.g., "male" or "female").

11. pronoun_being_resolved: 
The exact pronoun found in the sentence that the model must correctly link to the target entity (e.g., "అతను" / he, "ఆమె" / she).

The "Language" column uses the following standard ISO 639-1 codes:

* te - Telugu
* ta - Tamil
* kn - Kannada
* ml - Malayalam
* mr - Marathi
* hi - Hindi
* bn - Bengali
* od - Odia