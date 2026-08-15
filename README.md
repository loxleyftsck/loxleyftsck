<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=0,2,30&height=200&section=header&text=Herald%20Ginting,%20S.Kom&fontSize=48&fontColor=fff&desc=AI%20Engineer%20%7C%20RAG%20%26%20RL%20Systems%20%7C%20Web3&descFontSize=18&fontAlign=25&descAlign=78" width="100%"/>
</div>

<div align="center">
  <img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&weight=600&size=22&pause=1000&color=256EFF&center=true&vCenter=true&width=650&lines=AI+Engineer+%7C+Informatics+Graduate;RAG+Systems+%C2%B7+Reinforcement+Learning+%C2%B7+LLM+Serving;Local-first+inference+%26+decentralized+infrastructure" alt="Typing SVG" />
</div>

<br>

## 👨‍💻 About

**AI Engineer** dengan latar Informatika (S.Kom). Fokus di sistem RAG produksi, reinforcement learning multi-agent, dan LLM serving yang efisien di hardware terbatas. Sampingan di Web3 — smart contract & DeFi primitives.

Prinsip kerja: **ukur dulu, klaim belakangan.** Semua angka di bawah ini punya konteks hardware dan bisa direproduksi dari repo-nya.

<br>

## 🛠 Tech Stack

<div align="center">

**AI / ML**

<img src="https://skillicons.dev/icons?i=py,pytorch,tensorflow,fastapi&theme=dark" alt="AI Stack" />

`RAG` · `Reinforcement Learning` · `Ray RLlib` · `MLflow` · `ChromaDB` · `llama.cpp` · `Quantization`

**Web3**

<img src="https://skillicons.dev/icons?i=solidity,ts,nextjs&theme=dark" alt="Web3 Stack" />

`Hardhat` · `OpenZeppelin` · `wagmi` · `BEP-20`

**Core**

<img src="https://skillicons.dev/icons?i=java,docker,kubernetes,linux&theme=dark" alt="Core Stack" />

</div>

<br>

## ⚔️ Featured Projects

### 🔒 [MicroLLM-PrivateStack](https://github.com/loxleyftsck/MicroLLM-PrivateStack) — Private LLM Infrastructure

LLM stack lokal, zero external API call. DeepSeek-R1-1.5B (Q4) via llama-cpp-python.

Benchmark di **Intel i5-12400, 2GB RAM**:

| Metrik | Hasil |
| :--- | :--- |
| Inference (uncached) | 280 ms |
| Inference (cached) | 18 ms — **15.5x** lebih cepat |
| Cache lookup (SoA-optimized) | 0.2 ms |
| Throughput | 450 req/s dengan caching |
| Security overhead | < 50 ms/request |

OWASP ASVS Level 2 · prompt-injection guard · PII masking otomatis · Docker + K8s
`Flask` `llama-cpp-python` `SQLite` `JWT` `Electron` · 61 commits · MIT

---

### 🇮🇩 [IndoGovRAG](https://github.com/loxleyftsck/IndoGovRAG) — Regulatory RAG untuk Peraturan Pemerintah

Hybrid retrieval (BM25 + vector) di atas ChromaDB, generation via Gemini API. 53 chunk dokumen dari 17+ kategori regulasi.

**Catatan jujur:** akurasi retrieval terukur baik pada korpus ini, tapi response time masih 10–60 detik karena keterbatasan free-tier API — bukan masalah arsitektur, tapi belum diselesaikan.

`FastAPI` `Next.js 14` `ChromaDB` `Gemini` · CI/CD · test suite · Docker · 59 commits

---

### 🤖 [EquilibriumX](https://github.com/loxleyftsck/EquilibriumX-Multi-Agent-Negotiation-Sandbox) — Multi-Agent Negotiation Sandbox

Platform negosiasi hybrid: RL agent + LLM untuk komunikasi bahasa natural. Distributed training via Ray RLlib, eksperimen dilacak dengan MLflow.

<!-- TODO Herald: klaim "95% konvergensi Nash dalam <100 iterasi" belum ada di README repo.
     Kalau angkanya nyata, taruh tabel hasil + script reproduksinya di repo, baru tulis di sini.
     Kalau belum diukur rapi, biarkan deskripsi kualitatif seperti sekarang. -->

`Python` `Ray RLlib` `MLflow` · notebooks + docs + draft paper · 25 commits

---

### 🥩 [BNB Staking DApp](https://github.com/loxleyftsck/bnb-staking-dapp) — DeFi Staking Protocol

BEP-20 token (HLD, max supply 10M) + StakingPool dengan reward akrual per detik, APR 10%, emergency withdrawal.

- **37 test lulus** (Chai + Hardhat)
- Gas: stake ~75.000 · unstake ~85.000 (termasuk mint reward)
- ReentrancyGuard, role-based minting, pausable

`Solidity 0.8.20` `OpenZeppelin v5.4.0` `Hardhat 2.22` · BSC Testnet · MIT

> ⚠️ Testnet only — belum diaudit eksternal, jangan dipakai dengan dana riil.

<!-- TODO Herald: klaim "30% gas savings" butuh baseline pembanding.
     Ukur staking pool standar, taruh tabel before/after, baru klaim. Kalau tidak, biarkan angka gas absolut di atas — itu sudah informatif. -->

---

### 📡 [CARL-DTN](https://github.com/loxleyftsck/CARL-DTN) — Context-Aware RL Routing

Protokol routing untuk Delay Tolerant Network: Q-Learning + evaluasi konteks multi-dimensi (resource fisik, metrik sosial, properti pesan) + adaptive copy control berbasis densitas jaringan.

Dievaluasi terhadap Epidemic, PRoPHET, dan Spray-and-Wait pada delivery probability, overhead ratio, dan latency.

`Java` `ONE Simulator v1.4.1` `Fuzzy Logic (FCL)` · GPL v3

<!-- TODO Herald: hasil numerik benchmark belum ada di README repo. Tambahkan tabel hasil di sana dulu. -->

<br>

## 🔭 Current Focus

- 🚧 **Building** — Inverse RL agent untuk optimasi portofolio kripto (`Stable-Baselines3`). Baseline pembanding: HODL.
- 📝 **Researching** — ZK-SNARK privacy layer untuk DAO governance. Target: draft paper ICBC.
- 📚 **Learning** — Harness engineering & eval-driven development untuk sistem agentic.

<br>

## 📈 Activity

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=loxleyftsck&show_icons=true&theme=radical&hide_border=true&bg_color=0D1117&count_private=true" height="160" alt="GitHub Stats" />
  <img src="https://streak-stats.demolab.com/?user=loxleyftsck&theme=radical&hide_border=true&background=0D1117" height="160" alt="GitHub Streak" />
</div>

<br>

## 📫 Connect

<div align="center">
  <a href="https://www.linkedin.com/in/herald-michain-samuel-theo-ginting-9b70762a3/">
    <img src="https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
  <a href="mailto:heraldmsamuelginting@gmail.com">
    <img src="https://img.shields.io/badge/Email-Contact-red?style=for-the-badge&logo=gmail&logoColor=white" />
  </a>
</div>

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=0,2,30&height=100&section=footer"/>
</div>
