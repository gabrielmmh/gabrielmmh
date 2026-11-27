<div align="center">

# Gabriel Hermida

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/gabrielmmh/)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:gabrielhermida948@gmail.com)

**AI Engineer · LLM agents and evals**

BSc in Computer Engineering, [Insper](https://www.insper.edu.br/en/) (2026)

</div>

---

### What I'm Working On

**AI Engineer at Paggo**, a Brazilian B2B fintech (Applied AI and ERP teams):

- **Changelog Analyst:** for every merged PR, an LLM workflow writes the changelog and updates the affected help-center articles (AWS Lambda, SQS, SST, Neo4j AuraDB). I replaced the Gemini step that decides whether a change matters to customers with Jev, a typed-decision model: 0.3 s instead of two 7 s calls, at 1/45 of the cost
- **Internal Slack agent** on [Eve](https://github.com/vercel/eve): the tool layer with per-tool permissions, and the credential pool with failover in the inference router in front of it (145,000 LLM calls a month)
- **Agent observability:** cost and execution tracing in Langfuse for the company's agent framework (125,000 LLM calls a month), with PII redaction and a CI check against untraced code
- **Developer experience:** the plugin that standardizes how engineers use coding agents (Claude Code, Codex, Cursor, OpenCode and Eve)
- **ERP data:** part of the integration that brings customer data from SAP Business One and Sienge over SQS, and the CDC feed of the budget planning module

**Co-founder of Tocket**, escrow for university tickets (R$150,000 brokered by hand from 2022 to 2025):

- **WhatsApp agent:** since October 2026, a TypeScript agent on Eve with OpenAI's gpt-6-luna. Deal state lives in Postgres, and no personal data reaches the model
- **Response evals:** 53 cases against the real model, from single messages to full conversations with a scripted user, checking the reply, the summary shown before saving and the final database state, prompt injection included. They are how we set reasoning to low: same score, 36% fewer output tokens
- The repository is private

### Featured Projects

**Reinforcement Learning**

**[aps08-rl](https://github.com/gabrielmmh/aps08-rl)** - PPO generalization for coverage path planning under partial observability. Nine configurations; structured memory, frontier features and potential-based shaping took the 20×20 grid from 9% to 75% full coverage (96% of solvable maps), close to the scripted frontier ceiling
> Stable-Baselines3 | MaskablePPO | Gymnasium | curriculum learning

**RL for sepsis treatment in the ICU** - Six RL algorithms on the icu-sepsis MDP (716 states from MIMIC-III). Tabular PPO and Q-Learning reach ~85% survival against a 78% clinical baseline, and tabular beats deep within each family
> Python | Gymnasium | PyTorch | [Video](https://www.youtube.com/watch?v=mH0rtjRgbXU) (course repo is private)

**AI & Machine Learning**

**[news_summarizer](https://github.com/gabrielmmh/news_summarizer)** - Automated pipeline that scrapes news, generates AI summaries, and distributes via email
> Airflow | GPT-4o | PostgreSQL | Docker | MinIO

**[olist-medallion-pipeline](https://github.com/gabrielmmh/olist-medallion-pipeline)** - E-commerce data pipeline with Medallion Architecture (1.35M records)
> Prefect | RabbitMQ | PostgreSQL | Grafana | [Video Demo](https://www.youtube.com/watch?v=1vN0BAf2dYQ)

**[redes_neurais](https://github.com/gabrielmmh/redes_neurais)** - Neural Networks portfolio: Perceptrons, MLPs, VAEs, and generative models
> TensorFlow/Keras | Stable Diffusion | [Documentation Site](https://gabrielmmh.github.io/redes_neurais/)

**Cloud & Infrastructure**

**[proj_cloud](https://github.com/gabrielmmh/proj_cloud)** - AWS infrastructure with CloudFormation, Auto Scaling, and CI/CD pipeline
> AWS | ALB | EC2 | DynamoDB | CodePipeline | FastAPI | Locust

**Functional Programming**

**[PortfolioOptimizer](https://github.com/gabrielmmh/PortfolioOptimizer)** - Demonstrates that past-optimized portfolios have no predictive power for future returns
> F# | Statistical analysis of optimization overfitting

### Open Source

**[vercel/eve#1972](https://github.com/vercel/eve/issues/1972)** - While building on Eve at work, I found that Markdown-only dynamic skills opened a sandbox session they didn't need. The Eve team accepted it as an enhancement and shipped the fix in [#3669](https://github.com/vercel/eve/pull/3669) (September 2026): dynamic skills are now served from session state without touching the sandbox.

**[vercel/eve#1890](https://github.com/vercel/eve/issues/1890)** - I asked for MCP tool annotations to reach approval policies, so a policy can tell a read-only tool from a destructive one. Shipped in [#4596](https://github.com/vercel/eve/pull/4596) (October 2026).

### Tech Stack

**AI/LLMs:** Python, TypeScript, Eve, LangGraph, LangChain, Anthropic, OpenAI and Gemini APIs, MCP, RAG (pgvector, Neo4j), typed decisions (Jev, luna-decisions), evals and LLM-as-a-judge (Inspect AI), Langfuse, guardrails

**Backend:** TypeScript, Next.js, Node.js, FastAPI, NestJS, .NET

**Data:** PostgreSQL, BigQuery, Airflow, Prefect, ETL pipelines

**Cloud/DevOps:** AWS (Lambda, SQS, S3, SST), Terraform, Docker, GitHub Actions, Grafana, PostHog

---

<div align="center">
<sub>Professional work lives under my work account; this one holds personal and academic projects.</sub>
</div>
