# Create Backlog Prompt

## Setting the Stage

<!-- You are a **Product Owner** assigned to the team who has generated some artifacts including a product vision and product goal, as gathered other artifacts.  You are in **Backlog Creation** mode to generate product backlog for your Scrum team to execute, in accordance with the standards included as a part of The Intertech Way. -->

## Optional Additional Context
<!-- Here is an example of additional context that could be included -->

<!-- **Example:* "We are currently in the discovery phase for enhancing the event filtering capabilities." OR "Following a major competitor release, we need to reassess our feature parity based on recent market analysis and internal documentation." -->

### Instructions:

## 3. Input Data Specification

* **List the Artifacts:** Clearly enumerate *all* documents or data sources the LLM must process. Use identifiers for clarity.
    * *Example:* "You will analyze the following artifacts:
        * [DOC 1] /ProductInfo/ProductGoal.md for information about the current goal for the product.
        * [DOC 2] /ProductInfo/ProductVision.md for the larger product vision.
        * [DOC 3] /BacklogGuidelines/ProductBacklogGuidelines.md for the standards for backlogs for The Intertech Way, including the desired hierarchy of backlog items.
        * [DOC 4] /Definitions/ScrumTerms.md for definitions of terminology not in the Scrum Guide.
        
 **Specify Focus Areas (If Applicable):** Direct the LLM's attention if certain documents are more relevant for specific tasks.
    * *Example:* "For identifying user-requested filter types, prioritize [DOC A] and [DOC E]. For understanding current implementation details, refer solely to [DOC B]."

## 4. Detailed Task Instructions (The Core)

<!-- * **Break Down the Request:** Use a numbered or bulleted list for specific, granular tasks. Be explicit.

    * **Extraction Tasks:** Define *exactly* what to pull out.
        * *Example:* "1. Extract all explicit user requests for new filter categories or sorting options mentioned in [DOC A] and [DOC E]." "2. List all currently implemented filter mechanisms described in [DOC B]." "3. Identify specific filter features highlighted in the 'EventFinder Pro' analysis in [DOC C]."

    * **Summarization Tasks:** Specify desired length and focus.
        * *Example:* "4. Provide a brief (2-4 bullet points) summary of the main usability issues related to filtering mentioned in [DOC A] or [DOC E]." "5. Summarize the key takeaways from the brainstorming session regarding filters [DOC D]."

    * **Synthesis Tasks:** Ask the LLM to connect information across sources.
        * *Example:* "6. Synthesize a list of potential new filter requirements by combining user requests ([DOC A], [DOC E]) and ideas from the brainstorming session ([DOC D])." "7. Compare the filtering features of 'EventFinder Pro' ([DOC C]) with our current implementation ([DOC B]). Identify key gaps."

    * **Identification Tasks:** Ask the LLM to locate specific information types.
        * *Example:* "8. Identify any inconsistencies between user requests ([DOC A], [DOC E]) and the current specifications ([DOC B])." "9. List any technical limitations or challenges regarding filtering mentioned in any document."

    * **Analysis/Comparison Tasks:** Require analysis based *only* on provided text.
        * *Example:* "10. Based *only* on the feedback in [DOC A] and [DOC E], identify the top 3 most frequently mentioned frustrations with the current filtering system." -->

## 5. Output Format and Structure Requirements

* **Specify the Format:** Define the desired output format (e.g., Markdown, JSON).
    * *Example:* "Present your findings in well-structured Markdown format."
* **Structure:** Detail the organization of the output.
    * *Example:* "Organize your response with clear headings corresponding to each task number (e.g., 'Task 1: User Requested Filters'). Use nested bullet points for detailed lists. Highlight critical findings or inconsistencies in **bold**."
* **Citations:** Mandate source attribution for traceability.
    * *Example:* "Crucially, for every piece of extracted information, synthesis point, or identified issue, **you MUST cite the source document identifier and, if possible, a relevant section or page number** (e.g., 'Users requested a 'date range' filter - [DOC A], Survey Q5 Response Summary)."

## 6. Constraints and Guardrails

* **Scope Limitation:** Emphasize using *only* the provided materials.
    * *Example:* "Your analysis must be based *strictly* on the content within the provided artifacts [DOC A-E]. Do not incorporate external knowledge, make assumptions, or infer information not explicitly stated."
* **Handling Ambiguity/Contradictions:** Provide instructions for unclear or conflicting data.
    * *Example:* "If information is ambiguous, note the ambiguity clearly. If information conflicts between documents, report both conflicting points and cite their respective sources accurately."
* **Tone and Style:** Specify the desired writing style.
    * *Example:* "Maintain a professional, objective, and analytical tone. Be factual and avoid speculative language."
* **Prioritization (if applicable):** Indicate if some tasks hold more weight.
    * *Example:* "Accuracy in Task 8 (Identifying Inconsistencies) is paramount."

## 7. Clarification Clause

* **Encourage Questions:** Permit the LLM to seek clarification.
    * *Example:* "If any part of these instructions is unclear, or if you encounter ambiguity within the documents that prevents task completion, please ask for clarification before generating the full response."
