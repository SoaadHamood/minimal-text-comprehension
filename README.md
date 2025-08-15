# Minimal Text Comprehension: Neural Evidence for POS Hierarchies

**Which parts of speech are essential for neural language understanding?**

Brain encoding analysis revealing that content words maintain 85-90% of neural prediction accuracy while function words drop to only 17%.

## Files

- `structured_tasks.ipynb` - Tasks 1-3: Cross-embedding validation and brain encoding
- `unstructured_analysis.ipynb` - Core POS filtering analysis and semantic categorization
- `figures/` - All result figures referenced in the paper

## Key Findings

- Clear neural hierarchy: **content words > nouns+verbs > individual categories > function words**
- Content words alone sufficient for robust brain prediction (72.6% top-1 accuracy)
- 52-point mean rank difference between best (content words: 8.25) and worst (function words: 70.70) strategies

## Data Source

Analysis uses fMRI datasets from Pereira et al. (2018) - 627 sentences with corresponding brain activity.

## Citation

```bibtex
@article{hamood2025minimal,
  title={Minimal Text Comprehension: Which Parts of Speech Are Essential for Neural Language Understanding?},
  author={Hamood, Soaad and Saleh, Alaa},
  journal={Proceedings of the Annual Cognitive Science Conference},
  year={2025}
}
