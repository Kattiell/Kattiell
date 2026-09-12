<h1>Gabriel Caetano</h1>

<p>
  <strong>QA Engineer</strong> — API testing, test automation and release gates.<br>
  Patos de Minas, Minas Gerais, Brazil.
</p>

<p>
  <a href="https://www.linkedin.com/in/gabriel-caetano-28a16317a/">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:gabrielcaetanopf.contato@gmail.com">
    <img src="https://img.shields.io/badge/e--mail-informational?style=flat&logo=gmail&logoColor=white" alt="e-mail"></a>
</p>

---

### What I do

I test the part of a system that nobody sees until it breaks: the API boundary.

At **B2LIST** I work on the quality of a platform being rewritten service by
service — designing test scenarios from requirements, building request suites
across dozens of endpoints, running load and batch-import stress tests, and
turning the results into bug reports a developer can act on without a second
conversation.

Most of my work is the unglamorous half of QA: deciding *what* is worth testing
before writing a single assertion, and making sure the evidence survives the
meeting.

---

### Featured — [parity-gate](https://github.com/Kattiell/parity-gate)

**A CI gate that proves an API rewrite did not break the contract.**

It runs the same requests against the old service and the new one and reports
what a consumer would actually notice: a field that changed type, a value that
is now `null`, a `404` that quietly became a `200`.

The hard part is not the diff — it is the noise. Two live services return
different timestamps on every call, pages come back reordered, and one flaky
endpoint makes an entire report untrustworthy. So the tool masks volatile paths
(and proposes the masks itself), matches collections by identity instead of by
position, and measures whether an endpoint is stable *before* comparing anything.

Every run leaves a hash-chained evidence bundle: a report for the ticket, a
machine-readable record, and a requirement traceability matrix.

<sub>Python 3.11+ · zero runtime dependencies · 97 tests on Linux and Windows ·
includes the test strategy, an ADR, and three written bug reports</sub>

---

### What I work with

**Testing** &nbsp;API & contract testing · exploratory testing · risk-based test
design · load and stress testing · bug reporting · test strategy · traceability

**Tools** &nbsp;Postman · pytest · Insomnia · ClickUp · Git / GitHub Actions · Docker

**Code** &nbsp;Python · JavaScript / TypeScript · SQL · Java

**Data** &nbsp;SQL Server · PostgreSQL · MongoDB

---

### Other things I have built

| | |
| --- | --- |
| [**parity-gate**](https://github.com/Kattiell/parity-gate) | Contract-parity gate for API migrations, with an auditable evidence trail |
| [**cnpj_validator**](https://github.com/Kattiell/cnpj_validator) | CNPJ validation, the boring correctness kind |
| [**SplitExcel**](https://github.com/Kattiell/SplitExcel) | Splitting spreadsheets that were never meant to be that large |
| [**PetTracker**](https://github.com/Kattiell/PetTracker) | Full-stack side project — TypeScript front end and API |

---

<sub>"Do a little or do a lot, but do something every day."</sub>
