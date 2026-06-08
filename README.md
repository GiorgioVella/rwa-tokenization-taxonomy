# A Taxonomy of Real-World Asset Tokenization for Blockchain-Based Financial Infrastructure

This repository contains the replication dataset and classification matrix accompanying the paper:

> Vella, G., Pennella, L., & Ballandies, M. C. (2026). *A Taxonomy of Real-World Asset Tokenization for Blockchain-Based Financial Infrastructure.*

The paper develops a system-level taxonomy of Real-World Asset (RWA) tokenization composed of **23 attributes** organized across **five components** — Governance, Asset, Token Properties, Distributed Ledger Technology (DLT), and Economy — and applies it to the **20 largest RWA tokenization protocols** by market capitalization listed on the [DeFiLlama RWA dashboard](https://defillama.com/rwa).

> **Note on the canonical link.** The footnote in the paper points to this repository as the official source for the classification data. Earlier drafts referenced a different URL; this repository under `GiorgioVella/` is the authoritative replication package.

## Contents

The dataset is provided as a single workbook, `REPO_Final_RWA_Taxonomy___Classification__20_SYSTEMS.xlsx`, with four sheets:

| Sheet | Description | Maps to |
|---|---|---|
| `Final RWA Taxonomy` | The taxonomy matrix: components, attributes, sub-attributes, definitions, and permitted values. | Appendix A, Table VI |
| `Classification Work` | The 20 protocols classified across the 23 attributes, with protocol ID, classification date, and market-cap ranking. | Tables I–V |
| `Sources` | 460 per-assignment source citations. Each row documents one attribute→value assignment with rationale, access date, source type, confidence level, supporting text excerpt, and link. | — |
| `DefiLlama Top 100 RWA` | Snapshot of the DeFiLlama RWA dashboard (February 2026) used as the external sample-selection criterion. | Section V |

## The 20 classified protocols

The sample is the top 20 RWA protocols by market capitalization as listed on DeFiLlama in February 2026:

1. Tether Gold (XAUt)
2. BUIDL
3. PAX Gold
4. US Yield Coin (UYSC)
5. Superstate USTB
6. WisdomTree Treasury Money Market Digital Fund (WTGXX)
7. Janus Henderson Anemoy AAA CLO Fund (JAAA)
8. Janus Henderson Anemoy Treasury Fund (JTRSY)
9. Ondo OUSG
10. BlackRock USD Institutional Digital Liquidity Fund – I Class (BUIDL-I)
11. Hastra PRIME (PRIME)
12. Franklin OnChain U.S. Government Money Fund (BENJI)
13. Superstate Crypto Carry Fund (USCC)
14. Exodus Movement, Inc. Class B (EXODB)
15. Theo Network thBill (thBILL)
16. Fidelity Digital Interest Token (FDIT)
17. EUTBL by Spiko (EUTBL)
18. Spiko US T-Bills Money Market Fund (USTBL)
19. Mantle Index Four Fund (MI4)
20. mF-ONE (MF-ONE)

## Methodology summary

The taxonomy was developed following the iterative method of Nickerson et al. (2013), combining empirical-to-conceptual and conceptual-to-empirical iterations. Classification of each protocol is based exclusively on publicly available documentation: official protocol documentation, legal documents, product pages, smart-contract references, audit and attestation reports, regulatory filings, and on-chain information.

Every attribute→value assignment in the classification is backed by an entry in the `Sources` sheet, recording the supporting text, access date, source type, and a confidence level (High / Medium / Low). Where documentation does not explicitly verify a characteristic, the value is recorded as `N/A`; where a protocol exhibits a relevant characteristic outside the predefined values, it is recorded as `Other` and documented separately.

## How to use this dataset

- To reproduce **Tables I–V** of the paper, read the `Classification Work` sheet (header rows 1–3 define Component → Attribute → Sub-Attribute; data begin at row 4).
- To audit any single classification decision, filter the `Sources` sheet by `System` and `Attribute`.
- To reproduce the **sample selection**, see the `DefiLlama Top 100 RWA` sheet.

## Citation

If you use this dataset, please cite the paper. A machine-readable citation is provided in [`CITATION.cff`](CITATION.cff). A `.bib` entry will be added once the arXiv identifier is assigned.

## License

The contents of this repository are released under the
[Creative Commons Attribution 4.0 International (CC BY 4.0)](LICENSE) license,
consistent with the open-access terms applied to the paper.

## Authors

- **Giorgio Vella** — School of Banking, Finance and Insurance, Università Cattolica del Sacro Cuore, Milano, Italy
- **Luca Pennella** — Interdisciplinary Centre for Security, Reliability and Trust, University of Luxembourg
- **Mark C. Ballandies** — Blockchain and Distributed Ledgers, University of Zurich
