# HeroBrain Documentation
## Memory-as-a-Service for AI Applications

Welcome to the HeroBrain documentation! This is the source for `docs.herobrain.dev`.

---

## 📚 Documentation Structure

### [Getting Started](./getting-started/)
New to HeroBrain? Start here.
- **Quickstart** - Get up and running in 5 minutes
- **Installation** - SDK installation for TypeScript and Python
- **Authentication** - API key setup and security
- **First API Call** - Store and search your first memory

### [Core Concepts](./core-concepts/)
Understand how HeroBrain works.
- **Memory Types** - 13 cognitive memory types explained
- **Semantic Search** - How hybrid search works
- **Intelligence Layer** - Automatic pattern detection and learning
- **Multi-Tenant Architecture** - Isolation and security
- **Storage & Performance** - PostgreSQL, Qdrant, Redis architecture

### [Guides](./guides/)
Step-by-step tutorials for common tasks.
- **Storing Memories** - Best practices for memory creation
- **Searching Memories** - Query optimization and filters
- **Webhooks** - Real-time event notifications
- **OAuth Integrations** - Connect Gmail, Calendar, Slack, etc.
- **Importance Prediction** - Understanding the scoring system
- **Behavioral Learning** - How the system adapts to users
- **Batch Operations** - Efficient bulk imports

### [API Reference](./api-reference/)
Complete API documentation.
- **REST API** - All endpoints with examples
- **TypeScript SDK** - Node.js library reference
- **Python SDK** - Python library reference
- **GraphQL API** - GraphQL schema and queries (coming soon)
- **Rate Limits** - Quotas and best practices
- **Error Codes** - Complete error reference

### [Examples](./examples/)
Real-world applications and code samples.
- **AI Assistant** - Memory-powered chatbot
- **Meeting Notes** - Intelligence extraction from transcripts
- **Knowledge Base** - Semantic search over documents
- **Customer Support** - Context-aware support bot
- **More Examples** - Community-contributed examples

### [Resources](./resources/)
Additional resources and help.
- **FAQ** - Frequently asked questions
- **Troubleshooting** - Common issues and solutions
- **Best Practices** - Performance and security tips
- **Migration Guide** - Moving from other solutions
- **Changelog** - Product updates and releases
- **Status** - System status and uptime

---

## 🚀 Quick Links

- **Website:** [herobrain.dev](https://herobrain.dev)
- **Dashboard:** [app.herobrain.dev](https://app.herobrain.dev)
- **API Base URL:** `https://api.herobrain.dev`
- **GitHub:** [github.com/herobrain](https://github.com/herobrain)
- **Discord:** [discord.gg/herobrain](#)
- **Twitter:** [@herobrainapi](#)

---

## 📝 Contributing to Documentation

Found an error or want to improve the docs? We welcome contributions!

1. Fork the repository
2. Make your changes
3. Submit a pull request

**Style guide:**
- Use clear, concise language
- Include code examples that actually work
- Test all code snippets before submitting
- Follow the existing structure

---

## 🛠️ Documentation Setup

This documentation is designed to work with **Mintlify** or **Docusaurus**.

### For Mintlify:

```bash
# Install Mintlify CLI
npm i -g mintlify

# Run locally
cd docs-production
mintlify dev
```

### For Docusaurus:

```bash
# Install Docusaurus
npx create-docusaurus@latest docs-site classic

# Copy docs to docusaurus/docs/
cp -r docs-production/* docs-site/docs/

# Run locally
cd docs-site
npm start
```

---

## 📂 Folder Structure

```
docs-production/
├── README.md                    # This file
├── getting-started/
│   ├── quickstart.md
│   ├── installation.md
│   ├── authentication.md
│   └── first-api-call.md
├── core-concepts/
│   ├── memory-types.md
│   ├── semantic-search.md
│   ├── intelligence-layer.md
│   ├── multi-tenant.md
│   └── architecture.md
├── guides/
│   ├── storing-memories.md
│   ├── searching-memories.md
│   ├── webhooks.md
│   ├── oauth-integrations.md
│   ├── importance-prediction.md
│   ├── behavioral-learning.md
│   └── batch-operations.md
├── api-reference/
│   ├── rest-api.md
│   ├── typescript-sdk.md
│   ├── python-sdk.md
│   ├── rate-limits.md
│   └── error-codes.md
├── examples/
│   ├── ai-assistant.md
│   ├── meeting-notes.md
│   ├── knowledge-base.md
│   └── customer-support.md
└── resources/
    ├── faq.md
    ├── troubleshooting.md
    ├── best-practices.md
    ├── migration-guide.md
    ├── changelog.md
    └── status.md
```

---

## 📖 Writing Guidelines

### Code Examples

Always include working code examples:

```typescript
// ✅ Good - Complete, working example
import { HeroBrain } from '@herobrain/sdk';

const client = new HeroBrain({ apiKey: process.env.HEROBRAIN_API_KEY });

const memory = await client.memories.create({
  type: 'episodic',
  content: 'Example content',
  tenantId: 'user_123'
});
```

```typescript
// ❌ Bad - Incomplete, assumes context
const memory = await create({
  content: 'Example'
});
```

### Headers and Structure

Use clear hierarchy:

```markdown
# Page Title (H1 - only one per page)

Brief introduction to the topic.

## Main Section (H2)

Content here.

### Subsection (H3)

Content here.

#### Detail (H4)

Content here.
```

### Links

Use relative links for internal docs:

```markdown
<!-- ✅ Good -->
See [Memory Types](../core-concepts/memory-types.md) for details.

<!-- ❌ Bad -->
See [Memory Types](https://docs.herobrain.dev/core-concepts/memory-types) for details.
```

---

## 📊 Documentation Status

| Section | Status | Progress |
|---------|--------|----------|
| Getting Started | 🟡 In Progress | 75% |
| Core Concepts | 🟢 Complete | 100% |
| Guides | 🟡 In Progress | 50% |
| API Reference | 🔴 Planned | 0% |
| Examples | 🟡 In Progress | 40% |
| Resources | 🔴 Planned | 20% |

**Legend:**
- 🟢 Complete - Ready for production
- 🟡 In Progress - Being written
- 🔴 Planned - Not started yet

---

## 🎯 Documentation Goals

1. **Comprehensive** - Cover every feature and use case
2. **Clear** - Easy to understand for all skill levels
3. **Accurate** - All code examples work and are tested
4. **Up-to-date** - Keep in sync with API changes
5. **Searchable** - Good SEO and site search
6. **Beautiful** - Professional design and formatting

---

## 📅 Last Updated

**Date:** 2025-10-25
**Version:** 1.0.0
**API Version:** v1

---

**Questions?** Join our [Discord](https://discord.gg/herobrain) or email docs@herobrain.dev
