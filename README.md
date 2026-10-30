<h1 align="center">Marcel Roozekrans</h1>

<p align="center">
  .NET engineer building <strong>ZeroAlloc.NET</strong>, compile-time .NET without reflection,<br>
  and <strong>AI libraries for .NET</strong>: agents, RAG, decisions and security. Based in Cruquius, the Netherlands.
</p>

<p align="center">
  <a href="https://roozekrans.nl"><img src="https://img.shields.io/badge/roozekrans.nl-0b1120?style=for-the-badge&logo=astro&logoColor=22d3ee" alt="Website"></a>
  <a href="https://zeroalloc.net"><img src="https://img.shields.io/badge/zeroalloc.net-0b1120?style=for-the-badge&logo=dotnet&logoColor=22d3ee" alt="ZeroAlloc.NET"></a>
  <a href="https://www.nuget.org/profiles/MarcelRoozekrans"><img src="https://img.shields.io/badge/NuGet-004880?style=for-the-badge&logo=nuget&logoColor=white" alt="NuGet"></a>
  <a href="https://www.linkedin.com/in/marcelroozekrans/"><img src="https://img.shields.io/badge/LinkedIn-0a66c2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="https://github.com/sponsors/MarcelRoozekrans"><img src="https://img.shields.io/badge/Sponsor-ea4aaa?style=for-the-badge&logo=githubsponsors&logoColor=white" alt="Sponsor"></a>
</p>

<p align="center">
  <strong>245+</strong> NuGet packages &nbsp;·&nbsp; <strong>2.8M+</strong> downloads
</p>

---

Two things get most of my time: moving .NET work from runtime to compile time, so it is fast, allocation-free and Native AOT safe, and giving AI agents in .NET the building blocks they are missing: a framework, retrieval, calibrated decisions, guardrails and real tools.

## ZeroAlloc.NET

A 100+ package ecosystem where every dispatch, registration, mapping and validation rule is wired at compile time by a Roslyn source generator — no reflection, no boxing, Native AOT safe throughout.

