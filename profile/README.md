<p align="center">
  <a href="https://pgcircuit.com">
    <img src="https://raw.githubusercontent.com/PG-Circuit/pg-circuit/main/docs/assets/banner-readme.png" alt="PG Circuit — PostgreSQL circuit breaker and runtime protection" width="420"/>
  </a>
</p>

<p align="center">
  <strong>PG Circuit</strong><br/>
  Runtime protection for PostgreSQL · A circuit breaker that runs inside Postgres
</p>

<p align="center">
  <a href="https://pgcircuit.com">Website</a> ·
  <a href="https://pgcircuit.com/docs">Docs</a> ·
  <a href="https://pgcircuit.com/pricing">Pricing</a> ·
  <a href="https://github.com/PG-Circuit/pg-circuit">Open source (Community)</a>
</p>

---

## What we build

**PG Circuit** is a [PostgreSQL circuit breaker](https://pgcircuit.com) and **runtime protection** extension. It scores risky SQL against live locks, replication lag, and database pressure, then **ALLOW**, **WARN**, or **BLOCK** — so production stays safe from:

- `DELETE` / `UPDATE` without `WHERE`
- `TRUNCATE` / `DROP`
- Destructive DDL under pressure

Unlike migration linters or proxies, PG Circuit runs **inside PostgreSQL** and sees live database state.

| Product | Availability |
|--------|--------------|
| **[Community](https://github.com/PG-Circuit/pg-circuit)** | Public on GitHub · Apache 2.0 · free forever |
| **[Pro](https://pgcircuit.com/pro)** | Commercial · sales · not a public GitHub repo |
| **[Cloud](https://pgcircuit.com/cloud)** | Commercial · sales · not a public GitHub repo |
| **[Enterprise](https://pgcircuit.com/pricing)** | Contracted support |

> Only **Community** (`pg-circuit`) is open source. Pro and Cloud ship via [pgcircuit.com](https://pgcircuit.com) — their source stays private.

---

## Open source on GitHub

<table>
  <tr>
    <td width="80">
      <a href="https://github.com/PG-Circuit/pg-circuit">
        <img src="https://raw.githubusercontent.com/PG-Circuit/pg-circuit/main/docs/assets/logo.png" alt="pg-circuit" width="56"/>
      </a>
    </td>
    <td>
      <strong><a href="https://github.com/PG-Circuit/pg-circuit">pg-circuit</a></strong> — Community<br/>
      Circuit breaker for production PostgreSQL. Native extension · deterministic risk · observe / warn / enforce.<br/>
      <code>postgresql</code> · <code>circuit-breaker</code> · <code>database-security</code> · <code>sql-guardrails</code>
    </td>
  </tr>
</table>

```sql
DELETE FROM users;
-- ERROR: PG Circuit blocked high-risk operation (Risk: 95/100)
```

---

## Learn more

- **Website:** [pgcircuit.com](https://pgcircuit.com)
- **Docs / quick start:** [pgcircuit.com/docs](https://pgcircuit.com/docs)
- **Pro & Cloud:** [pricing](https://pgcircuit.com/pricing) · [sales](mailto:sales@pgcircuit.com)
- **Packaging & install:** [PACKAGING.md](https://github.com/PG-Circuit/pg-circuit/blob/main/PACKAGING.md)
- **Contact:** [hello@pgcircuit.com](mailto:hello@pgcircuit.com)

<p align="center">
  <sub>
    Keywords: PostgreSQL extension · Postgres circuit breaker · SQL guardrails · query firewall ·
    runtime protection · destructive query protection · database safety · SRE · DBA tooling
  </sub>
</p>
