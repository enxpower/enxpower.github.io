# Decision Log

## Active Decisions

- Decision: Initial Project Context Pack added.
  Reason: Future AI coding sessions need a reliable project baseline instead of relying on chat history.
  Impact: Future sessions should read `CLAUDE.md` and docs files before making changes.

- Decision: This repository remains a static official website.
  Reason: Inspection found `index.html` and `CNAME`, with no root `README.md` or root `package.json`.
  Impact: Future work must not add a build system, framework, dependency, or package file unless explicitly approved.

- Decision: The canonical public domain is `agim.ca`.
  Reason: The root `CNAME` file contains `agim.ca`, and `index.html` uses `https://agim.ca/` in canonical and social metadata.
  Impact: Do not change domain routing, canonical URLs, or public routes without explicit approval.

- Decision: AGI&M visual identity governs the public surface.
  Reason: The site is the official AGI&M Assets Inc. website.
  Impact: Future UI work must preserve a serious, institutional, execution-oriented, and infrastructure-grade AGI&M presentation.

- Decision: Public messaging must remain holding-company and infrastructure focused.
  Reason: The site positions AGI&M as a Canadian holding company across energy infrastructure, power equipment, and autonomous industrial systems.
  Impact: Future copy must not drift into generic startup, consumer app, or unsupported investment claims.