**[github.com/ZeroAlloc-Net](https://github.com/ZeroAlloc-Net)** · **[zeroalloc.net](https://zeroalloc.net)**

| Package | What it does |
|---|---|
| [**Mediator**](https://github.com/ZeroAlloc-Net/ZeroAlloc.Mediator) [![v](https://img.shields.io/nuget/v/ZeroAlloc.Mediator?style=flat-square&label=)](https://www.nuget.org/packages/ZeroAlloc.Mediator) | Dispatch resolved at compile time — no dictionaries, no virtual calls |
| [**ORM**](https://github.com/ZeroAlloc-Net/ZeroAlloc.ORM) [![v](https://img.shields.io/nuget/v/ZeroAlloc.ORM?style=flat-square&label=)](https://www.nuget.org/packages/ZeroAlloc.ORM) | Raw-SQL data access from `[Query]`/`[Command]` partial methods |
| [**Inject**](https://github.com/ZeroAlloc-Net/ZeroAlloc.Inject) [![v](https://img.shields.io/nuget/v/ZeroAlloc.Inject?style=flat-square&label=)](https://www.nuget.org/packages/ZeroAlloc.Inject) | Compile-time DI with a standalone AOT container |
| [**Analyzers**](https://github.com/ZeroAlloc-Net/ZeroAlloc.Analyzers) [![v](https://img.shields.io/nuget/v/ZeroAlloc.Analyzers?style=flat-square&label=)](https://www.nuget.org/packages/ZeroAlloc.Analyzers) | Flags allocations, boxing and virtual dispatch on hot paths |
| [**EventSourcing**](https://github.com/ZeroAlloc-Net/ZeroAlloc.EventSourcing) [![v](https://img.shields.io/nuget/v/ZeroAlloc.EventSourcing?style=flat-square&label=)](https://www.nuget.org/packages/ZeroAlloc.EventSourcing) | Event streams, projections and aggregates, generated |
| [**Templates**](https://github.com/ZeroAlloc-Net/ZeroAlloc.Templates) [![v](https://img.shields.io/nuget/v/ZeroAlloc.Templates?style=flat-square&label=)](https://www.nuget.org/packages/ZeroAlloc.Templates) | `dotnet new` Clean Architecture API wiring 12 of the libraries together |

<sub>Plus Rest, Saga, Outbox, Pipeline, Scheduling, Serialisation, StateMachine, Resilience, Validation, ValueObjects, Results, Collections, Mapping, Telemetry, Specification, Authorization, AsyncEvents, Cache, Notify, Flux, TestHelpers and more.</sub>

## AI for .NET

A family of libraries for building AI agents in .NET on Microsoft.Extensions.AI, several of them built on ZeroAlloc.

| Project | What it does |
|---|---|
| [**Thalos.NET**](https://github.com/MarcelRoozekrans/Thalos.NET) [![v](https://img.shields.io/nuget/v/Thalos.NET?style=flat-square&label=)](https://www.nuget.org/packages/Thalos.NET) | ZeroAlloc-native agent framework on Microsoft Agent Framework, with AI.Sentinel security and MCP tool sources |
| [**Rag.NET**](https://github.com/MarcelRoozekrans/Rag.NET) [![v](https://img.shields.io/nuget/v/Rag.NET?style=flat-square&label=)](https://www.nuget.org/packages/Rag.NET) | Modular RAG pipeline — 74 packages covering chunking, vector stores, rerankers, data providers, evaluation |
| [**Minos.NET**](https://github.com/MarcelRoozekrans/Minos.NET) [![★](https://img.shields.io/github/stars/MarcelRoozekrans/Minos.NET?style=flat-square&label=&logo=github)](https://github.com/MarcelRoozekrans/Minos.NET) | Unofficial client for TypeSafe's Jev decision models — typed questions in, calibrated probabilities out; source-generated, Native AOT safe |
| [**AI.Sentinel**](https://github.com/MarcelRoozekrans/AI.Sentinel) [![v](https://img.shields.io/nuget/v/AI.Sentinel?style=flat-square&label=)](https://www.nuget.org/packages/AI.Sentinel) | Security middleware for `IChatClient` — 56 detectors for the OWASP LLM Top 10 |
| [**Daedalus.NET**](https://github.com/MarcelRoozekrans/Daedalus.NET) | Reference application for Thalos.NET — AI task execution with Railway-Oriented Programming, Blazor and console front ends, orchestrated by Aspire |

### Tools for coding agents

MCP servers that give agents real understanding instead of a text search.

| Project | What it does |
|---|---|
| [**roslyn-codelens-mcp**](https://github.com/MarcelRoozekrans/roslyn-codelens-mcp) [![★](https://img.shields.io/github/stars/MarcelRoozekrans/roslyn-codelens-mcp?style=flat-square&label=&logo=github)](https://github.com/MarcelRoozekrans/roslyn-codelens-mcp) | 67 tools exposing Roslyn semantic analysis — call graphs, DI graphs, diagnostics, code fixes, refactoring, test intelligence |
| [**memorylens-mcp**](https://github.com/MarcelRoozekrans/memorylens-mcp) [![★](https://img.shields.io/github/stars/MarcelRoozekrans/memorylens-mcp?style=flat-square&label=&logo=github)](https://github.com/MarcelRoozekrans/memorylens-mcp) | .NET memory profiling — in-process heap snapshots, leak heuristics, actionable fix suggestions |
| [**LongtermMemory-MCP**](https://github.com/MarcelRoozekrans/LongtermMemory-MCP) [![v](https://img.shields.io/npm/v/longterm-memory-mcp?style=flat-square&label=&logo=npm)](https://www.npmjs.com/package/longterm-memory-mcp) | Persistent semantic memory, fully local — SQLite + a local transformer, no API keys |

<sub>More libraries, analyzers and tools: <a href="https://roozekrans.nl/projects">roozekrans.nl/projects</a>.</sub>

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
