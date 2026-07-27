# P11_RedactionModule


# Enterprise AI Security Gateway - PII Detection & Redaction Module

[![Python 3.10+](https://img.shields.io/badge/Python-3.10%2B-blue.svg)](https://www.python.org/)
[![LangChain v1](https://img.shields.io/badge/LangChain-v1-green.svg)](https://python.langchain.com/)
[![LiteLLM](https://img.shields.io/badge/LiteLLM-Proxy-orange.svg)](https://www.litellm.ai/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

An enterprise-grade security middleware and guardrail system designed to protect sensitive data and enforce compliance before prompts reach external Large Language Models (LLMs).

This gateway intercepts incoming user queries in real-time, inspects payloads for **Personally Identifiable Information (PII)** and **Adversarial Prompt Injections**, redacts high-risk data on the fly, and logs operational metrics.

---

## 📌 Key Features

* 🛡️ **Real-Time PII Detection & Redaction:** Automatically masks sensitive identifiers including Emails, Phone numbers, PAN numbers, Aadhaar numbers, and custom enterprise data formats using pre-execution input callbacks.
* 🚨 **Prompt Injection & Jailbreak Defense:** Intercepts hostile inputs, DAN jailbreak patterns, and prompt override instructions before they reach the model.
* 🔀 **Unified Gateway Proxy:** Abstract multiple model providers (OpenAI, Groq, Anthropic, Ollama) behind a single secure interface powered by `LiteLLM`.
* 📊 **Token & Cost Observability:** Captures input/output token counts, execution latency, and security audit logs without compromising data privacy.

---

## 🏗️ Architecture & Control Flow
