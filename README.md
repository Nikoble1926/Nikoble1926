### Hi, I am Nikolaos (Nikoble1926)

I build and operate **nsgoods**, a live suite of signed, pay per call data oracles on the x402 protocol. Every response is a signed, verifiable verdict, not just JSON.

**What is live right now**

- **12 x402 services** running in production, each pay per call over HTTP 402
- **Sanctions screening**: `/screen` (single address) and `/screen-multi` (one address against four lists: OFAC, UN, EU, UK), returning signed verdicts
- **payable v3**: metered, dual format 402 challenge on every endpoint
- **Observatory**: on chain forensics and proof of payment verification
- **Reproductions**: independent, verifiable rebuilds of published results

**How it works**

- Signed with **EIP-191**; verdicts are canonicalized and independently verifiable by anyone
- Runs across **Base** and **Solana**
- Payment is settled per call; you pay only for a successful `2xx` response

**Integrations, in production**

- **Walpulse** renders our signed sanctions verdicts inside its own product UI and verifies the signature on every render ([case study](https://x402.nsgoods.org/proof/case-studies/walpulse.html))
- **SafeGate** references our signed screening verdict by its hash and request id in its paid evidence ([case study](https://safegate-nsgoods-case-study.vercel.app/))
- **Waveline × nsgoods**: checked end to end before it opened to agents, first mainnet payment, and the x402 docs ([PR #38](https://github.com/dimopapa91/music-insight-pipeline/pull/38))

**Hub**: [x402.nsgoods.org](https://x402.nsgoods.org)

Open to interesting work in agentic commerce, x402 integrations, and verifiable data services.
