<h1>Gabriel Caetano</h1>

<p>
  <strong>QA Engineer</strong> · Patos de Minas, Minas Gerais, Brazil<br>
  Professionally suspicious. I break things on purpose so nobody does it by accident.
</p>

<p>
  <a href="https://www.linkedin.com/in/gabriel-caetano-28a16317a/">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:gabrielcaetanopf.contato@gmail.com">
    <img src="https://img.shields.io/badge/e--mail-informational?style=flat&logo=gmail&logoColor=white" alt="e-mail"></a>
  <a href="https://github.com/Kattiell/parity-gate">
    <img src="https://img.shields.io/badge/featured-parity--gate-success?style=flat" alt="parity-gate"></a>
</p>

---

### The job, honestly

Someone has to be the person who asks what happens when the quantity field gets
a negative number, and I enjoy it more than is probably healthy.

Day to day I work on the quality of a platform being rewritten service by
service at **B2LIST**: turning requirements into test scenarios, building request
suites across dozens of endpoints, pushing batch imports until something gives,
and writing the bug up well enough that the developer doesn't need a second
conversation about it.

The half nobody puts on a CV is the half I actually care about — deciding *what
is worth testing* before writing a single assertion, and making sure the evidence
still stands up in the meeting where someone says "but it worked yesterday".

---

### The first things I try

Not a checklist. Just where the bodies are usually buried.

| | |
| --- | --- |
| **Empty** | `[]` where the code plainly expects at least one item |
| **Twice** | the same request again, fast, before the first one has settled |
| **Zero** | `0`, `0.00`, and the difference between `0` and `null` that nobody decided on |
| **Off by one** | page `0`. page `-1`. page `999999`. |
| **Wrong type** | a string where someone assumed a number — and the reverse, which is worse |
| **Unicode** | `José`, `北京`, and an emoji in a field sized for initials |
| **Absence** | the required field, simply not sent |
| **The back button** | the one nobody tests, ever |

---

### Featured — [parity-gate](https://github.com/Kattiell/parity-gate)

**A CI gate that proves an API rewrite did not break the contract.**

It fires the same requests at the old service and the new one, then reports what
a consumer would actually notice: a field that changed type, a value that is now
`null`, a `404` that quietly became a `200`.

The hard part was never the diff. Two live services return different timestamps
on every call, pages come back reordered, and one flaky endpoint makes an entire
report untrustworthy — that is how these harnesses end up switched off within a
quarter. So it masks volatile paths *and proposes the masks itself*, matches
collections by identity instead of by position, and measures whether an endpoint
is stable **before** comparing anything.

Every run leaves a hash-chained evidence bundle: a report for the ticket, a
machine-readable record, and a requirement traceability matrix.

<sub>Python 3.11+ · zero runtime dependencies · 98 tests, Linux and Windows ·
ships with the test strategy, an ADR, and three written bug reports</sub>

---

### What I work with

**Testing** &nbsp;API & contract testing · exploratory testing · risk-based test design ·
load and batch stress testing · bug reporting · test strategy · traceability

**Tools** &nbsp;Postman · pytest · Insomnia · ClickUp · Git / GitHub Actions · Docker

**Code** &nbsp;Python · JavaScript / TypeScript · SQL · Java

**Data** &nbsp;SQL Server · PostgreSQL · MongoDB

---

### Other things I have built

| | |
| --- | --- |
| [**parity-gate**](https://github.com/Kattiell/parity-gate) | Contract-parity gate for API migrations. The one I'd want you to read. |
| [**cnpj_validator**](https://github.com/Kattiell/cnpj_validator) | Check digits and the CNPJs that are technically valid and absolutely fake |
| [**SplitExcel**](https://github.com/Kattiell/SplitExcel) | For spreadsheets that were never meant to get that large |
| [**PetTracker**](https://github.com/Kattiell/PetTracker) | Full-stack side project, TypeScript front to back |
| [**racing-game**](https://github.com/Kattiell/racing-game) | Because not everything needs a test plan |

---

### Off the clock

Lo-fi on, always one more side project open than I can reasonably finish. A few
of them are up here: a Telegram trading bot, an e-commerce, a racing game, and a
horror visual novel from university that I still think holds up.

<sub>Falo português — quebro software em qualquer idioma.<br>
<em>"Do a little or do a lot, but do something every day."</em></sub>
