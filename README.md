# sample-prompts

## Anki Flashcards creator
Please create a set of cloze-only flashcards based on the lecture notes I will supply. Follow these guidelines:

Each flashcard must be minimal-information, containing no more than 10 words.
Structure the clozes so that key terms and context are enclosed in cloze deletion markers (e.g., {{c1::...}}). Use multiple cloze markers per card when necessary to force recall of all essential elements.
Ensure that every flashcard covers a single, focused concept from the notes. Do not include any text or references (e.g., 'Figure 3.8') that depend on external materials.
The flashcards should collectively capture all important details, including definitions, examples, and relationships, exactly as presented in the notes.
Do not add extra information or line breaks beyond what is needed for Anki import.
Once you receive the lecture notes, transform them into cloze flashcards following these instructions.
{{Lecture Notes}}

## Lecture Notes Improver
**Transform these "Bad Lecture Notes" into "Good Lecture Notes":**

Your goal is to rewrite the following "bad notes" into clear, concise, and well-structured "good notes," similar to the style and improvements demonstrated in the "Good notes" example provided for "Clustering Techniques."

**Focus on making the notes:**

* **Clear and Understandable:** Ensure concepts are explained simply and directly, avoiding jargon where possible or explaining it when necessary.
* **Complete and Informative:** Fill in any missing definitions, expand on key concepts that are only briefly mentioned, and add relevant details to ensure understanding.
* **Well-Structured and Organized:** Use headings, subheadings, bullet points, and numbered lists to create a logical flow and make the information easy to navigate and digest.
* **Formatted for Readability:** Utilize formatting like bold text, headings, and spacing to make the notes visually appealing and easy to scan and review.  Emphasize key terms.
* **Comprehensive (where appropriate):**  Consider adding elements that were present in the "Good Notes" example but missing in the "Bad Notes," such as:
    *  Alternative names for techniques (e.g., "Agglomerative Clustering")
    *  Key related concepts (e.g., "Proximity Matrix," "Dendrogram")
    *  Formulas (if mathematical concepts are involved and formulas are missing but relevant)
    *  "Pros and Cons" lists that are currently incomplete.
    *  "Important Considerations" or summarizing takeaways.

**Here are the "Bad Lecture Notes" to be transformed:**

{{bad notes}}


**Desired Output:**  "Good Lecture Notes" in a similar format and style to the provided example, significantly improved in clarity, completeness, structure, and readability.

**Example of Desired "Good Notes" Style (referencing the Clustering Techniques example):**

###
### Clustering Techniques (Example Style - You don't need to re-process this)

**1. Hierarchical Clustering**

- Also known as **Agglomerative Clustering**
- Uses a **Proximity Matrix** to measure distances between clusters
- Results visualized in a **Dendrogram**

- **Pros:**
    - No need to specify the number of clusters in advance
    - Provides a hierarchical representation of data

- **Process:**
    1. Start with each data point as a separate cluster
    2. Merge closest clusters iteratively
    3. Continue until all points are in one cluster or a stopping criterion is met

**2. Density-Based Clustering**

- **DBSCAN** (Density-Based Spatial Clustering of Applications with Noise)
    - Key concepts:
        - **Epsilon (ε)**: Maximum distance between two points for them to be considered as neighbors
        - **MinPts**: Minimum number of points required to form a dense region

    - Point classifications:
        1. **Core Point**: Has at least MinPts points within distance ε
        2. **Border Point**: Within ε distance of a core point but has fewer than MinPts neighbors
        3. **Noise Point**: Neither a core point nor a border point

    - **Pros:**
        - Can find arbitrarily shaped clusters
        - Robust to outliers
        - Does not require specifying the number of clusters a priori

    - **Cons:**
        - Sensitive to choice of ε and MinPts
        - May struggle with clusters of varying densities

### Key Formulas:

- Distance measure (e.g., Euclidean distance):
  $d(p,q) = \sqrt{\sum_{i=1}^n (p_i - q_i)^2}$

- DBSCAN density criterion:
  $|\{p \in D | \text{dist}(p,q) \leq \varepsilon\}| \geq \text{MinPts}$

### Important Considerations:

- Choice of distance metric in hierarchical clustering
- Interpretation of the dendrogram
- Selection of ε and MinPts in DBSCAN
- Handling of high-dimensional data in both techniques
###

## Practice Questions Generator
**Generate practice questions for me on the topic of: {{Clearly Define the Topic(s) Here - Be Specific!}}

**I need approximately [Number] practice questions at each of the following difficulty levels:**
* **Beginner:** (Define what "beginner" means in this context. E.g., "For someone with no prior knowledge," or "Focusing on basic definitions and concepts"). [Your Beginner Level Definition Here]
* **Intermediate:** (Define "intermediate" for this topic. E.g., "For someone who understands the basics and is learning to apply them," or "Focusing on problem-solving with straightforward scenarios"). [Your Intermediate Level Definition Here]
* **Advanced:** (Define "advanced" for this topic. E.g., "For someone aiming for mastery and tackling complex problems," or "Focusing on nuanced applications, critical analysis, and challenging scenarios"). [Your Advanced Level Definition Here]

**Question Types:** (Select one or more from the following or specify your preference)
* [ ] Multiple Choice
* [ ] Short Answer
* [ ] Problem-Solving (e.g., calculations, coding problems)
* [ ] True/False
* [ ] Fill-in-the-Blanks
* [ ] Essay/Discussion Questions
* [ ] Other: [Specify if other type desired]

**Optional Features:**
* [ ] Please provide an **answer key**.
* [ ] Please provide **brief explanations** for the answers (especially for problem-solving or concepts that might be tricky).
* **Learning Goal (Optional):**  [Briefly describe your learning goal or why you need these practice questions, if desired. E.g., "Preparing for an exam on this topic," "Reinforcing my understanding after reading a chapter," "Self-testing my knowledge."]

**Desired Output Format (Optional):** [Specify if you have a preferred output format. If not specified, plain text is fine. E.g., "Markdown format," "Organized in a table," "Numbered list."]
