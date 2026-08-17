# Awesome AI Testing with stars

> A curated list of AI-powered testing tools, frameworks, and resources for QA engineers.

AI is reshaping software testing. This list collects tools, platforms, and resources that use AI or LLMs to generate tests, heal broken locators, triage failures, write assertions in natural language, and more. Both open source and commercial offerings are included, marked with badges so you can filter by what fits your stack.

## Contents

* [Legend](#legend)
* [Test Generation](#test-generation)
* [MCP-Based Testing](#mcp-based-testing)
* [Self-Healing Test Frameworks](#self-healing-test-frameworks)
* [AI-Powered E2E Platforms](#ai-powered-e2e-platforms)
* [Mobile AI Testing](#mobile-ai-testing)
* [Visual AI Testing](#visual-ai-testing)
* [Natural Language Test Authoring](#natural-language-test-authoring)
* [LLM-as-Judge Evaluation](#llm-as-judge-evaluation)
* [Test Analytics and Triage](#test-analytics-and-triage)
* [Code Coverage with AI](#code-coverage-with-ai)
* [AI Test Data Generation](#ai-test-data-generation)
* [Mock and Service Virtualization](#mock-and-service-virtualization)
* [Performance Testing with AI](#performance-testing-with-ai)
* [AI for Accessibility Testing](#ai-for-accessibility-testing)
* [API Testing with AI](#api-testing-with-ai)
* [LLM and AI System Testing](#llm-and-ai-system-testing)
* [Browser Automation for AI Agents](#browser-automation-for-ai-agents)
* [Articles and Talks](#articles-and-talks)
* [Courses and Tutorials](#courses-and-tutorials)
* [Newsletters and Communities](#newsletters-and-communities)
* [Benchmarks and Datasets](#benchmarks-and-datasets)
* [Related Awesome Lists](#related-awesome-lists)

## Legend

* 🆓 Open source
* 💰 Commercial
* 🆓💰 Open core (free tier or open source with paid features)

## Test Generation

Tools that generate test cases from code, requirements, or user behavior using AI.

* [Qodo-Cover](https://github.com/qodo-ai/qodo-cover) ⭐ 5,611 | 🐛 37 | 🌐 Python | 📅 2026-04-05 🆓 - AI-powered tool for automated test generation and code coverage enhancement.
* [Pynguin](https://github.com/se2p/pynguin) ⭐ 1,384 | 🐛 9 | 🌐 Python | 📅 2026-07-30 🆓 - Automated unit test generation for Python via evolutionary algorithms, from Saarland University.
* [EvoSuite](https://github.com/EvoSuite/evosuite) ⭐ 918 | 🐛 165 | 🌐 Java | 📅 2025-02-14 🆓 - Generates JUnit tests using evolutionary and genetic search-based algorithms for Java.
* [EvoMaster](https://github.com/EMResearch/EvoMaster) ⭐ 772 | 🐛 46 | 🌐 Kotlin | 📅 2026-08-17 🆓 - First open source AI tool that automatically generates test cases via evolutionary algorithms for REST, GraphQL, and RPC APIs.
* [Symflower](https://symflower.com/) 💰 - Commercial tool that combines symbolic execution, static analysis, and LLMs to generate unit tests for Java, Go, and Kotlin. Free CLI available with limitations.
* [CodiumAI / Qodo](https://www.qodo.ai/) 💰 - AI assistant generating meaningful tests from code context.
* [Diffblue Cover](https://www.diffblue.com/) 💰 - Autonomous Java unit test writer using reinforcement learning.
* [GitHub Copilot](https://github.com/features/copilot) 💰 - AI pair programmer that generates test code in Playwright, Cypress, Selenium across editors.
* [Cursor](https://www.cursor.com/) 💰 - AI-first code editor with strong test generation capabilities for major frameworks.
* [Claude Code](https://www.anthropic.com/claude-code) 💰 - Anthropic's terminal-based agentic coding assistant, useful for test suite generation and refactoring.

## MCP-Based Testing

Tools and servers that use the Model Context Protocol to give AI agents browser control and testing capabilities.

* [Chrome DevTools MCP](https://github.com/ChromeDevTools/chrome-devtools-mcp) ⭐ 49,305 | 🐛 112 | 🌐 TypeScript | 📅 2026-08-17 🆓 - Official MCP server from the Chrome DevTools team, with 26 tools for browser automation, debugging, and performance analysis.
* [Playwright MCP](https://github.com/microsoft/playwright-mcp) ⭐ 36,211 | 🐛 6 | 🌐 TypeScript | 📅 2026-08-12 🆓 - Official Playwright MCP server giving AI agents full browser control through structured accessibility snapshots.
* [Playwright CLI](https://github.com/microsoft/playwright-cli) ⭐ 12,586 | 🐛 2 | 🌐 JavaScript | 📅 2026-08-13 🆓 - Token-efficient CLI for coding agents like Claude Code and GitHub Copilot, with installable skills.
* [BrowserTools MCP](https://github.com/AgentDeskAI/browser-tools-mcp) ⭐ 7,293 | 🐛 1 | 🌐 TypeScript | 📅 2026-08-12 🆓 - Browser monitoring and console log access for AI agents via Chrome extension.
* [Browser MCP](https://github.com/browsermcp/mcp) ⭐ 6,978 | 🐛 147 | 🌐 TypeScript | 📅 2025-04-24 🆓 - Popular MCP server that automates the user's own local browser, preserving logged-in sessions and avoiding bot detection. Note: limited maintenance activity since mid-2025 but widely used (6.5k+ stars).
* [ExecuteAutomation Playwright MCP](https://github.com/executeautomation/mcp-playwright) ⭐ 5,632 | 🐛 32 | 🌐 TypeScript | 📅 2025-12-13 🆓 - Community Playwright MCP server with API testing support and 143 device emulation profiles.
* [Puppeteer MCP](https://github.com/modelcontextprotocol/servers-archived/tree/main/src/puppeteer) ⚠️ Archived 🆓 - Reference MCP server for Puppeteer-based browser automation from the official MCP servers repo.
* [Podium MCP](https://github.com/hoainho/podium-mcp) ⭐ 3 | 🐛 9 | 🌐 TypeScript | 📅 2026-06-30 🆓 - MCP server purpose-built for mobile app testing on Android/iOS simulators using Maestro, with deep Redux state inspection and CI pipeline integration.
* [prufa-mcp](https://github.com/prufa-dev/prufa-mcp) ⭐ 2 | 🐛 0 | 🌐 Python | 📅 2026-07-01 🆓💰 - Open-source (Apache-2.0) MCP server connected to Prufa's hosted audit backend; an AI agent runs a QA audit of a web app (analytics, broken flows, security headers, accessibility) and gets back machine-verified findings. First audit is free; further audits and features require a paid plan.

## Self-Healing Test Frameworks

Tools that automatically repair broken test locators and adapt to UI changes.

* [CodeceptJS](https://github.com/codeceptjs/CodeceptJS) ⭐ 4,240 | 🐛 217 | 🌐 JavaScript | 📅 2026-08-15 🆓 - End-to-end testing framework with built-in AI heal plugin that uses OpenAI, Anthropic, or local models to repair failing steps and propose locator fixes.
* [Healenium](https://github.com/healenium/healenium) ⭐ 162 | 🐛 49 | 🌐 Shell | 📅 2026-03-31 🆓 - Self-healing library for Selenium, Appium, and Playwright. Replaces broken selectors at runtime.
* [Testim](https://www.testim.io/) 💰 - Pioneer of self-healing tests with AI-driven smart locators.
* [Functionize](https://www.functionize.com/) 💰 - AI-powered tests that adapt without selectors.
* [TestSigma](https://testsigma.com/) 💰 - AI-driven low-code platform with self-healing across web, mobile, and API.
* [Tricentis Tosca](https://www.tricentis.com/products/automate-continuous-testing-tosca) 💰 - Enterprise platform with Vision AI for resilient automation.
* [Perfecto](https://www.perfecto.io/) 💰 - Cloud testing platform with self-healing locators.

## AI-Powered E2E Platforms

End-to-end testing platforms with AI at the core.

* [TestZeus Hercules](https://github.com/test-zeus-ai/testzeus-hercules) ⭐ 1,116 | 🐛 36 | 🌐 Python | 📅 2026-08-04 🆓 - World's first open-source testing agent for UI, API, security, accessibility, and visual validations, no code required.
* [agent-qa](https://github.com/vostride/agent-qa) ⭐ 895 | 🐛 0 | 🌐 TypeScript | 📅 2026-08-03 🆓 - Self-improving QA agent for natural-language web and mobile tests with run memory, UI-change adaptation, and regression detection.
* [Mabl](https://www.mabl.com/) 💰 - Low-code platform with auto-healing and ML-based test maintenance.
* [Meticulous](https://www.meticulous.ai/) 💰 - Records real user sessions and generates regression tests automatically.
* [Momentic](https://momentic.ai/) 💰 - AI-native end-to-end testing platform that writes, runs, and maintains web and mobile tests automatically using natural language.
* [Autify](https://autify.com/) 💰 - No-code end-to-end testing platform with AI-driven maintenance.
* [Reflect](https://reflect.run/) 💰 - No-code regression testing with AI-assisted authoring.
* [QA Wolf](https://www.qawolf.com/) 💰 - AI-powered QA-as-a-service generating Playwright tests at scale.
* [Bug0](https://bug0.com/) 💰 - Agentic testing platform built on the Planner, Generator, Healer pattern with MCP integration.
* [Checksum](https://checksum.ai/) 💰 - Generates Playwright and Cypress tests from real user sessions.
* [Rainforest QA](https://www.rainforestqa.com/) 💰 - No-code testing platform with AI-driven test generation.
* [BrowserStack Low Code Automation](https://www.browserstack.com/low-code-automation) 💰 - AI-powered low-code platform with self-healing agents, NL test authoring, and real device cloud execution.
* [LambdaTest KaneAI](https://www.lambdatest.com/kane-ai) 💰 - GenAI-native test agent for authoring, executing, and maintaining tests using natural language.
* [Virtuoso QA](https://www.virtuosoqa.com/) 💰 - NLP-based codeless E2E platform with self-healing and visual testing.
* [Katalon Studio](https://katalon.com/) 🆓💰 - Test automation platform with AI features including TrueTest and Visual Testing.

## Mobile AI Testing

AI-powered tools specifically for mobile app testing.

* [Maestro](https://github.com/mobile-dev-inc/maestro) ⭐ 15,356 | 🐛 494 | 🌐 Kotlin | 📅 2026-08-17 🆓💰 - YAML-based mobile UI automation that reads accessibility tree, no XPath needed.
* [Appium](https://appium.io/) 🆓 - Industry standard mobile automation, with AI plugins for self-healing.
* [Sofy](https://sofy.ai/) 💰 - No-code AI mobile testing platform.
* [Kobiton](https://kobiton.com/) 💰 - Mobile device cloud with AI-driven scriptless automation.
* [HeadSpin](https://www.headspin.io/) 💰 - Mobile testing platform with AI-driven performance insights.
* [Waldo](https://www.waldo.com/) 💰 - Scriptless mobile testing platform with visual regression and AI-driven flow recording.
* [testRigor](https://testrigor.com/) 💰 - Plain English test authoring across web, mobile, and API with AI-driven element identification.

## Visual AI Testing

Visual regression and UI verification powered by AI.

* [BackstopJS](https://github.com/garris/BackstopJS) ⭐ 7,171 | 🐛 578 | 🌐 JavaScript | 📅 2024-09-07 🆓 - Visual regression testing for responsive web UIs.
* [Pixelmatch](https://github.com/mapbox/pixelmatch) ⭐ 6,917 | 🐛 15 | 🌐 JavaScript | 📅 2026-07-07 🆓 - Pixel-level image comparison library.
* [Loki](https://github.com/oblador/loki) ⭐ 1,908 | 🐛 140 | 🌐 JavaScript | 📅 2024-10-12 🆓 - Visual regression testing for Storybook.
* [Lost Pixel](https://github.com/lost-pixel/lost-pixel) ⚠️ Archived 🆓💰 - Open source visual regression testing.
* [Reg-Suit](https://github.com/reg-viz/reg-suit) ⭐ 1,287 | 🐛 71 | 🌐 TypeScript | 📅 2026-08-14 🆓 - Visual regression testing workflow with publish/notify integrations for CI.
* [Argos](https://github.com/argos-ci/argos) ⭐ 611 | 🐛 3 | 🌐 TypeScript | 📅 2026-08-17 🆓💰 - Open source visual testing for engineering teams.
* [Applitools Eyes](https://applitools.com/) 💰 - Visual AI platform with cross-browser and cross-device verification.
* [Percy](https://percy.io/) 💰 - Visual review and regression testing, part of BrowserStack.
* [Chromatic](https://www.chromatic.com/) 💰 - Visual and interaction tests for Storybook.
* [Happo](https://happo.io/) 💰 - Cross-browser screenshot testing with Playwright, Cypress, and Storybook integrations.

## Natural Language Test Authoring

Write tests using plain English (or other natural languages).

* [Midscene.js](https://github.com/web-infra-dev/midscene) ⭐ 14,595 | 🐛 99 | 🌐 TypeScript | 📅 2026-08-17 🆓 - AI-driven UI automation with natural language commands.
* [Shortest](https://github.com/anti-work/shortest) ⭐ 5,663 | 🐛 2 | 🌐 TypeScript | 📅 2026-08-06 🆓 - QA via natural language AI tests, built on Playwright.
* [Passmark](https://github.com/bug0inc/passmark) ⭐ 1,250 | 🐛 34 | 🌐 TypeScript | 📅 2026-07-30 🆓 - Open-source AI regression testing framework on Playwright with intelligent caching, auto-healing, and multi-model verification.
* [Magnitude](https://github.com/magnitudedev/magnitude) ⭐ 946 | 🐛 6 | 🌐 TypeScript | 📅 2026-08-17 🆓 - AI-native, vision-first testing framework that lets you write E2E tests in plain language.
* [Auto Playwright](https://github.com/lucgagan/auto-playwright) ⭐ 844 | 🐛 22 | 🌐 TypeScript | 📅 2025-07-08 🆓 - Run Playwright tests with AI through plain text prompts.
* [ZeroStep](https://zerostep.com/) 💰 - Plain English test steps that compile to Playwright actions.
* [Tusk](https://www.usetusk.ai/) 💰 - AI agent that auto-generates and runs tests for pull requests.

## LLM-as-Judge Evaluation

Use LLMs to evaluate test outputs, assertions, and quality.

* [Langfuse](https://github.com/langfuse/langfuse) ⭐ 33,260 | 🐛 783 | 🌐 TypeScript | 📅 2026-08-17 🆓💰 - Open source LLM observability, tracing, and evaluation platform.
* [Promptfoo](https://github.com/promptfoo/promptfoo) ⭐ 24,312 | 🐛 512 | 🌐 TypeScript | 📅 2026-08-17 🆓💰 - Test framework with LLM-as-judge for prompts, models, and RAG pipelines.
* [Opik](https://github.com/comet-ml/opik) ⭐ 21,430 | 🐛 201 | 🌐 Python | 📅 2026-08-17 🆓💰 - Open-source LLM evaluation and observability platform with automated tracing, LLM-as-judge metrics, and pytest integration for CI pipelines.
* [OpenAI Evals](https://github.com/openai/evals) ⭐ 19,187 | 🐛 225 | 🌐 Python | 📅 2026-04-14 🆓 - Framework for evaluating LLMs and an open-source registry of benchmarks from OpenAI. No longer actively maintained for new evals, but still widely used as a reference.
* [DeepEval](https://github.com/confident-ai/deepeval) ⭐ 17,644 | 🐛 466 | 🌐 Python | 📅 2026-08-17 🆓💰 - Pytest-like LLM evaluation framework with built-in judge metrics.
* [Ragas](https://github.com/explodinggradients/ragas) ⭐ 15,345 | 🐛 559 | 🌐 Python | 📅 2026-02-24 🆓 - Evaluation framework for RAG pipelines using LLM judges.
* [lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness) ⭐ 13,686 | 🐛 936 | 🌐 Python | 📅 2026-08-14 🆓 - EleutherAI's framework for few-shot evaluation of language models, backing the Hugging Face Open LLM Leaderboard.
* [Arize Phoenix](https://github.com/Arize-ai/phoenix) ⭐ 11,088 | 🐛 923 | 🌐 Python | 📅 2026-08-17 🆓 - Open-source LLM observability and evaluation.
* [Evidently](https://github.com/evidentlyai/evidently) ⭐ 7,813 | 🐛 298 | 🌐 Jupyter Notebook | 📅 2026-08-05 🆓💰 - Open-source Python library for evaluating, testing, and monitoring ML and LLM systems with 100+ built-in metrics for data quality, drift detection, and LLM output quality.
* [Helicone](https://github.com/Helicone/helicone) ⭐ 6,076 | 🐛 172 | 🌐 TypeScript | 📅 2026-08-16 🆓💰 - Open source LLM observability and prompt evaluation platform.
* [TruLens](https://github.com/truera/trulens) ⭐ 3,512 | 🐛 60 | 🌐 Python | 📅 2026-08-14 🆓 - Evaluation framework for LLM apps with feedback functions and tracing.
* [LangWatch](https://github.com/langwatch/langwatch) ⭐ 3,493 | 🐛 835 | 🌐 TypeScript | 📅 2026-08-17 🆓💰 - Open-source LLM evaluation and AI agent testing platform combining end-to-end scenario simulation, observability, and prompt management in a single unified loop.
* [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) ⭐ 2,563 | 🐛 269 | 🌐 Python | 📅 2026-08-17 🆓 - LLM evaluation framework from the UK AI Safety Institute.
* [Weights & Biases Weave](https://github.com/wandb/weave) ⭐ 1,118 | 🐛 243 | 🌐 Python | 📅 2026-08-17 🆓💰 - Weights & Biases toolkit for tracing, debugging, and evaluating generative AI applications with built-in LLM-as-judge metrics and dataset management.
* [LangSmith](https://www.langchain.com/langsmith) 💰 - LangChain's platform for testing and monitoring LLM apps.
* [Braintrust](https://www.braintrust.dev/) 💰 - LLM eval platform with experiments, datasets, and observability.
* [Patronus AI](https://www.patronus.ai/) 💰 - Automated evaluation and security testing for LLMs.
* [Respan](https://www.respan.ai/ai-gateway) 🆓💰 - LLM observability, evaluation, and prompt management platform with a multi-provider gateway.

## Test Analytics and Triage

AI for failure analysis, flaky test detection, and reporting.

* [ReportPortal](https://github.com/reportportal/reportportal) ⭐ 2,018 | 🐛 450 | 🌐 Makefile | 📅 2026-08-14 🆓💰 - Open source results management with ML-based failure clustering.
* [agenttrace](https://github.com/luoyuctl/agenttrace) ⭐ 119 | 🐛 8 | 🌐 Rust | 📅 2026-08-17 🆓 - Local-first TUI and CLI for evaluating AI coding agent sessions with cost, token, latency, and failure regression gates.
* [flaky-test-detector](https://github.com/sametcelikbicak/flaky-test-detector) ⚠️ Archived 🆓 - AI agent skill that detects, analyzes, and eliminates flaky tests across any test runner. Compatible with opencode, Claude Code, Cursor, Windsurf, and GitHub Copilot.
* [Allure TestOps](https://qameta.io/) 💰 - Test management with AI-driven analytics and flaky detection.
* [Sealights](https://www.sealights.io/) 💰 - Quality intelligence platform using ML for test gap analysis.
* [Trunk Flaky Tests](https://trunk.io/flaky-tests) 💰 - ML-based flaky test detection and quarantine.
* [Datadog CI Visibility](https://www.datadoghq.com/product/ci-cd-monitoring/) 💰 - Test analytics with flaky test detection across CI pipelines.
* [Launchable](https://www.launchableinc.com/) 💰 - ML-driven predictive test selection and flaky test detection.
* [BuildPulse](https://buildpulse.io/) 💰 - Flaky test detection and analytics platform.

## Code Coverage with AI

Tools that use AI to fill coverage gaps and prioritize testing efforts.

* [Stryker Mutator](https://github.com/stryker-mutator/stryker-js) ⭐ 3,018 | 🐛 89 | 🌐 TypeScript | 📅 2026-08-15 🆓 - Mutation testing framework that pairs well with AI test generators.
* [Mutahunter](https://github.com/codeintegrity-ai/mutahunter) ⭐ 299 | 🐛 2 | 🌐 Python | 📅 2025-04-17 🆓 - LLM-based mutation testing for stronger test suites.
* [coverage-guard](https://github.com/sametcelikbicak/coverage-guard) ⚠️ Archived 🆓 - AI agent skill that enforces 100% test coverage for any JavaScript/TypeScript project. Works with Vitest, Jest, react-scripts, and more. Compatible with opencode, Claude Code, Cursor, Windsurf, and GitHub Copilot.

## AI Test Data Generation

Tools that use AI to generate realistic test data, fixtures, and edge cases.

* [Faker.js](https://github.com/faker-js/faker) ⭐ 15,449 | 🐛 102 | 🌐 TypeScript | 📅 2026-08-17 🆓 - Standard fake data library, often paired with AI for context-aware data.
* [Datafaker](https://github.com/datafaker-net/datafaker) ⭐ 1,791 | 🐛 11 | 🌐 Java | 📅 2026-08-17 🆓 - Java/Kotlin port of Faker for realistic fake data generation in JVM-based test suites.
* [Snowfakery](https://github.com/SFDO-Tooling/Snowfakery) ⭐ 157 | 🐛 57 | 🌐 Python | 📅 2026-04-27 🆓 - Relational synthetic data generator from Salesforce, useful for complex schema-aware test fixtures.
* [Mockaroo](https://www.mockaroo.com/) 🆓💰 - Realistic test data generation with AI-suggested schemas.
* [Synthesized](https://www.synthesized.io/) 💰 - AI-driven synthetic data platform for testing.
* [Tonic.ai](https://www.tonic.ai/) 💰 - Generate realistic safe test data from production using AI.
* [Gretel](https://gretel.ai/) 💰 - Synthetic data platform with AI-generated test datasets.

## Mock and Service Virtualization

Tools for mocking external services, LLM APIs, and dependencies in AI testing pipelines.

* [MSW (Mock Service Worker)](https://github.com/mswjs/msw) ⭐ 18,143 | 🐛 41 | 🌐 TypeScript | 📅 2026-07-24 🆓 - API mocking library for browser and Node.js, ideal for frontend AI testing.
* [Mockoon](https://github.com/mockoon/mockoon) ⭐ 8,368 | 🐛 46 | 🌐 TypeScript | 📅 2026-08-17 🆓 - GUI-based open source API mocking tool, easy to set up.
* [WireMock](https://github.com/wiremock/wiremock) ⭐ 7,336 | 🐛 495 | 🌐 Java | 📅 2026-08-17 🆓💰 - Industry standard HTTP mocking with 7.1k stars and a native MCP server in the cloud version for AI coding assistants.
* [Hoverfly](https://github.com/SpectoLabs/hoverfly) ⭐ 2,508 | 🐛 34 | 🌐 Go | 📅 2026-08-17 🆓 - Lightweight service virtualization with proxy-based recording and replay.
* [Mountebank](https://github.com/mountebank-testing/mountebank) ⭐ 2,103 | 🐛 101 | 🌐 JavaScript | 📅 2026-08-12 🆓 - Mature open source service virtualization for HTTP, HTTPS, TCP, and SMTP protocols. Supports stubbing, mock verification, and record-playback.
* [Pact](https://github.com/pact-foundation/pact-specification) ⭐ 317 | 🐛 44 | 📅 2024-04-11 🆓 - Contract testing framework for microservices and API consumers.

## Performance Testing with AI

AI-enhanced performance, load, and chaos testing.

* [k6](https://github.com/grafana/k6) ⭐ 31,272 | 🐛 786 | 🌐 Go | 📅 2026-08-17 🆓💰 - Open-source load testing tool, increasingly paired with AI for scenario generation.
* [WebPageTest](https://www.webpagetest.org/) 🆓💰 - Performance testing with AI-suggested optimizations.
* [LoadView](https://www.loadview-testing.com/) 💰 - Cloud-based load testing with AI-powered insights.
* [Akamas](https://www.akamas.io/) 💰 - AI-driven performance optimization and tuning.

## AI for Accessibility Testing

AI-powered accessibility scanners and remediation tools.

* [Pa11y](https://github.com/pa11y/pa11y) ⭐ 4,488 | 🐛 47 | 🌐 JavaScript | 📅 2026-08-17 🆓 - Open-source automated accessibility testing tool.
* [Axe DevTools](https://www.deque.com/axe/devtools/) 💰 - AI-powered accessibility scanner from Deque.
* [Evinced](https://www.evinced.com/) 💰 - AI-driven accessibility testing platform.
* [UserWay](https://userway.org/) 🆓💰 - AI-powered WCAG compliance scanner.

## API Testing with AI

AI features for API testing, schema generation, and contract validation.

* [Keploy](https://github.com/keploy/keploy) ⭐ 18,401 | 🐛 701 | 🌐 Go | 📅 2026-08-17 🆓 - Generates API tests and mocks from real traffic, with AI assertion generation.
* [Stepci](https://github.com/stepci/stepci) ⭐ 1,868 | 🐛 73 | 🌐 TypeScript | 📅 2024-08-03 🆓💰 - API testing framework with AI-suggested assertions.
* [Postman](https://www.postman.com/) 🆓💰 - AI-assisted API test generation and contract validation with Postbot assistant.

## LLM and AI System Testing

Tools to test LLM applications themselves (security, robustness, hallucination).

* [Garak](https://github.com/NVIDIA/garak) ⭐ 8,836 | 🐛 388 | 🌐 Python | 📅 2026-08-14 🆓 - LLM vulnerability scanner from NVIDIA.
* [Guardrails AI](https://github.com/guardrails-ai/guardrails) ⭐ 7,295 | 🐛 87 | 🌐 Python | 📅 2026-08-14 🆓💰 - Python framework for validating and structuring LLM outputs using composable validators covering toxicity, PII leakage, and hallucination detection.
* [NeMo Guardrails](https://github.com/NVIDIA/NeMo-Guardrails) ⭐ 6,967 | 🐛 218 | 🌐 Python | 📅 2026-08-17 🆓 - Open-source toolkit from NVIDIA for adding programmable guardrails to LLM-based conversational systems, preventing jailbreaks, topic drift, and unsafe outputs.
* [Giskard](https://github.com/Giskard-AI/giskard) ⭐ 5,754 | 🐛 56 | 🌐 Python | 📅 2026-08-17 🆓💰 - Testing framework for LLMs and ML models.
* [LLM Guard](https://github.com/protectai/llm-guard) ⚠️ Archived 🆓 - Open source security toolkit from Protect AI with scanners for prompt injection, toxicity, secrets, and data leakage in LLM inputs and outputs.
* [DeepTeam](https://github.com/confident-ai/deepteam) ⭐ 2,451 | 🐛 56 | 🌐 Python | 📅 2026-08-12 🆓 - LLM red teaming for prompt injection, jailbreaks, and data leaks.
* [LLMFuzzer](https://github.com/mnns/LLMFuzzer) ⭐ 377 | 🐛 3 | 🌐 Python | 📅 2024-02-12 🆓 - Early open-source fuzzing framework for testing LLMs via their API integrations. No longer actively maintained (last commit early 2024) but still referenced in LLM security lists.
* [PyRIT](https://github.com/Azure/PyRIT) ⚠️ Archived 🆓 - Microsoft's Python Risk Identification Tool for generative AI.
* [llm-security-scanner](https://github.com/tugkanboz/llm-security-scanner) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-05-02 🆓 - Red-team toolkit with OWASP LLM Top 10 alignment and Turkish payload library.
* [Lakera Guard](https://www.lakera.ai/) 💰 - Real-time prompt injection and jailbreak detection.
* [Prompt Security](https://www.prompt.security/) 💰 - Runtime prompt injection and data leak protection platform.
* [WhyLabs](https://whylabs.ai/) 💰 - ML observability and LLM monitoring.
* [Confident AI](https://www.confident-ai.com/) 💰 - LLM testing platform built around DeepEval.

## Browser Automation for AI Agents

Browser automation libraries designed for or commonly used by AI agents.

* [Browser Use](https://github.com/browser-use/browser-use) ⭐ 109,508 | 🐛 359 | 🌐 Python | 📅 2026-08-17 🆓 - Make websites accessible to AI agents.
* [Lightpanda](https://github.com/lightpanda-io/browser) ⭐ 34,001 | 🐛 88 | 🌐 Zig | 📅 2026-08-17 🆓 - Headless browser written in Zig, optimized for AI agents and scraping workloads.
* [Stagehand](https://github.com/browserbase/stagehand) ⭐ 23,966 | 🐛 328 | 🌐 TypeScript | 📅 2026-08-17 🆓 - AI browser automation with predictable yet flexible APIs.
* [Skyvern](https://github.com/Skyvern-AI/skyvern) ⭐ 22,771 | 🐛 218 | 🌐 Python | 📅 2026-08-17 🆓💰 - Automate browser-based workflows using LLMs and computer vision.
* [Steel Browser](https://github.com/steel-dev/steel-browser) ⭐ 7,498 | 🐛 58 | 🌐 TypeScript | 📅 2026-08-05 🆓 - Open-source browser API for AI agents.
* [Patchright](https://github.com/Kaliiiiiiiiii-Vinyzu/patchright) ⭐ 4,109 | 🐛 3 | 🌐 TypeScript | 📅 2026-08-17 🆓 - Patched Playwright for stealth automation.
* [AgentQL](https://github.com/tinyfish-io/agentql) ⭐ 1,451 | 🐛 9 | 🌐 Python | 📅 2026-08-17 🆓💰 - Natural language query language for AI agents to interact with and extract structured data from web pages, with self-healing selectors that integrate with Playwright.
* [Browserbase](https://www.browserbase.com/) 💰 - Cloud browser infrastructure with natural language automation.

## Articles and Talks

Essential reading on AI in software testing.

* [Best AI Test Generation Tools for Playwright in 2026](https://testdino.com/blog/ai-test-generation-tools/) - Practical guide to choosing AI test generators.
* [Playwright Test Agents: AI Testing Explained](https://bug0.com/blog/playwright-test-agents) - Deep dive into the Planner, Generator, Healer pattern.
* [Modern Test Automation with LLM and Playwright MCP](https://kailash-pathak.medium.com/modern-test-automation-with-ai-llm-and-playwright-mcp-model-context-protocol-0c311292c7fb) - Setting up MCP for test automation.
* [20 Open-Source Projects Redefining AI + Playwright Testing](https://bug0.com/blog/20-underdog-open-source-projects-pushing-limits-ai-playwright) - Roundup of emerging AI Playwright projects.
* [Best 12 Generative AI Testing Tools 2026](https://hashnode.com/blog/best-generative-ai-testing-tools-2026) - Ranked review of top GenAI testing platforms.
* [Give your AI eyes: Introducing Chrome DevTools MCP](https://addyosmani.com/blog/devtools-mcp/) - Deep dive on Chrome DevTools MCP by Addy Osmani.
* [State of AI in Software Testing 2026](https://www.browserstack.com/resources/state-of-ai-in-software-testing) - BrowserStack's industry report on AI adoption trends in QA.
* [The Test Pyramid in the AI Era](https://martinfowler.com/articles/practical-test-pyramid.html) - Classic reference, still relevant.

## Courses and Tutorials

Learning resources for AI-powered testing.

* [Generative AI in Software Testing](https://www.udemy.com/course/generative-ai-in-software-testing/) - Comprehensive course on Copilot, Claude Code, MCP, and AI agents for QA.
* [Test Automation University](https://testautomationu.applitools.com/) - Free courses including AI testing modules from Applitools.
* [Chrome DevTools MCP Tutorial](https://www.datacamp.com/tutorial/chrome-devtools-mcp) - DataCamp's hands-on guide to Chrome DevTools MCP with AI assistants.

## Newsletters and Communities

* [Software Testing Weekly](https://softwaretestingweekly.com/) - Weekly testing newsletter with strong AI coverage.
* [Test Guild](https://testguild.com/) - Podcast and community for automation testing.
* [Ministry of Testing](https://www.ministryoftesting.com/) - Global testing community with AI-focused tracks.

## Benchmarks and Datasets

* [SWE-bench](https://github.com/princeton-nlp/SWE-bench) ⭐ 5,655 | 🐛 5 | 🌐 Python | 📅 2026-08-17 - Benchmark for evaluating LLMs on real software engineering tasks, including test fixes.
* [AgentBench](https://github.com/THUDM/AgentBench) ⭐ 3,675 | 🐛 75 | 🌐 Python | 📅 2026-02-08 🆓 - ICLR 2024 benchmark for evaluating LLMs as autonomous agents across eight environments including OS, database, web browsing, and game tasks.
* [HumanEval](https://github.com/openai/human-eval) ⭐ 3,341 | 🐛 44 | 🌐 Python | 📅 2025-01-17 - Evaluating large language models trained on code.
* [OSWorld](https://github.com/xlang-ai/OSWorld) ⭐ 3,090 | 🐛 191 | 🌐 Python | 📅 2026-08-12 🆓 - NeurIPS 2024 benchmark for evaluating multimodal AI agents on open-ended tasks in real computer environments, supporting VMware, Docker, and AWS virtualization.
* [HELM](https://github.com/stanford-crfm/helm) ⭐ 2,879 | 🐛 93 | 🌐 Python | 📅 2026-08-01 🆓 - Stanford CRFM's open-source Python framework for holistic, reproducible, and transparent evaluation of LLMs and multimodal models across dozens of scenarios covering accuracy, robustness, efficiency, bias, and safety.
* [WebArena](https://github.com/web-arena-x/webarena) ⭐ 1,579 | 🐛 100 | 🌐 Python | 📅 2025-11-26 - Self-hostable web environment for building and evaluating autonomous agents on realistic, multi-site tasks.
* [tau-bench](https://github.com/sierra-research/tau-bench) ⭐ 1,386 | 🐛 51 | 🌐 Python | 📅 2026-03-18 - Benchmark for evaluating tool-using language agents through dynamic conversations with simulated users and domain-specific APIs.
* [StructEval](https://github.com/TIGER-AI-Lab/StructEval) ⭐ 23 | 🐛 6 | 🌐 Python | 📅 2026-07-26 🆓 - Benchmark for structured-output generation and cross-format conversion across text and renderable formats, with syntax, structural, and visual-fidelity checks.
* [BenchClaw](https://github.com/Agnuxo1/BenchClaw) ⭐ 6 | 🐛 0 | 🌐 HTML | 📅 2026-06-05 🆓 - Multi-dimension AI benchmark with 17-judge evaluation tribunal for scientific paper generation. Evaluates IMRaD structure, citation quality, methodological rigor, and reproducibility across 10 dimensions with uncertainty quantification and P2P verification.

## Related Awesome Lists

* [awesome-test-automation](https://github.com/atinfo/awesome-test-automation) ⭐ 7,134 | 🐛 127 | 📅 2025-11-28 - General test automation across languages.
* [awesome-llm-security](https://github.com/corca-ai/awesome-llm-security) ⭐ 1,683 | 🐛 185 | 📅 2025-08-20 - LLM security tools and resources.
* [awesome-mutation-testing](https://github.com/theofidry/awesome-mutation-testing) ⭐ 467 | 🐛 2 | 📅 2026-08-06 - Mutation testing resources.
* [awesome-testing-tools](https://github.com/ZoranPandovski/awesome-testing-tools) ⭐ 364 | 🐛 30 | 🌐 CSS | 📅 2026-06-19 - General testing tools.
* [awesome-ai-agent-testing](https://github.com/chaosync-org/awesome-ai-agent-testing) ⭐ 46 | 🐛 14 | 📅 2025-05-28 - Testing AI agents themselves.
* [awesome-ai-pentest](https://github.com/insidetrust/awesome-ai-pentest) ⭐ 27 | 🐛 1 | 📅 2026-02-20 - AI-assisted penetration testing.

## Contributing

Contributions are welcome. Please read the [contribution guidelines](contributing.md) before opening a pull request.

***

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-08-17._
