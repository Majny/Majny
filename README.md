### Hi, I'm Jakub

**Engineer & founder moving into AI-safety research.** I study how neural networks represent
what they know — superposition, feature geometry, and whether a goal a model is hiding stays
legible from the inside. MFF UK Prague · Co-founder & CTO at [Zoplio](https://zoplio.com).

**Research**

- **[absorption-atlas](https://github.com/Majny/absorption-atlas)**: how sparse-autoencoder
  features carry different kinds of token property (Gemma-2-2B/9B, Gemma Scope). Feature
  absorption tracks a *family* of properties rather than being a universal SAE failure mode:
  last-letter absorbs much like first-letter, but on a structural property no single latent
  causally carries the concept — which is also where the standard projection and causal metrics
  disagree. 15-page technical report + code.
- **[lost-in-the-monitor](https://github.com/Majny/lost-in-the-monitor)**: how reliably a model
  pursuing a hidden goal can be caught by reading its chain of thought. A control-style deception
  eval with programmatic ground truth. Monitors turn out to be bimodal at temperature 0, so
  detection has to be K-sampled to mean anything, and monitor strength interacts sharply with how
  subtle the sabotage is. Published null on the cross-lingual hypothesis, with the pre-registration
  and a dated lab log.
- **[superposition-phases](https://github.com/Majny/superposition-phases)** *(write-up in review)*:
  what kind of solution training finds when a layer computes more functions than it has neurons.
  The superposed code grows continuously out of the dedicated-neuron solution; the boundary between
  families is a level set of falling code coherence.

**Engineering**

- **[bitcoin-multisig-wallet](https://github.com/Majny/bitcoin-multisig-wallet)**: Android M-of-N
  multisig Bitcoin wallet with Trezor hardware signing, coin control and PSBT cosigner coordination.
  Seven Kotlin/Ktor microservices, hand-written BIP-174 serialisation, 116 backend test methods.
  Bachelor's thesis at MFF UK, defended with grade Excellent.
- **[Zoplio](https://zoplio.com)**: an AI assistant that books your meetings — it writes to the
  other side on WhatsApp or by email, reads the replies, checks your calendar and books the time.
  I own the agent runtime.

**Elsewhere**

[kubadvorak.com](https://kubadvorak.com) · [Writing (Substack)](https://kubadvorak.substack.com) ·
[X](https://x.com/jakubdvorak_ai) · [hi@kubadvorak.com](mailto:hi@kubadvorak.com)
