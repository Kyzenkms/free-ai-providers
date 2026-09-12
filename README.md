<div align="center">

# ⚡ Curated Free & Trial AI API Providers
### High-Performance Reverse Proxies, Free Quota Relays, & Real-Time Model Diagnostics

[![Live Diagnostic Checker](https://img.shields.io/badge/Diagnostic_Suite-ai.solisk.org%2Fchecker-4f46e5?style=for-the-badge&logo=fastapi&logoColor=white)](https://ai.solisk.org/checker)
[![Verified Relays](https://img.shields.io/badge/Verified_Relays-16+_Endpoints-059669?style=for-the-badge&logo=statuspage&logoColor=white)](https://ai.solisk.org/)
[![Total Free Grant Pool](https://img.shields.io/badge/Free_Credit_Pool-$400%2B_Initial-d97706?style=for-the-badge&logo=circleci&logoColor=white)](https://ai.solisk.org/)
[![Protocols](https://img.shields.io/badge/Protocols-OpenAI_%7C_Anthropic-2563eb?style=for-the-badge&logo=openai&logoColor=white)](https://ai.solisk.org/)
[![PRs Welcome](https://img.shields.io/badge/PRs-Welcome-brightgreen?style=for-the-badge&logo=github)](https://github.com/Kyzenkms/free-ai-providers/pulls)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](LICENSE)

<p align="center">
  <b>An analytical benchmark and technical registry of free-tier AI API relays, token gateways, and community inference pools.</b><br>
  Engineered for autonomous coding agents, LLM evaluation pipelines, high-throughput fallbacks, and zero-cost prototyping.
</p>

[🌐 Web Directory](https://ai.solisk.org/) • [⚡ Live API Checker](https://ai.solisk.org/checker) • [📥 Submit New Relay](https://github.com/Kyzenkms/free-ai-providers/issues) • [🛠️ Client Recipes](#client-integration-recipes)

</div>

---

## 📑 Table of Contents
- [Executive Summary](#-analytical-executive-summary)
- [System Architecture & Uptime Advisory](#-system-architecture--uptime-advisory)
- [Provider Benchmark Matrix](#-provider-benchmark-matrix)
- [Comprehensive Provider Directory](#-comprehensive-provider-directory)
  - [S-Tier: High Initial Allocations](#s-tier--high-initial-allocations)
  - [A-Tier: Daily Quotas & Refreshing Credits](#a-tier--daily-quotas--refreshing-credits)
  - [B-Tier: Specialized & Secondary Endpoints](#b-tier--specialized--secondary-endpoints)
- [Client Integration Recipes](#-client-integration-recipes)
  - [Python (OpenAI SDK)](#1-python-openai-v1)
  - [Node.js / TypeScript](#2-nodejs--typescript-openai-sdk)
  - [cURL Command](#3-curl-cli-benchmark)
  - [OpenClaw Configuration](#4-openclaw-integration-openclawjson)
  - [OpenCode Configuration](#5-opencode-integration-opencodejson)
- [Live Diagnostic Suite](#-live-diagnostic-suite)
- [Contributing](#-contributing)

---

## 📊 Analytical Executive Summary

| Benchmark Metric | Aggregated Value | Technical Scope & Analysis |
|:---|:---|:---|
| **Cumulative Initial Credit Pool** | **`$470+ USD` equivalent** | Sum of unmetered starter grants across all verified endpoints |
| **Max Automated 24h Quota** | **`$45 / day`** | Daily automated credit refreshes (AgentRouter: `$25`, JustWoker: `$20`) |
| **Keyless / Public Bearer Relays** | **`2 Endpoints`** | Direct access via `public` Bearer key (OpenCode Zen) and Discord pools |
| **Frontier Model Coverage** | **DeepSeek R1/V3/V4, Claude 3.5/3.7, GPT-4o, GLM-4/5** | Reverse proxy tunnels upstreamed to official provider APIs |
| **Standardized Protocols** | **OpenAI (`/v1/chat/completions`) & Anthropic (`/v1/messages`)** | Universal drop-in compatibility across modern SDKs and agent harnesses |

> [!TIP]
> **Check providers quickly without hassle:** Ping endpoint latency, validate token authorization, inspect group model allocations, and auto-generate client JSON configurations directly in your browser at **[ai.solisk.org/checker](https://ai.solisk.org/checker)**.

---

## ⚠️ System Architecture & Uptime Advisory

> [!NOTE]
> **Third-Party Relay Dynamics:** The services cataloged in this repository operate as **third-party aggregators and upstream relays**. Because they pool, balance, and route traffic across shared upstream enterprise accounts, the following operational dynamics apply:
> 1. **Uptime & Latency Fluctuation:** Latency response times and connection stability may fluctuate during peak global usage hours.
> 2. **Dynamic Quota Allocations:** Free allowances and model routing permissions are governed autonomously by each relay operator.
> 3. **High-Availability Best Practice:** Never rely on a single relay for mission-critical production. Configure **multi-endpoint round-robin** or **cascading fallback lists** in your agent frameworks (e.g., OpenClaw, LiteLLM, or LangChain).

---

## 🧭 Provider Benchmark Matrix

| Provider | Base URL | Protocol | Free Quota | Daily Refresh | Key Type | Best Suited For | Diagnostic |
|:---|:---|:---|:---|:---|:---|:---|:---:|
| **SeekAI** | `https://seekai.cc/v1` | OpenAI | `$200` | None | API Key | Heavy inference, wide model range | [Test](https://ai.solisk.org/checker) |
| **HCNSEC** | `https://api.hcnsec.cn/v1` | OpenAI | Generous Pool | None | API Key | Fallback routing, agent loops | [Test](https://ai.solisk.org/checker) |
| **AgentRouter** | `https://agentrouter.org/v1` | OpenAI | `$50` | `$25` / 24h | API Key | Daily development, CI/CD runs | [Test](https://ai.solisk.org/checker) |
| **JustWoker** | `https://api.justwoker.icu/v1` | Anthropic + OpenAI | `$100` | `$20` / 24h | API Key | Claude coding agents & benchmarks | [Test](https://ai.solisk.org/checker) |
| **APIMaster** | `https://apimaster.ai/v1` | OpenAI | `$20` | None | API Key | Clean GPT-4o / frontier testing | [Test](https://ai.solisk.org/checker) |
| **TokenForge** | `https://tokenforge.ai.studio/v1` | OpenAI | `$90` | 2×/day pool | API Key | Scheduled batch tasks | [Test](https://ai.solisk.org/checker) |
| **OpenCode Zen** | `https://opencode.ai/zen/v1` | OpenAI | Free Tier | Continuous | `public` | DeepSeek V4 Flash, MiMo V2.5 | [Test](https://ai.solisk.org/checker) |
| **Orbelius** | `https://nova.vcrauo.com/v1` | OpenAI | `$10` | Claimable | API Key | Testing relays & dashboard rewards | [Test](https://ai.solisk.org/checker) |
| **VSLLM** | `https://vsllm.cc/v1` | OpenAI | `¥0.5` | Subscription | API Key | Secondary low-latency failover | [Test](https://ai.solisk.org/checker) |
| **GetUniKey** | `https://api.getunikey.ai/v1` | OpenAI | 5,000 Credits | None | API Key | Image generation models | [Test](https://ai.solisk.org/checker) |
| **Yingz Bot** | Telegram Relay | Custom | 10M Tokens | Referral | Custom | Lightweight bot automation | [Test](https://ai.solisk.org/checker) |

---

## 📦 Comprehensive Provider Directory

### S-Tier — High Initial Allocations

#### 1. SeekAI
* **Base URL:** `https://seekai.cc/v1`
* **Protocol:** OpenAI Compatible (`/v1/chat/completions`)
* **Registration:** [seekai.cc/sign-up?aff=8lEz](https://seekai.cc/sign-up?aff=8lEz)
* **Allocation:** `$200` initial grant upon account activation.
* **Technical Notes:** Features comprehensive catalog of frontier LLMs with low-jitter streaming responses.

#### 2. HCNSEC
* **Base URL:** `https://api.hcnsec.cn/v1`
* **Protocol:** OpenAI Compatible (`/v1/chat/completions`)
* **Registration:** [api.hcnsec.cn/sign-up?aff=9A6V](https://api.hcnsec.cn/sign-up?aff=9A6V)
* **Allocation:** Generous default free credit pool.
* **Technical Notes:** High-throughput reverse gateway well-suited for autonomous agents and resilient fallback tiers.

---

### A-Tier — Daily Quotas & Refreshing Credits

#### 3. AgentRouter
* **Base URL:** `https://agentrouter.org/v1`
* **Protocol:** OpenAI Compatible (`/v1/chat/completions`)
* **Registration:** [agentrouter.org/register?aff=9tAF](https://agentrouter.org/register?aff=9tAF)
* **Allocation:** `$50` starting balance + automated `$25` daily quota refresh.
* **Technical Notes:** Highest sustained free quota available. Frontier model access included across major foundation model families.

#### 4. JustWoker
* **Base URL:** `https://api.justwoker.icu/v1`
* **Protocol:** Native Anthropic (`/v1/messages`) & OpenAI Compatible (`/v1/chat/completions`)
* **Registration:** [api.justwoker.icu/register?aff=OBJZ](https://api.justwoker.icu/register?aff=OBJZ)
* **Allocation:** `$100` starting grant + automated `$20` daily quota refresh.
* **Technical Notes:** Dual-protocol support allows direct integration into Claude-native toolkits and OpenAI-compatible clients alike.

#### 5. APIMaster
* **Base URL:** `https://apimaster.ai/v1`
* **Protocol:** OpenAI Compatible (`/v1/chat/completions`)
* **Registration:** [apimaster.ai/register?ref=atpht1pq](https://apimaster.ai/register?ref=atpht1pq)
* **Allocation:** `$20` trial credit allowance.
* **Technical Notes:** High-fidelity OpenAI model routing with predictable response serialization.

#### 6. TokenForge
* **Base URL:** `https://tokenforge.ai.studio/v1`
* **Protocol:** OpenAI Compatible (`/v1/chat/completions`)
* **Registration:** [tokenforge.ai.studio/sign-up?aff=tkjh](https://tokenforge.ai.studio/sign-up?aff=tkjh)
* **Allocation:** `$90` credit allowance via direct registration link.
* **Technical Notes:** Free tier community pool opens **2× daily for limited hours** (announcements delivered via their official Discord).

---

### B-Tier — Specialized & Secondary Endpoints

#### 7. OpenCode Zen
* **Base URL:** `https://opencode.ai/zen/v1`
* **Protocol:** OpenAI Compatible (`/v1/chat/completions`)
* **API Key:** `public` (Accepts bearer token `public` for free tier models)
* **Website:** [opencode.ai](https://opencode.ai)
* **Supported Models:** `deepseek-v4-flash-free`, `mimo-v2.5-free`, `big-pickle`, `nemotron-3-ultra-free`, `north-mini-code-free`
* **Technical Notes:** Zero-signup gateway provided by OpenCode. Requires setting `User-Agent: opencode/1.18.18`.

#### 8. Orbelius
* **Base URL:** `https://nova.vcrauo.com/v1`
* **Protocol:** OpenAI Compatible
* **Registration:** [nova.vcrauo.com/sign-up?aff=7Ny4](https://nova.vcrauo.com/sign-up?aff=7Ny4)
* **Allocation:** `$10` starting trial balance.
* **Technical Notes:** Claimable reward credits available periodically — inspect account dashboard for active reward campaigns.

#### 9. VSLLM
* **Base URL:** `https://vsllm.cc/v1`
* **Protocol:** OpenAI Compatible
* **Registration:** [vsllm.cc/register?aff=sTmW](https://vsllm.cc/register?aff=sTmW)
* **Allocation:** Subscription model with `¥0.5` trial credit.
* **Technical Notes:** Fast token generation speeds; effective as a secondary failover relay.

#### 10. GetUniKey
* **Base URL:** `https://api.getunikey.ai/v1`
* **Protocol:** OpenAI Compatible
* **Registration:** [getunikey.ai/sign-up?aff=8GN5](https://www.getunikey.ai/sign-up?aff=8GN5)
* **Allocation:** 5,000 credit allocation.
* **Technical Notes:** Recommended primarily for image generation models. Credits deplete rapidly when consumed by large context frontier LLMs.

#### 11. WorkBuddy
* **Platform:** CLI, IDE, and Work Agent
* **Website:** [workbuddy.ai](https://www.workbuddy.ai/)
* **Allocation:** Free registration tier.
* **Technical Notes:** Autonomous developer productivity suite functioning as a CLI, IDE, and workflow agent with integrated model access.

#### 12. Yingz Bot
* **Platform:** Telegram Bot Relay
* **Access Link:** [t.me/Yingzshopbot?start=ref7712622794](https://t.me/Yingzshopbot?start=ref7712622794)
* **Allocation:** 10,000,000 token grant (+ 10M per referral).
* **Technical Notes:** Programmatic API relay managed through Telegram.

#### 13. TokenRouter
* **Base URL:** `https://www.tokenrouter.com/v1`
* **Protocol:** OpenAI Compatible
* **Registration:** [tokenrouter.com](https://www.tokenrouter.com/)
* **Technical Notes:** Aggregator endpoint routing across multiple underlying models.

#### 14. QianXing
* **Base URL:** `https://fast.qianxing.pro/v1`
* **Protocol:** OpenAI Compatible
* **Registration:** [fast.qianxing.pro/sign-up?aff=IoIBndmu](https://fast.qianxing.pro/sign-up?aff=IoIBndmu)
* **Allocation:** Free trial quota.

#### 15. EMTF
* **Base URL:** `https://emtf.aipm9527.online/v1`
* **Protocol:** OpenAI Compatible
* **Registration:** [emtf.aipm9527.online/sign-up?aff=3wdE](https://emtf.aipm9527.online/sign-up?aff=3wdE)
* **Allocation:** Free registration allowance.

#### 16. SynteroLink
* **Registration:** [synterolink.com/register?aff=ET5P738DGDPV](https://synterolink.com/register?aff=ET5P738DGDPV)
* **Technical Notes:** Subscription-based service offering referral rewards.

---

## 🛠️ Client Integration Recipes

### 1. Python (OpenAI v1+)
```python
from openai import OpenAI

client = OpenAI(
    base_url="https://seekai.cc/v1",  # Replace with target relay Base URL
    api_key="sk-your-api-key"          # Use 'public' for OpenCode Zen
)

response = client.chat.completions.create(
    model="gpt-4o",
    messages=[{"role": "user", "content": "Explain consensus algorithms in distributed systems."}],
    temperature=0.7
)

print(response.choices[0].message.content)
```

### 2. Node.js / TypeScript (OpenAI SDK)
```typescript
import OpenAI from "openai";

const openai = new OpenAI({
  baseURL: "https://agentrouter.org/v1",
  apiKey: "sk-your-api-key",
});

async function main() {
  const completion = await openai.chat.completions.create({
    model: "claude-3-5-sonnet-20241022",
    messages: [{ role: "user", content: "Write a high-performance LRU cache in Rust." }],
  });
  console.log(completion.choices[0].message.content);
}

main();
```

### 3. cURL CLI Benchmark
```bash
curl https://seekai.cc/v1/chat/completions \
  -H "Content-Type: application/json" \
  -H "Authorization: Bearer sk-your-api-key" \
  -d '{
    "model": "deepseek-chat",
    "messages": [{"role": "user", "content": "Hello world"}]
  }'
```

### 4. OpenClaw Integration (`openclaw.json`)
Add under `models.providers`:
```json
{
  "seekai-relay": {
    "api": "openai-completions",
    "baseUrl": "https://seekai.cc/v1",
    "apiKey": "sk-your-api-key",
    "headers": {
      "User-Agent": "Mozilla/5.0"
    },
    "models": [
      {
        "id": "gpt-4o",
        "name": "GPT-4o (SeekAI)",
        "contextWindow": 128000,
        "maxTokens": 8192
      }
    ]
  }
}
```

### 5. OpenCode Integration (`opencode.json`)
Add under `providers`:
```json
{
  "agentrouter": {
    "npm": "@ai-sdk/openai-compatible",
    "options": {
      "baseURL": "https://agentrouter.org/v1",
      "apiKey": "sk-your-api-key"
    },
    "models": [
      {
        "id": "deepseek-v4-flash",
        "name": "DeepSeek V4 Flash",
        "contextLength": 128000
      }
    ]
  }
}
```

---

## ⚡ Live Diagnostic Suite

Validate credentials, ping latency, scan assigned group models, and generate client configurations directly in your browser:

👉 **[ai.solisk.org/checker](https://ai.solisk.org/checker)**

* No registration or software installation required.
* Tests endpoints securely and outputs client configs for OpenClaw and OpenCode.

---

## 🤝 Contributing

Contributions to update quota allocations, report deprecated endpoints, or add newly launched free-tier relays are welcome!

1. Fork this repository.
2. Verify the relay endpoint via `ai.solisk.org/checker` or local cURL.
3. Update `README.md` and submit a Pull Request.

---

<div align="center">
  <sub>Maintained with ❤️ for the open-source AI developer community. Star ⭐ this repo if you find it helpful!</sub>
</div>
