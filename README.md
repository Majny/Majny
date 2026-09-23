### Hi, I'm Jakub

**AI and backend engineer in Prague, trained in systems programming.** I build systems and study what happens inside a neural network: the systems are my work, the neural networks a serious hobby. Co-founder & CTO at [Zoplio](https://zoplio.com) (supported by [BUDETO Studio](https://www.budeto.xyz/)) · BSc Computer Science, Systems Programming, MFF UK (2026) · Master's in AI from October 2026.

[kubadvorak.com](https://kubadvorak.com) · [CV](https://kubadvorak.com/cv.pdf) · [hi@kubadvorak.com](mailto:hi@kubadvorak.com)

#### Engineering

- **[bitcoin-multisig-wallet](https://github.com/Majny/bitcoin-multisig-wallet)**: my Bachelor's thesis ([100 pages on DSpace](https://dspace.cuni.cz/handle/20.500.11956/210821)), graded Excellent. An Android M-of-N multisig wallet in which every signature is made on a Trezor via Trezor Connect; the backend coordinates the cosigners but never holds key material and never signs.
  - Hand-written BIP-174 (PSBT) encoding and parsing, the multisig P2WSH script and the bech32 encoder.
    - 7 Kotlin/Ktor services on PostgreSQL under Docker Compose.
  - 116 backend test methods in GitHub Actions.
  - A 2-of-3 transaction verified on testnet.
- **Zoplio developer API** (source private, surface public): [API docs](https://zoplio.com/docs) · [`@zoplio/sdk-js`](https://www.npmjs.com/package/@zoplio/sdk-js) · [`zoplio` on PyPI](https://pypi.org/project/zoplio/) · [`@zoplio/claude-tool`](https://www.npmjs.com/package/@zoplio/claude-tool). Zoplio is an AI assistant that books meetings over WhatsApp, Slack and email; it is in early access, and keys go out in waves. I wrote all of its backend, including:
    - the public API: keys, rate limits, usage quotas and signed webhooks;
  - both SDKs (Node/TypeScript and Python);
  - the hosted MCP server, so AI agents can book meetings.
- **Kreedl Intelligence** (private; Software Engineer at Kreedl, Jan–Jun 2026): I designed and shipped an internal Gemini pipeline for pitch-deck analysis in investment screening. Python, FastAPI, MongoDB, Docker.
- **Systems programming at MFF UK** (my Bachelor's specialization; course code, not public):
    - a RISC-V (Sv32) teaching kernel in C, built in a team of three: heap, scheduling, synchronization, virtual memory, user-mode processes;
  - a C-subset compiler to LLVM IR (flex, bison, IRBuilder);
  - parallel programming with TBB, OpenMP, SYCL (CPU target), Spark and C# async, with jobs on the faculty's SLURM cluster;
  - Linux Administration: QEMU/KVM VMs as systemd services, DNS with DNSSEC, backups verified by a restore.
- **[AntColonySimulator](https://github.com/Majny/AntColonySimulator)**: a multi-colony foraging simulator in Unity/C# (solo course project, Advanced C# Programming).

#### Inside neural networks, on the side

- **[lost-in-the-monitor](https://github.com/Majny/lost-in-the-monitor)**: can a monitor catch a hidden goal by reading a model's chain of thought? An eval harness around gpt-oss-20b, run under vLLM in single-GPU PBS jobs (and with Ollama locally). Model-written code is graded in a time-limited subprocess against public and hidden tests. Monitor scores are sampled 8 times, because they are bimodal even at temperature 0. On backdoors framed as a performance fast-path, gpt-oss-20b as a monitor caught 6% where Gemini 2.5 Flash caught 80%. My starting hypothesis, that monitoring degrades when the chain of thought is in a lower-resource language, did not survive scaling. The null is published with the pre-registration and a dated lab log.
- **[absorption-atlas](https://github.com/Majny/absorption-atlas)**: how a concept is carried inside Gemma-2-2B/9B depends on what kind of concept it is. Built with TransformerLens, SAELens and Gemma Scope, in GPU jobs on MetaCentrum; 15-page technical report.
- **[superposition-phases](https://github.com/Majny/superposition-phases)**: when a layer computes more functions than it has neurons, the superposed code grows continuously out of the dedicated-neuron solution. The public code is the preliminary first pass; the 256-job CPU sweep and the 40-page write-up (in review) are not public yet.



#### How I work

Day to day I build with Claude Code: I write a short spec first, keep each change small and read every diff before it goes in. The thesis wallet and my kernel code I wrote almost entirely by hand.

[kubadvorak.com](https://kubadvorak.com) · [LinkedIn](https://www.linkedin.com/in/jakubdvorak-ai/) · [Writing](https://kubadvorak.substack.com) · [hi@kubadvorak.com](mailto:hi@kubadvorak.com)
