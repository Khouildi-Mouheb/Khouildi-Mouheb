<p align="center">
  <img src="./banner.svg" alt="mouheb@enit:~$ ./boot --ai --systems --security" width="100%">
</p>

```console
mouheb@enit:~$ systemctl status mouheb.service
● mouheb.service - Computer Engineering Student @ ENIT
     Loaded: loaded (/home/bizerte/tunisia; enabled; vendor preset: curious)
     Active: active (building) since 2022
       Docs: linkedin.com/in/mouheb-khouildi
   Main PID: 2026 (looking-for-a-pfe)
      Tasks: 4 repos — forecasting, social-media-microservices, MatchingJavaApp, Linux-toolkit
     Memory: Python · Django · FastAPI · LLMs · Docker · Linux
     CGroup: /ai/systems/security

Nov 09 mouheb[2026]: I like building AI products end to end — from architecture to deployment.
Nov 09 mouheb[2026]: Lately obsessed with agents, RAG, and systems that fix themselves.
Nov 09 mouheb[2026]: Breaking things on purpose to understand them (security edition).
```

<br>

## `$ kubectl get repos -n mouheb`

```console
NAME                          STATUS      TYPE            STACK
forecasting                   Completed   internship      Python · FastAPI · Prophet · XGBoost
social-media-microservices    Completed   backend         Node.js · Express · MongoDB · JWT
MatchingJavaApp               Completed   java            Java · Jaro-Winkler · strategy pattern
Linux-toolkit                 Running     sysadmin        Bash · Ubuntu
```

<details open>
<summary><b> <a href="https://github.com/Khouildi-Mouheb/forecasting">forecasting</a></b> — two models compete, the best one predicts your stock</summary>
<br>

A stateless demand-forecasting microservice I built at **JCD Commerce** for their multi-tenant ERP SaaS. The ERP sends a product's history, and the service sends back a forecast with confidence bounds.

- **Prophet vs. XGBoost:** both are benchmarked on holdout data (MAE, RMSE, MAPE, R²) and a `ModelSelector` serves the champion, falling back if a model fails to converge
- **XGBoost features:** calendar signals, lags 1–7, rolling mean and std, recursive multi-step forecasting
- **Clean pipeline:** daily reindexing with zero-filling, same-day aggregation, negative-stock anomaly removal
- **Hexagonal architecture** with a FastAPI driving adapter, Swagger docs at `/docs`, tested with pytest

```http
POST /api/v1/forecast   { "itemId": "...", "horizon": 7, "modelType": null, "history": [...] }
```
</details>

<details>
<summary><b> <a href="https://github.com/Khouildi-Mouheb/social-media-microservices">social-media-microservices</a></b> — a social network backend split into six services</summary>
<br>

A REST backend for a social media app where every feature lives in its own Node.js service, behind one API gateway.

```console
gateway :3000  ──▶  users · posts · stories · comments · friendships
```

- **Gateway** routes `/api/*` requests and handles JWT authentication
- **Users:** registration, login, profiles, follow / unfollow
- **Posts & comments:** posts, nested replies, likes
- **Stories:** ephemeral stories with view tracking
- **Friendships:** full request workflow (send, accept, reject, cancel) with mutual friends
- Node.js + Express + MongoDB, JWT auth
</details>

<details>
<summary><b> <a href="https://github.com/Khouildi-Mouheb/MatchingJavaApp">MatchingJavaApp</a></b> — fuzzy name matching in Java</summary>
<br>

A modular engine where every stage is swappable: **preprocessing** (normalization, phonetic), **candidate generation**, **comparison** (exact, Jaro-Winkler) and **selection** (threshold or top-N), over CSV datasets.
</details>

<details>
<summary><b> <a href="https://github.com/Khouildi-Mouheb/Linux-toolkit">Linux-toolkit</a></b> — my growing box of Bash tools</summary>
<br>

Command-line utilities for automation, system administration and security, written in Bash on Ubuntu.
</details>

<br>

## `$ cat ~/.stack.yaml`

```yaml
languages:   [Python, Java, C, JavaScript/TypeScript, SQL, Bash, Dart]
backend:     [Django, FastAPI, Flask, Node.js, React]
ai:          [LLMs, RAG, ChromaDB, Transformers, scikit-learn, TensorFlow, XGBoost, Prophet]
infra:       [Linux, Docker, Kubernetes, Nginx, Azure Container Apps, Datadog, k6]
security:    [Wireshark, Nmap, iptables, OpenSSL, Kali Linux, Burp Suite, Metasploit]
databases:   [PostgreSQL, Oracle, MongoDB, SQLite]
learning:    [local LLMs, observability, self-healing systems]
```

<br>

## `$ journalctl -u mouheb --since 2022`

```console
2022  ▸ joined IPEIG prépa in Gabès — two years of maths, physics and sleepless nights
2024  ▸ entered ENIT, Computer Engineering
2026  ▸ AI / forecasting intern at JCD Commerce
2026  ▸ shipped a forecasting microservice into a real ERP
now   ▸ looking for a PFE in AI systems, SRE or security   ← you are here
```

<br>

## `$ ./contact.sh`

<p>
  <a href="https://linkedin.com/in/mouheb-khouildi"><img src="https://img.shields.io/badge/linkedin-mouheb--khouildi-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=0d1117"></a>
  <a href="mailto:khouildimouheb6@gmail.com"><img src="https://img.shields.io/badge/mail-khouildimouheb6@gmail.com-3fb950?style=for-the-badge&logo=gmail&logoColor=white&labelColor=0d1117"></a>
</p>

```console
mouheb@enit:~$ echo "got an interesting problem? let's talk."
got an interesting problem? let's talk.
mouheb@enit:~$ █
```