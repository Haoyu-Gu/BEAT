# BEAT: Rethinking Symbolic Music Encoding with Beat-Anchored Tones Representations

This repository contains the demo page for the paper **"BEAT: Rethinking Symbolic Music Encoding with Beat-Anchored Tones Representations"**.

## Abstract

The perception of symbolic music is fundamentally based on the relative durations and interval relationships between the notes. However, existing representations face an inherent trade-off between preserving these musical priors and achieving encoding efficiency. In this paper, we propose **BEAT** (Beat-based Encoding with Anchored Tones), which breaks from the conventional note-event paradigm by adopting beat units as the basic primitive. BEAT segments the temporal axis into beat units, organizing music as sequences of these units. Within each beat, notes are sorted by pitch, with the first serving as an anchor point, while subsequent notes are encoded through chained relative intervals coupled with rhythmic patterns. This approach achieves efficient serialization while explicitly preserving musical priors.

Additionally, BEAT employs beat indexing for temporal alignment, enhancing both concurrent modeling capabilities and editability, enabling seamless adaptation to diverse downstream tasks. Extensive experiments demonstrate that BEAT achieves better encoding efficiency than existing methods while achieving state-of-the-art generation quality in both objective and subjective benchmarks. BEAT also consistently outperforms baselines across diverse tasks including multi-track generation, segment infilling, and real-time accompaniment.

## Demo Page

The demo page showcases:

- **Encoding Efficiency**: BPE compression rate and sequence length comparisons
- **Unconditional Generation Results**: Evaluation metrics across different model architectures
- **Audio Samples**:
  - Piano Continuation (Method Comparison with REMI, ABC)
  - Expressive Piano Continuation
  - Real-time Accompaniment
  - Multi-track Ensemble (String Quartet, Piano Quartet, Piano & Choir, Clarinet & Piano)

## Local Development

To view the demo page locally, simply open `index.html` in a web browser, or use a local server:

```bash
# Python 3
python -m http.server 8000

# Then open http://localhost:8000 in your browser
```

## License

This website template is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/).
