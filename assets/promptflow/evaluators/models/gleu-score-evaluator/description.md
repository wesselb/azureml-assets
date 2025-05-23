| | |
| -- | -- |
| Score range | Float [0-1]: higher means better quality. |
| What is this metric? | The GLEU (Google-BLEU) score measures the similarity by shared n-grams between the generated text and ground truth, similar to the BLEU score, focusing on both precision and recall. But it addresses the drawbacks of the BLEU score using a per-sentence reward objective. |
| How does it work? | The GLEU score is computed by averaging the precision and recall of n-grams between the generated text and both the reference text and source text. It considers both the overlap of n-grams with the reference (similar to BLEU) and penalizes for over-generation. The score provides a balanced metric, where a value of 1 represents perfect overlap, and 0 represents no overlap. |
| When to use it? | The recommended scenario is Natural Language Processing (NLP) tasks. This balanced evaluation, designed for sentence-level assessment, makes it ideal for detailed analysis of translation quality. GLEU is well-suited for use cases such as machine translation, text summarization, and text generation. |
| What does it need as input? | Response, Ground Truth |
