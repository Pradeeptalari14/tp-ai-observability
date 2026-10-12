[![Ecosystem](https://img.shields.io/badge/Portfolio%20Ecosystem-341%20Studios-6366f1.svg)](https://pradeeptalari.me/projects/)
[![Architecture DAG](https://img.shields.io/badge/Architecture-DAG%20%26%20Course-10b981.svg)](https://pradeeptalari.me/tools/repo-learning/)

# AI Observability & Trace Studio

This repository contains the target configuration and SRE runtime files compiled by the **AI Observability & Trace Studio** dashboard module.

## 🚀 Description
Deploy trace instrumentation meshes. Generate Langfuse backend docker-compose structures, OpenTelemetry custom spans, and token budget alerts.

## 🛠️ Specification Matrix
- **Primary Configuration File**: `/deploy/observability/langfuse_otel.yaml`
- **Execution Command**: `kubectl apply -f langfuse_otel.yaml`
- **Validation Command**: `kubectl get pods -l app=langfuse`

## 📋 How to Run & Validate

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Pradeeptalari14/tp-ai-observability.git
   cd tp-ai-observability
   ```

2. **Run Execution Target:**
   ```bash
   kubectl apply -f langfuse_otel.yaml
   ```

3. **Verify Runtime Stability:**
   ```bash
   kubectl get pods -l app=langfuse
   ```

## 🔐 Security & Best Practices
* **Secret Isolation**: Use organization-level secrets (or SSM parameter hooks) rather than hardcoded environment variables inside files.
* **Pull Request Lifecycles**: Protect default branch merges with validation checks before merging code changes.

---
*Synchronized with [AI Observability & Trace Studio Studio](https://pradeeptalari.me/tools/ai-observability/) & [Repository Learning DAG](https://pradeeptalari.me/tools/repo-learning/) — [Talari Pradeep Portfolio](https://pradeeptalari.me)*
