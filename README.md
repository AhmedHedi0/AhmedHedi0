# Ahmed Hedi Abidi

Backend engineer in Passau, Germany. For the past year I have built production Python at
[Checkmk](https://github.com/Checkmk/checkmk), an open-source infrastructure-monitoring product:
a crash-reporting library and CLI, FastAPI endpoints behind mTLS, and asyncio daemons that run at
customer sites. M.Sc. Computer Science, Universität Passau (thesis submitted).

## Selected production work

Merged into Checkmk and public on GitHub:

- **Crash reporting for every edition.** I extracted the crash-reporting core into its own package
  ([cmk-crash](https://github.com/Checkmk/checkmk/commit/a0ebe4b19b4026e7f7586d206543fedc59cbc0fd),
  [moved out of the GUI](https://github.com/Checkmk/checkmk/commit/b9e7543cfbe30374936be199ab7e2f6a23b650fb)),
  added a [batch-upload CLI](https://github.com/Checkmk/checkmk/commit/a2b37a9f1475fc18433e54d9982ed478284af1cc),
  a [daily upload](https://github.com/Checkmk/checkmk/commit/a2e00f5cf16de832958cd037fd52b7d843461926)
  that [stops on any retryable failure](https://github.com/Checkmk/checkmk/commit/c0df30a8fe50226523d51b6186461855b30df294),
  and an [opt-in admin setting](https://github.com/Checkmk/checkmk/commit/fc26cdf2fbcf9582a2851134619cd117283a75a4).
- **Relay-to-site crash forwarding.** A
  [FastAPI endpoint](https://github.com/Checkmk/checkmk/commit/e2713cf57531bbfe629693ed57bf288ebccdead2)
  that accepts reports forwarded by the relay, and the
  [relay client](https://github.com/Checkmk/checkmk/commit/ed9b1565c419faec377f658654ada667b059fc42)
  that sends them and deletes its copy only after the site acknowledges it.
- **A relay daemon that does not die silently.** Every background task
  [now writes a crash report](https://github.com/Checkmk/checkmk/commit/7cea302a593f86c9caa9ed03f76afc6a149fb94e),
  reports [redact private keys by their value](https://github.com/Checkmk/checkmk/commit/405d5ec884537ec8f0fe81fc5a21f88549f378a9),
  and [crash.info is written atomically](https://github.com/Checkmk/checkmk/commit/3e05fe1299c301c8b31a8cfae873103ce073931e).
- **Usage data for Cloud trials.** [Session statistics](https://github.com/Checkmk/checkmk/commit/023ee55e7cb1f1a9ffcde311864a08d07b769ce1)
  and [trial users counted by email domain](https://github.com/Checkmk/checkmk/commit/724c9a59a367c758bb30f436f2c345cca8b6d9be).

## Projects

- [Web3](https://github.com/AhmedHedi0/Web3): Spring Boot / PostgreSQL REST API with a React
  frontend that issues ERC-20 tokens; Cloud Run, GitHub Actions.
- [PowerAnalysisAttack](https://github.com/AhmedHedi0/PowerAnalysisAttack): Python framework for
  power side-channel analysis of AES-128 on an FPGA; recovered keys with DPA and CPA.
- [ai-in-software-projects-csf](https://github.com/AhmedHedi0/ai-in-software-projects-csf):
  systematic literature review of how AI affects success factors in software projects, with the
  PRISMA search and screening scripts.

Merged upstream: [code-annotation#59](https://github.com/ductnguyen12/code-annotation/pull/59).

[LinkedIn](https://linkedin.com/in/ahmed-hedi-abidi-ba4771214)
