# Hi, I'm Felix 👋

Third-year Computer Science student at Maynooth University,
**currently looking for a software engineering internship or placement for 2027.**

I'm drawn to backend work, APIs, databases, and figuring out why something is
actually slow rather than guessing at it. Most of what I've enjoyed building has
been for people who had no interest in the software itself and just needed it to
work, which turns out to be a good teacher.

---

### 🏭 SMT Downtime & OEE Tracker - Abbott Diabetes Care
*Python · Flask · Azure SQL · Chart.js · Power BI · Azure App Service*

Sole developer on a production monitoring system now running on the factory floor.
Three production lines were tracking downtime on a hand-filled Excel workbook, so I
reverse-engineered its formula logic and rebuilt it as a web app where the counts
come directly from machine counter readings.

- ~10,300 lines over 166 commits · 24 routes · 12-table Azure SQL schema
- Operator console for logging machine states in real time, with reason codes and
  shift/crew tracking
- Three OEE metrics implemented to the plant's specification, each with different
  downtime-exclusion rules
- Live drill-down dashboard: factory overview → line → machine, with traffic-light
  thresholds
- Cut page loads from 2.7s by reducing database round-trips from 8 connections to 1
- Enforced quality workflow - unscheduled downtime locks a machine until a technician
  logs a root cause, validated server-side so no step can be skipped
- Deployed via GitHub Actions CI/CD, with a 20-page handover pack for the enterprise
  IT team

*Private repository - happy to walk through the architecture.*

---

### 📍 Location Recommender - mentored by Microsoft Ireland
*Spring Boot · React Native · PostgreSQL/PostGIS · Microsoft Entra ID*

A social location-review app built by a team of six over four months, working in
agile sprints with code review and weekly mentor check-ins.

I owned authentication end to end: Microsoft Entra External ID using the OAuth 2.0
PKCE flow with JWT validation. Most of that work was reading Azure documentation for
a system I didn't understand yet and chipping away at redirect-URI and guest-access
errors until I did. We demoed the finished app to a room of Microsoft engineers at
the Placemark showcase.

**[→ Repository](https://github.com/azriel0508/location-recommender)**

---

### 🗂️ AI File Sorter
*Python · OpenAI API*

A command-line tool that clears out messy directories on its own. It reads a short
preview of each file, works out what the file actually is, generates sensible folder
categories, and moves everything into place.

- Classifies by **content**, not filename - so `doc1.pdf` and `untitled(3).docx`
  still land in the right folder
- Generates the category structure from what it finds, rather than sorting into
  fixed buckets
- Structured prompting so the same directory produces the same result run to run
- Dry-run mode to preview the moves before anything is touched

Built it because my own Downloads folder was unusable. The interesting part wasn't
the API call, it was making the output *reproducible*, since a model that gives a
different answer each run is useless for a tool that moves your files around.

**[→ Repository](https://github.com/azriel0508/AI-File-Sorter)**

---

### 🛠️ Tools

**Languages** — Python · Java · SQL · JavaScript/TypeScript
**Backend** — Flask · Spring Boot · SQLAlchemy · REST APIs · OAuth 2.0
**Data** — PostgreSQL/PostGIS · Microsoft SQL · SQLite
**Infra** — Linux · Git · GitHub Actions · Azure App Service · Railway

---

### 📚 Also

I tutored Java, object-oriented design and debugging at Maynooth's CS Centre.

📫 **felix.elmido27@gmail.com** · [LinkedIn](https://www.linkedin.com/in/felix-azriel-elmido-4a1862296/)
