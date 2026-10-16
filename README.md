<div align="center">

<img src="assets/Rick.gif" alt="Rick coding" width="260"/>

</div>

```http
GET /v1/daniel HTTP/1.1
Host: github.com/DBermudez23
Accept: application/json
```

```http
HTTP/1.1 200 OK
Content-Type: application/json
X-Origin: Colombia
X-Default-Layer: backend
X-Chaos-Level: controlled
```

```json
{
  "name": "Daniel Bermúdez",
  "role": "Full-stack developer",
  "starts_from": "the database schema, never the button",
  "believes": "a good UI is just an honest view over a well-designed model",
  "currently_building": "[project] — [one line on what it solves]",
  "currently_breaking": "[thing you're learning by taking it apart]",
  "open_to": ["backend roles", "weird side projects", "systems that need untangling"]
}
```

---

## Endpoints

<details>
<summary><code>GET /stack</code> → what I reach for, and when</summary>

```json
{
  "when_it_must_not_fail":       [".NET", "C#", "PostgreSQL"],
  "when_it_must_ship_yesterday": ["NestJS", "Node.js", "Prisma", "Supabase"],
  "when_it_has_to_be_fast":      ["Redis"],
  "when_it_is_glue_or_a_script": ["Python", "Bash"],
  "when_a_human_has_to_use_it":  ["React", "TypeScript", "Tailwind CSS"],
  "where_it_lives":              ["Docker", "Linux", "GitHub", "GitLab"],
  "legacy_i_can_still_read":     ["PHP", "MySQL", "Express"]
}
```

</details>

<details>
<summary><code>GET /projects</code> → things that actually run</summary>

```json
[
  {
    "name": "[project-one]",
    "solves": "[the problem, in one line]",
    "stack": ["[tech]", "[tech]"],
    "hardest_decision": "[the trade-off you'd defend in an interview]",
    "repo": "[link]"
  },
  {
    "name": "[project-two]",
    "solves": "[the problem, in one line]",
    "stack": ["[tech]", "[tech]"],
    "hardest_decision": "[the trade-off you'd defend in an interview]",
    "repo": "[link]"
  }
]
```

</details>

<details>
<summary><code>GET /process</code> → the pipeline every feature goes through</summary>

```bash
$ cat idea.txt | make_it_work | understand_it | clean_it | simplify_it | ship_it
```

If a step fails, the pipeline restarts. Skipping `understand_it` is not supported.

</details>

<details>
<summary><code>POST /collab</code> → reach me</summary>

```bash
curl -X POST https://danielbermudez.netlify.app \
  -d '{"from": "you", "idea": "something worth building"}'
```

Or, less dramatically:
[Portfolio](https://danielbermudez.netlify.app/) · [LinkedIn](https://www.linkedin.com/in/dbermudez23/) · [danielbermudezwuw@gmail.com](mailto:danielbermudezwuw@gmail.com)

</details>

---

## Status codes

| Code | What it means around here |
|------|---------------------------|
| `200` | It works and I know why. |
| `201` | Shipped. |
| `304` | Refactored it. Does exactly the same thing. Now a human can read it. |
| `418` | I'm a teapot. Ask me about Colombian coffee instead. |
| `422` | Your requirements contradict each other. Let's talk before I write code. |
| `500` | It works and I don't know why. Not done yet. |
| `503` | Lost in another dimension. Back after this portal closes. |

---
<br>
<img src="assets/ricksanchez.gif" alt="Rick Sanchez coding" width="120" align="right"/>
</br>
## Known issues

- **#12** — Rewrites working code "just to understand it". `wontfix`
- **#27** — Draws the database diagram before agreeing on the app's name. `by design`
- **#31** — Cannot leave a `TODO` without a date next to it. `wontfix`
- **#40** — Opens the network tab before reading the error message. `investigating`

<br clear="right"/>

---

```
Connection closed by remote host.
```
