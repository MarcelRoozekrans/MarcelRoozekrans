<h1 align="center">Marcel Roozekrans</h1>

<p align="center">
  Software engineer in the .NET ecosystem — source generators, async libraries,<br>
  and AI/MCP infrastructure. Based in Cruquius, the Netherlands.
</p>

<p align="center">
  <a href="https://roozekrans.nl"><img src="https://img.shields.io/badge/roozekrans.nl-0b1120?style=for-the-badge&logo=astro&logoColor=22d3ee" alt="Website"></a>
  <a href="https://www.nuget.org/profiles/MarcelRoozekrans"><img src="https://img.shields.io/badge/NuGet-004880?style=for-the-badge&logo=nuget&logoColor=white" alt="NuGet"></a>
  <a href="https://www.linkedin.com/in/marcelroozekrans/"><img src="https://img.shields.io/badge/LinkedIn-0a66c2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="https://github.com/sponsors/MarcelRoozekrans"><img src="https://img.shields.io/badge/Sponsor-ea4aaa?style=for-the-badge&logo=githubsponsors&logoColor=white" alt="Sponsor"></a>
</p>

<p align="center">
  <strong>210+</strong> NuGet packages &nbsp;·&nbsp; <strong>840K+</strong> downloads &nbsp;·&nbsp; <strong>5</strong> MCP servers
</p>

---

I build tools that make other developers faster: compile-time code generation instead of runtime reflection, async-first abstractions over APIs that never got them, and infrastructure that gives AI agents real understanding of a codebase instead of a text search over it.

## ZeroAlloc.NET

A 96-package ecosystem where every dispatch, registration, mapping and validation rule is wired at compile time by a Roslyn source generator — no reflection, no boxing, Native AOT safe throughout.

