# Mikel Fernandes

**Software / Systems / Engineering**

`Mumbai, India` · `Open to Software Engineering / Backend roles`

I build backend systems, APIs, and software that turns messy inputs into useful data. I’m interested in what happens behind the interface, especially when systems scale, fail, or behave unexpectedly.

[Portfolio](https://portfolio-webpage-sooty-phi.vercel.app/) 

---

## 01 / Engineering record

### API Rate Limiter

`DISTRIBUTED SYSTEMS / TRAFFIC CONTROL`

Rate-limiting middleware implementing **Token Bucket, Sliding Window, and Fixed Window** policies.

```text
Client → API nodes → Redis + Lua
                         ↓
                  Accept / HTTP 429
```

**Core idea:** multiple API nodes share a quota while atomic Redis Lua operations keep concurrent checks consistent.

**Notable details:** per-route policies, tier-based quotas, and explicit `429` / `Retry-After` responses.

**Recorded k6 load test:** approximately **140 requests/sec**, **5.7 ms average latency**, and **9.7 ms p95 latency**. Results describe the tested setup rather than a universal throughput guarantee.

**Stack:** Node.js · Express · Redis · Lua · Docker · k6 · Jest

[Inspect repository ↗](https://github.com/MikelBuilds/api-rate-limiter)

---

### Structify

`DOCUMENT INTELLIGENCE / EXTRACTION PIPELINE`

Converts unstructured PDFs into validated, structured data.

```text
PDF
 ├─ Digital → pdfplumber
 └─ Scanned → Tesseract OCR
                    ↓
              Extracted text
                    ↓
                  Gemini
                    ↓
                Validation
                    ↓
              Structured JSON
```

**Core idea:** separate document reading from interpretation. Extract the text, map it into a schema, then validate the result.

**Notable detail:** digital PDFs and scanned pages follow different extraction paths before entering the same structured-output pipeline.

**Stack:** Python · FastAPI · React · PostgreSQL · Gemini · Tesseract · pdfplumber

[Inspect repository ↗](https://github.com/MikelBuilds/Structify)

---

### PharmaWise

`APPLIED ML / HEALTHCARE WORKFLOWS`

A full-stack healthcare project combining Random Forest disease prediction, automated PDF lab-report extraction, and patient/doctor dashboards.

**Core idea:** connect prediction and document processing to the workflows where their outputs are actually reviewed and used.

**Notable detail:** the project also has a related IEEE conference paper.

**Stack:** Python · React · Machine Learning · OCR

[Inspect repository ↗](https://github.com/MikelBuilds/PharmaWise)

### Additional record

**[PeerLink ↗](https://github.com/MikelBuilds/PeerLink)** — nearby device discovery and offline messaging using Flutter, Dart, and Google’s Nearby Connections API. Supports Bluetooth / Wi-Fi communication with retry logic without relying on conventional internet connectivity.

---

## 02 / Working toolkit

- **Services:** Node.js, Express, FastAPI — APIs and backend logic.
- **Data:** PostgreSQL, Redis, MongoDB — persistence, caching, and shared state.
- **Interfaces:** React, Next.js, Tailwind CSS — web; Flutter — mobile.
- **Document intelligence:** Gemini, Tesseract, pdfplumber — interpretation and extraction.
- **Languages:** Python, JavaScript, TypeScript, C++, Dart.
- **Development & verification:** Git, GitHub, Postman, Docker, k6, Jest.

---

## 03 / Current log

Final-year Computer Engineering student at **Don Bosco Institute of Technology, Mumbai**.

Backend-leaning, with frontend and mobile development when the system needs an interface.

**Major project:** building a smart campus energy anomaly-detection system.

**Next chapter:** Software Engineering opportunities, particularly backend, APIs, distributed systems, and systems-oriented work.

**Away from the keyboard:** learning chess. Still debugging the opening.

---

## 04 / Practice, on record

**300+ DSA problems solved** across LeetCode and GeeksforGeeks.

**LeetCode peak rating:** 1594.

[LeetCode](https://leetcode.com/u/mikelfernandes/) 

---

**Have an interesting problem?**

[Portfolio](https://portfolio-webpage-sooty-phi.vercel.app/) · 

`END OF RECORD / STILL BUILDING`