**[github.com/ZeroAlloc-Net](https://github.com/ZeroAlloc-Net)** · **[zeroalloc.net](https://zeroalloc.net)**

| Package | What it does |
|---|---|
| [**Mediator**](https://github.com/ZeroAlloc-Net/ZeroAlloc.Mediator) [![v](https://img.shields.io/nuget/v/ZeroAlloc.Mediator?style=flat-square&label=)](https://www.nuget.org/packages/ZeroAlloc.Mediator) | Dispatch resolved at compile time — no dictionaries, no virtual calls |
| [**ORM**](https://github.com/ZeroAlloc-Net/ZeroAlloc.ORM) [![v](https://img.shields.io/nuget/v/ZeroAlloc.ORM?style=flat-square&label=)](https://www.nuget.org/packages/ZeroAlloc.ORM) | Raw-SQL data access from `[Query]`/`[Command]` partial methods |
| [**Inject**](https://github.com/ZeroAlloc-Net/ZeroAlloc.Inject) [![v](https://img.shields.io/nuget/v/ZeroAlloc.Inject?style=flat-square&label=)](https://www.nuget.org/packages/ZeroAlloc.Inject) | Compile-time DI with a standalone AOT container |
| [**Analyzers**](https://github.com/ZeroAlloc-Net/ZeroAlloc.Analyzers) [![v](https://img.shields.io/nuget/v/ZeroAlloc.Analyzers?style=flat-square&label=)](https://www.nuget.org/packages/ZeroAlloc.Analyzers) | Flags allocations, boxing and virtual dispatch on hot paths |
| [**EventSourcing**](https://github.com/ZeroAlloc-Net/ZeroAlloc.EventSourcing) [![v](https://img.shields.io/nuget/v/ZeroAlloc.EventSourcing?style=flat-square&label=)](https://www.nuget.org/packages/ZeroAlloc.EventSourcing) | Event streams, projections and aggregates, generated |
| [**Templates**](https://github.com/ZeroAlloc-Net/ZeroAlloc.Templates) [![v](https://img.shields.io/nuget/v/ZeroAlloc.Templates?style=flat-square&label=)](https://www.nuget.org/packages/ZeroAlloc.Templates) | `dotnet new` Clean Architecture API wiring 10 of the packages together |

<sub>Plus Rest, Saga, Outbox, Pipeline, Scheduling, Serialisation, StateMachine, Resilience, Validation, ValueObjects, Results, Collections, Mapping, Telemetry, Specification, Authorization, AsyncEvents, Cache, Notify, Flux, TestHelpers and more.</sub>

## AI & MCP infrastructure

Giving coding agents real tools instead of guesswork.

| Project | What it does |
|---|---|
| [**roslyn-codelens-mcp**](https://github.com/MarcelRoozekrans/roslyn-codelens-mcp) [![★](https://img.shields.io/github/stars/MarcelRoozekrans/roslyn-codelens-mcp?style=flat-square&label=&logo=github)](https://github.com/MarcelRoozekrans/roslyn-codelens-mcp) | 67 tools exposing Roslyn semantic analysis to AI agents — call graphs, DI graphs, diagnostics, code fixes, refactoring, test intelligence |
| [**memorylens-mcp**](https://github.com/MarcelRoozekrans/memorylens-mcp) [![★](https://img.shields.io/github/stars/MarcelRoozekrans/memorylens-mcp?style=flat-square&label=&logo=github)](https://github.com/MarcelRoozekrans/memorylens-mcp) | .NET memory profiling — in-process heap snapshots, leak heuristics, actionable fix suggestions |
| [**AI.Sentinel**](https://github.com/MarcelRoozekrans/AI.Sentinel) [![v](https://img.shields.io/nuget/v/AI.Sentinel?style=flat-square&label=)](https://www.nuget.org/packages/AI.Sentinel) | Security middleware for `IChatClient` — 55 detectors for the OWASP LLM Top 10 |
| [**LongtermMemory-MCP**](https://github.com/MarcelRoozekrans/LongtermMemory-MCP) [![v](https://img.shields.io/npm/v/longterm-memory-mcp?style=flat-square&label=&logo=npm)](https://www.npmjs.com/package/longterm-memory-mcp) | Persistent semantic memory, fully local — SQLite + a local transformer, no API keys |
| [**Thalos.NET**](https://github.com/MarcelRoozekrans/Thalos.NET) [![v](https://img.shields.io/nuget/v/Thalos.NET?style=flat-square&label=)](https://www.nuget.org/packages/Thalos.NET) | ZeroAlloc-native agent framework on Microsoft Agent Framework, with AI.Sentinel security and MCP tool sources |
| [**Rag.NET**](https://github.com/MarcelRoozekrans/Rag.NET) [![v](https://img.shields.io/nuget/v/Rag.NET?style=flat-square&label=)](https://www.nuget.org/packages/Rag.NET) | Modular RAG pipeline on Microsoft.Extensions.AI — 41 packages covering chunking, vector stores, rerankers, data providers, evaluation |
| [**Copilot-Skill-Bridge**](https://github.com/MarcelRoozekrans/Copilot-Skill-Bridge) | Brings Claude Code marketplace skills into GitHub Copilot |
| [**superpowers-extensions**](https://github.com/MarcelRoozekrans/superpowers-extensions) | Regression testing, pre-push review and refactor analysis skills for Claude Code |
| [**lucent-code**](https://github.com/lucent-org/lucent-code) | AI chat & completions for VS Code, driven by the language server |

## Libraries & analyzers

| Project | What it does |
|---|---|
| [**AdoNet.Async**](https://github.com/MarcelRoozekrans/AdoNet.Async) [![v](https://img.shields.io/nuget/v/AdoNet.Async?style=flat-square&label=)](https://www.nuget.org/packages/AdoNet.Async) | Async-first ADO.NET — `await foreach` over rows, typed DataSets generated from XSD |
| [**Owasp.Analyzers**](https://github.com/MarcelRoozekrans/Owasp.Analyzers) [![v](https://img.shields.io/nuget/v/Owasp.Analyzers?style=flat-square&label=)](https://www.nuget.org/packages/Owasp.Analyzers) | OWASP Top 10 2025 as Roslyn rules, with taint analysis for SSRF |
| [**MailPeek**](https://github.com/MarcelRoozekrans/MailPeek) [![v](https://img.shields.io/nuget/v/MailPeek?style=flat-square&label=)](https://www.nuget.org/packages/MailPeek) | In-memory fake SMTP server with a live dashboard for ASP.NET Core |
| [**BlazorNative**](https://github.com/MarcelRoozekrans/BlazorNative) [![v](https://img.shields.io/nuget/v/BlazorNative.Core?style=flat-square&label=)](https://www.nuget.org/packages/BlazorNative.Core) | Blazor components as native mobile widgets via NativeAOT — no WebView |
| [**SSH.NET.Fork.Abstractions**](https://github.com/MarcelRoozekrans/SSH.NET.Fork.Abstractions) | Testable interface abstractions over SSH.NET |
| [**System.Reflection.Abstractions**](https://github.com/MarcelRoozekrans/System.Reflection.Abstractions) | Mockable wrappers around the reflection API |

## Elsewhere

[**Unearth**](https://github.com/MarcelRoozekrans/Unearth) — a read-only data-recovery and disk-forensics toolkit in pure Rust. Filesystem-aware undelete across FAT, exFAT, NTFS, ext2/3/4 and HFS+, signature carving of 150+ formats, lost-partition recovery — drivable from the shell or by an agent over MCP.

## GitHub activity

<p align="center">
  <img height="380" alt="GitHub stats" src="https://ghstats.dev/api/card?username=MarcelRoozekrans&amp;hide=followers,issues&amp;border_radius=8&amp;bg=0b1120&amp;text=cbd5e1&amp;title_color=22d3ee&amp;icon_color=22d3ee&amp;border_color=1e293b">
  <img height="380" alt="Most used languages" src="https://ghstats.dev/api/langs?username=MarcelRoozekrans&amp;layout=donut_vertical&amp;max_langs=8&amp;border_radius=8&amp;bg=0b1120&amp;text=cbd5e1&amp;title_color=22d3ee&amp;icon_color=22d3ee&amp;border_color=1e293b">
</p>

<p align="center">
  <sub>Cards by <a href="https://ghstats.dev">ghstats.dev</a> — regenerated on every page load.</sub>
</p>

## Sponsor

If my open source work saves you time, consider sponsoring to help me keep maintaining and building more.

**What sponsorship funds:**

- Continued maintenance of the ZeroAlloc.NET packages
- New features and .NET version upgrades across all projects
- More MCP servers and AI tooling for .NET developers
- Time I can spend on OSS instead of client work

<p align="center">
  <a href="https://github.com/sponsors/MarcelRoozekrans"><img src="https://img.shields.io/badge/%E2%9D%A4%20Become%20a%20sponsor-ea4aaa?style=for-the-badge&logo=githubsponsors&logoColor=white" alt="Become a sponsor"></a>
</p>
