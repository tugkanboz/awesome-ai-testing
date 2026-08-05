# Awesome AI Testing [![Awesome](https://awesome.re/badge.svg)](https://awesome.re) [![Lint](https://github.com/tugkanboz/awesome-ai-testing/actions/workflows/lint.yml/badge.svg)](https://github.com/tugkanboz/awesome-ai-testing/actions/workflows/lint.yml)

> A curated list of AI-powered testing tools, frameworks, and resources for QA engineers.

AI is reshaping software testing. This list collects tools, platforms, and resources that use AI or LLMs to generate tests, heal broken locators, triage failures, write assertions in natural language, and more. Both open source and commercial offerings are included, marked with badges so you can filter by what fits your stack.

## Contents

- [Legend](#legend)
- [Test Generation](#test-generation)
- [MCP-Based Testing](#mcp-based-testing)
- [Self-Healing Test Frameworks](#self-healing-test-frameworks)
- [AI-Powered E2E Platforms](#ai-powered-e2e-platforms)
- [Mobile AI Testing](#mobile-ai-testing)
- [Visual AI Testing](#visual-ai-testing)
- [Natural Language Test Authoring](#natural-language-test-authoring)
- [LLM-as-Judge Evaluation](#llm-as-judge-evaluation)
- [Test Analytics and Triage](#test-analytics-and-triage)
- [Code Coverage with AI](#code-coverage-with-ai)
- [AI Test Data Generation](#ai-test-data-generation)
- [Mock and Service Virtualization](#mock-and-service-virtualization)
- [Performance Testing with AI](#performance-testing-with-ai)
- [AI for Accessibility Testing](#ai-for-accessibility-testing)
- [API Testing with AI](#api-testing-with-ai)
- [LLM and AI System Testing](#llm-and-ai-system-testing)
- [Browser Automation for AI Agents](#browser-automation-for-ai-agents)
- [Articles and Talks](#articles-and-talks)
- [Courses and Tutorials](#courses-and-tutorials)
- [Newsletters and Communities](#newsletters-and-communities)
- [Benchmarks and Datasets](#benchmarks-and-datasets)
- [Related Awesome Lists](#related-awesome-lists)

## Legend

- 🆓 Open source
- 💰 Commercial
- 🆓💰 Open core (free tier or open source with paid features)

## Test Generation

Tools that generate test cases from code, requirements, or user behavior using AI.

- [Qodo-Cover](https://github.com/qodo-ai/qodo-cover) 🆓 - AI-powered tool for automated test generation and code coverage enhancement.
- [EvoMaster](https://github.com/EMResearch/EvoMaster) 🆓 - First open source AI tool that automatically generates test cases via evolutionary algorithms for REST, GraphQL, and RPC APIs.
- [EvoSuite](https://github.com/EvoSuite/evosuite) 🆓 - Generates JUnit tests using evolutionary and genetic search-based algorithms for Java.
- [Pynguin](https://github.com/se2p/pynguin) 🆓 - Automated unit test generation for Python via evolutionary algorithms, from Saarland University.
- [Symflower](https://symflower.com/) 💰 - Commercial tool that combines symbolic execution, static analysis, and LLMs to generate unit tests for Java, Go, and Kotlin. Free CLI available with limitations.
- [CodiumAI / Qodo](https://www.qodo.ai/) 💰 - AI assistant generating meaningful tests from code context.
- [Diffblue Cover](https://www.diffblue.com/) 💰 - Autonomous Java unit test writer using reinforcement learning.
- [GitHub Copilot](https://github.com/features/copilot) 💰 - AI pair programmer that generates test code in Playwright, Cypress, Selenium across editors.
- [Cursor](https://www.cursor.com/) 💰 - AI-first code editor with strong test generation capabilities for major frameworks.
- [Claude Code](https://www.anthropic.com/claude-code) 💰 - Anthropic's terminal-based agentic coding assistant, useful for test suite generation and refactoring.

## MCP-Based Testing

Tools and servers that use the Model Context Protocol to give AI agents browser control and testing capabilities.

- [Playwright MCP](https://github.com/microsoft/playwright-mcp) 🆓 - Official Playwright MCP server giving AI agents full browser control through structured accessibility snapshots.
- [Playwright CLI](https://github.com/microsoft/playwright-cli) 🆓 - Token-efficient CLI for coding agents like Claude Code and GitHub Copilot, with installable skills.
- [Chrome DevTools MCP](https://github.com/ChromeDevTools/chrome-devtools-mcp) 🆓 - Official MCP server from the Chrome DevTools team, with 26 tools for browser automation, debugging, and performance analysis.
- [ExecuteAutomation Playwright MCP](https://github.com/executeautomation/mcp-playwright) 🆓 - Community Playwright MCP server with API testing support and 143 device emulation profiles.
- [BrowserTools MCP](https://github.com/AgentDeskAI/browser-tools-mcp) 🆓 - Browser monitoring and console log access for AI agents via Chrome extension.
- [Browser MCP](https://github.com/browsermcp/mcp) 🆓 - Popular MCP server that automates the user's own local browser, preserving logged-in sessions and avoiding bot detection. Note: limited maintenance activity since mid-2025 but widely used (6.5k+ stars).
- [Podium MCP](https://github.com/hoainho/podium-mcp) 🆓 - MCP server purpose-built for mobile app testing on Android/iOS simulators using Maestro, with deep Redux state inspection and CI pipeline integration.
- [Puppeteer MCP](https://github.com/modelcontextprotocol/servers-archived/tree/main/src/puppeteer) 🆓 - Reference MCP server for Puppeteer-based browser automation from the official MCP servers repo.
- [prufa-mcp](https://github.com/prufa-dev/prufa-mcp) 🆓💰 - Open-source (Apache-2.0) MCP server connected to Prufa's hosted audit backend; an AI agent runs a QA audit of a web app (analytics, broken flows, security headers, accessibility) and gets back machine-verified findings. First audit is free; further audits and features require a paid plan.

## Self-Healing Test Frameworks

Tools that automatically repair broken test locators and adapt to UI changes.

- [Healenium](https://github.com/healenium/healenium) 🆓 - Self-healing library for Selenium, Appium, and Playwright. Replaces broken selectors at runtime.
- [CodeceptJS](https://github.com/codeceptjs/CodeceptJS) 🆓 - End-to-end testing framework with built-in AI heal plugin that uses OpenAI, Anthropic, or local models to repair failing steps and propose locator fixes.
- [Testim](https://www.testim.io/) 💰 - Pioneer of self-healing tests with AI-driven smart locators.
- [Functionize](https://www.functionize.com/) 💰 - AI-powered tests that adapt without selectors.
- [TestSigma](https://testsigma.com/) 💰 - AI-driven low-code platform with self-healing across web, mobile, and API.
- [Tricentis Tosca](https://www.tricentis.com/products/automate-continuous-testing-tosca) 💰 - Enterprise platform with Vision AI for resilient automation.
- [Perfecto](https://www.perfecto.io/) 💰 - Cloud testing platform with self-healing locators.

## AI-Powered E2E Platforms

End-to-end testing platforms with AI at the core.

- [TestZeus Hercules](https://github.com/test-zeus-ai/testzeus-hercules) 🆓 - World's first open-source testing agent for UI, API, security, accessibility, and visual validations, no code required.
- [agent-qa](https://github.com/vostride/agent-qa) 🆓 - Self-improving QA agent for natural-language web and mobile tests with run memory, UI-change adaptation, and regression detection.
- [Mabl](https://www.mabl.com/) 💰 - Low-code platform with auto-healing and ML-based test maintenance.
- [Meticulous](https://www.meticulous.ai/) 💰 - Records real user sessions and generates regression tests automatically.
- [Momentic](https://momentic.ai/) 💰 - AI-native end-to-end testing platform that writes, runs, and maintains web and mobile tests automatically using natural language.
- [Autify](https://autify.com/) 💰 - No-code end-to-end testing platform with AI-driven maintenance.
- [Reflect](https://reflect.run/) 💰 - No-code regression testing with AI-assisted authoring.
- [QA Wolf](https://www.qawolf.com/) 💰 - AI-powered QA-as-a-service generating Playwright tests at scale.
- [Bug0](https://bug0.com/) 💰 - Agentic testing platform built on the Planner, Generator, Healer pattern with MCP integration.
- [Checksum](https://checksum.ai/) 💰 - Generates Playwright and Cypress tests from real user sessions.
- [Rainforest QA](https://www.rainforestqa.com/) 💰 - No-code testing platform with AI-driven test generation.
- [BrowserStack Low Code Automation](https://www.browserstack.com/low-code-automation) 💰 - AI-powered low-code platform with self-healing agents, NL test authoring, and real device cloud execution.
- [LambdaTest KaneAI](https://www.lambdatest.com/kane-ai) 💰 - GenAI-native test agent for authoring, executing, and maintaining tests using natural language.
- [Virtuoso QA](https://www.virtuosoqa.com/) 💰 - NLP-based codeless E2E platform with self-healing and visual testing.
- [Katalon Studio](https://katalon.com/) 🆓💰 - Test automation platform with AI features including TrueTest and Visual Testing.

## Mobile AI Testing

AI-powered tools specifically for mobile app testing.

- [Maestro](https://github.com/mobile-dev-inc/maestro) 🆓💰 - YAML-based mobile UI automation that reads accessibility tree, no XPath needed.
- [Appium](https://appium.io/) 🆓 - Industry standard mobile automation, with AI plugins for self-healing.
- [Sofy](https://sofy.ai/) 💰 - No-code AI mobile testing platform.
- [Kobiton](https://kobiton.com/) 💰 - Mobile device cloud with AI-driven scriptless automation.
- [HeadSpin](https://www.headspin.io/) 💰 - Mobile testing platform with AI-driven performance insights.
- [Waldo](https://www.waldo.com/) 💰 - Scriptless mobile testing platform with visual regression and AI-driven flow recording.
- [testRigor](https://testrigor.com/) 💰 - Plain English test authoring across web, mobile, and API with AI-driven element identification.

## Visual AI Testing

Visual regression and UI verification powered by AI.

- [Lost Pixel](https://github.com/lost-pixel/lost-pixel) 🆓💰 - Open source visual regression testing.
- [Loki](https://github.com/oblador/loki) 🆓 - Visual regression testing for Storybook.
- [Argos](https://github.com/argos-ci/argos) 🆓💰 - Open source visual testing for engineering teams.
- [BackstopJS](https://github.com/garris/BackstopJS) 🆓 - Visual regression testing for responsive web UIs.
- [Pixelmatch](https://github.com/mapbox/pixelmatch) 🆓 - Pixel-level image comparison library.
- [Reg-Suit](https://github.com/reg-viz/reg-suit) 🆓 - Visual regression testing workflow with publish/notify integrations for CI.
- [Applitools Eyes](https://applitools.com/) 💰 - Visual AI platform with cross-browser and cross-device verification.
- [Percy](https://percy.io/) 💰 - Visual review and regression testing, part of BrowserStack.
- [Chromatic](https://www.chromatic.com/) 💰 - Visual and interaction tests for Storybook.
- [Happo](https://happo.io/) 💰 - Cross-browser screenshot testing with Playwright, Cypress, and Storybook integrations.

## Natural Language Test Authoring

Write tests using plain English (or other natural languages).

- [Shortest](https://github.com/anti-work/shortest) 🆓 - QA via natural language AI tests, built on Playwright.
- [Magnitude](https://github.com/magnitudedev/magnitude) 🆓 - AI-native, vision-first testing framework that lets you write E2E tests in plain language.
- [Auto Playwright](https://github.com/lucgagan/auto-playwright) 🆓 - Run Playwright tests with AI through plain text prompts.
- [Passmark](https://github.com/bug0inc/passmark) 🆓 - Open-source AI regression testing framework on Playwright with intelligent caching, auto-healing, and multi-model verification.
- [Midscene.js](https://github.com/web-infra-dev/midscene) 🆓 - AI-driven UI automation with natural language commands.
- [ZeroStep](https://zerostep.com/) 💰 - Plain English test steps that compile to Playwright actions.
- [Tusk](https://www.usetusk.ai/) 💰 - AI agent that auto-generates and runs tests for pull requests.

## LLM-as-Judge Evaluation

Use LLMs to evaluate test outputs, assertions, and quality.

- [Promptfoo](https://github.com/promptfoo/promptfoo) 🆓💰 - Test framework with LLM-as-judge for prompts, models, and RAG pipelines.
- [DeepEval](https://github.com/confident-ai/deepeval) 🆓💰 - Pytest-like LLM evaluation framework with built-in judge metrics.
- [Ragas](https://github.com/explodinggradients/ragas) 🆓 - Evaluation framework for RAG pipelines using LLM judges.
- [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) 🆓 - LLM evaluation framework from the UK AI Safety Institute.
- [TruLens](https://github.com/truera/trulens) 🆓 - Evaluation framework for LLM apps with feedback functions and tracing.
- [Arize Phoenix](https://github.com/Arize-ai/phoenix) 🆓 - Open-source LLM observability and evaluation.
- [Weights & Biases Weave](https://github.com/wandb/weave) 🆓💰 - Weights & Biases toolkit for tracing, debugging, and evaluating generative AI applications with built-in LLM-as-judge metrics and dataset management.
- [OpenAI Evals](https://github.com/openai/evals) 🆓 - Framework for evaluating LLMs and an open-source registry of benchmarks from OpenAI. No longer actively maintained for new evals, but still widely used as a reference.
- [lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness) 🆓 - EleutherAI's framework for few-shot evaluation of language models, backing the Hugging Face Open LLM Leaderboard.
- [Langfuse](https://github.com/langfuse/langfuse) 🆓💰 - Open source LLM observability, tracing, and evaluation platform.
- [Helicone](https://github.com/Helicone/helicone) 🆓💰 - Open source LLM observability and prompt evaluation platform.
- [Opik](https://github.com/comet-ml/opik) 🆓💰 - Open-source LLM evaluation and observability platform with automated tracing, LLM-as-judge metrics, and pytest integration for CI pipelines.
- [LangWatch](https://github.com/langwatch/langwatch) 🆓💰 - Open-source LLM evaluation and AI agent testing platform combining end-to-end scenario simulation, observability, and prompt management in a single unified loop.
- [Evidently](https://github.com/evidentlyai/evidently) 🆓💰 - Open-source Python library for evaluating, testing, and monitoring ML and LLM systems with 100+ built-in metrics for data quality, drift detection, and LLM output quality.
- [LangSmith](https://www.langchain.com/langsmith) 💰 - LangChain's platform for testing and monitoring LLM apps.
- [Braintrust](https://www.braintrust.dev/) 💰 - LLM eval platform with experiments, datasets, and observability.
- [Patronus AI](https://www.patronus.ai/) 💰 - Automated evaluation and security testing for LLMs.
- [Respan](https://www.respan.ai/ai-gateway) 🆓💰 - LLM observability, evaluation, and prompt management platform with a multi-provider gateway.

## Test Analytics and Triage

AI for failure analysis, flaky test detection, and reporting.

- [agenttrace](https://github.com/luoyuctl/agenttrace) 🆓 - Local-first TUI and CLI for evaluating AI coding agent sessions with cost, token, latency, and failure regression gates.
- [ReportPortal](https://github.com/reportportal/reportportal) 🆓💰 - Open source results management with ML-based failure clustering.
- [Allure TestOps](https://qameta.io/) 💰 - Test management with AI-driven analytics and flaky detection.
- [Sealights](https://www.sealights.io/) 💰 - Quality intelligence platform using ML for test gap analysis.
- [Trunk Flaky Tests](https://trunk.io/flaky-tests) 💰 - ML-based flaky test detection and quarantine.
- [Datadog CI Visibility](https://www.datadoghq.com/product/ci-cd-monitoring/) 💰 - Test analytics with flaky test detection across CI pipelines.
- [Launchable](https://www.launchableinc.com/) 💰 - ML-driven predictive test selection and flaky test detection.
- [BuildPulse](https://buildpulse.io/) 💰 - Flaky test detection and analytics platform.
- [flaky-test-detector](https://github.com/sametcelikbicak/flaky-test-detector) 🆓 - AI agent skill that detects, analyzes, and eliminates flaky tests across any test runner. Compatible with opencode, Claude Code, Cursor, Windsurf, and GitHub Copilot.

## Code Coverage with AI

Tools that use AI to fill coverage gaps and prioritize testing efforts.

- [Mutahunter](https://github.com/codeintegrity-ai/mutahunter) 🆓 - LLM-based mutation testing for stronger test suites.
- [Stryker Mutator](https://github.com/stryker-mutator/stryker-js) 🆓 - Mutation testing framework that pairs well with AI test generators.
- [coverage-guard](https://github.com/sametcelikbicak/coverage-guard) 🆓 - AI agent skill that enforces 100% test coverage for any JavaScript/TypeScript project. Works with Vitest, Jest, react-scripts, and more. Compatible with opencode, Claude Code, Cursor, Windsurf, and GitHub Copilot.

## AI Test Data Generation

Tools that use AI to generate realistic test data, fixtures, and edge cases.

- [Faker.js](https://github.com/faker-js/faker) 🆓 - Standard fake data library, often paired with AI for context-aware data.
- [Datafaker](https://github.com/datafaker-net/datafaker) 🆓 - Java/Kotlin port of Faker for realistic fake data generation in JVM-based test suites.
- [Snowfakery](https://github.com/SFDO-Tooling/Snowfakery) 🆓 - Relational synthetic data generator from Salesforce, useful for complex schema-aware test fixtures.
- [Mockaroo](https://www.mockaroo.com/) 🆓💰 - Realistic test data generation with AI-suggested schemas.
- [Synthesized](https://www.synthesized.io/) 💰 - AI-driven synthetic data platform for testing.
- [Tonic.ai](https://www.tonic.ai/) 💰 - Generate realistic safe test data from production using AI.
- [Gretel](https://gretel.ai/) 💰 - Synthetic data platform with AI-generated test datasets.

## Mock and Service Virtualization

Tools for mocking external services, LLM APIs, and dependencies in AI testing pipelines.

- [Mountebank](https://github.com/mountebank-testing/mountebank) 🆓 - Mature open source service virtualization for HTTP, HTTPS, TCP, and SMTP protocols. Supports stubbing, mock verification, and record-playback.
- [WireMock](https://github.com/wiremock/wiremock) 🆓💰 - Industry standard HTTP mocking with 7.1k stars and a native MCP server in the cloud version for AI coding assistants.
- [Mockoon](https://github.com/mockoon/mockoon) 🆓 - GUI-based open source API mocking tool, easy to set up.
- [Pact](https://github.com/pact-foundation/pact-specification) 🆓 - Contract testing framework for microservices and API consumers.
- [MSW (Mock Service Worker)](https://github.com/mswjs/msw) 🆓 - API mocking library for browser and Node.js, ideal for frontend AI testing.
- [Hoverfly](https://github.com/SpectoLabs/hoverfly) 🆓 - Lightweight service virtualization with proxy-based recording and replay.

## Performance Testing with AI

AI-enhanced performance, load, and chaos testing.

- [k6](https://github.com/grafana/k6) 🆓💰 - Open-source load testing tool, increasingly paired with AI for scenario generation.
- [WebPageTest](https://www.webpagetest.org/) 🆓💰 - Performance testing with AI-suggested optimizations.
- [LoadView](https://www.loadview-testing.com/) 💰 - Cloud-based load testing with AI-powered insights.
- [Akamas](https://www.akamas.io/) 💰 - AI-driven performance optimization and tuning.

## AI for Accessibility Testing

AI-powered accessibility scanners and remediation tools.

- [Pa11y](https://github.com/pa11y/pa11y) 🆓 - Open-source automated accessibility testing tool.
- [Axe DevTools](https://www.deque.com/axe/devtools/) 💰 - AI-powered accessibility scanner from Deque.
- [Evinced](https://www.evinced.com/) 💰 - AI-driven accessibility testing platform.
- [UserWay](https://userway.org/) 🆓💰 - AI-powered WCAG compliance scanner.

## API Testing with AI

AI features for API testing, schema generation, and contract validation.

- [Keploy](https://github.com/keploy/keploy) 🆓 - Generates API tests and mocks from real traffic, with AI assertion generation.
- [Stepci](https://github.com/stepci/stepci) 🆓💰 - API testing framework with AI-suggested assertions.
- [Postman](https://www.postman.com/) 🆓💰 - AI-assisted API test generation and contract validation with Postbot assistant.

## LLM and AI System Testing

Tools to test LLM applications themselves (security, robustness, hallucination).

- [Garak](https://github.com/NVIDIA/garak) 🆓 - LLM vulnerability scanner from NVIDIA.
- [DeepTeam](https://github.com/confident-ai/deepteam) 🆓 - LLM red teaming for prompt injection, jailbreaks, and data leaks.
- [llm-security-scanner](https://github.com/tugkanboz/llm-security-scanner) 🆓 - Red-team toolkit with OWASP LLM Top 10 alignment and Turkish payload library.
- [Giskard](https://github.com/Giskard-AI/giskard) 🆓💰 - Testing framework for LLMs and ML models.
- [Guardrails AI](https://github.com/guardrails-ai/guardrails) 🆓💰 - Python framework for validating and structuring LLM outputs using composable validators covering toxicity, PII leakage, and hallucination detection.
- [NeMo Guardrails](https://github.com/NVIDIA/NeMo-Guardrails) 🆓 - Open-source toolkit from NVIDIA for adding programmable guardrails to LLM-based conversational systems, preventing jailbreaks, topic drift, and unsafe outputs.
- [PyRIT](https://github.com/Azure/PyRIT) 🆓 - Microsoft's Python Risk Identification Tool for generative AI.
- [LLM Guard](https://github.com/protectai/llm-guard) 🆓 - Open source security toolkit from Protect AI with scanners for prompt injection, toxicity, secrets, and data leakage in LLM inputs and outputs.
- [LLMFuzzer](https://github.com/mnns/LLMFuzzer) 🆓 - Early open-source fuzzing framework for testing LLMs via their API integrations. No longer actively maintained (last commit early 2024) but still referenced in LLM security lists.
- [Lakera Guard](https://www.lakera.ai/) 💰 - Real-time prompt injection and jailbreak detection.
- [Prompt Security](https://www.prompt.security/) 💰 - Runtime prompt injection and data leak protection platform.
- [WhyLabs](https://whylabs.ai/) 💰 - ML observability and LLM monitoring.
- [Confident AI](https://www.confident-ai.com/) 💰 - LLM testing platform built around DeepEval.

## Browser Automation for AI Agents

Browser automation libraries designed for or commonly used by AI agents.

- [Browser Use](https://github.com/browser-use/browser-use) 🆓 - Make websites accessible to AI agents.
- [Stagehand](https://github.com/browserbase/stagehand) 🆓 - AI browser automation with predictable yet flexible APIs.
- [Skyvern](https://github.com/Skyvern-AI/skyvern) 🆓💰 - Automate browser-based workflows using LLMs and computer vision.
- [Steel Browser](https://github.com/steel-dev/steel-browser) 🆓 - Open-source browser API for AI agents.
- [Patchright](https://github.com/Kaliiiiiiiiii-Vinyzu/patchright) 🆓 - Patched Playwright for stealth automation.
- [Lightpanda](https://github.com/lightpanda-io/browser) 🆓 - Headless browser written in Zig, optimized for AI agents and scraping workloads.
- [AgentQL](https://github.com/tinyfish-io/agentql) 🆓💰 - Natural language query language for AI agents to interact with and extract structured data from web pages, with self-healing selectors that integrate with Playwright.
- [Browserbase](https://www.browserbase.com/) 💰 - Cloud browser infrastructure with natural language automation.

## Articles and Talks

Essential reading on AI in software testing.

- [Best AI Test Generation Tools for Playwright in 2026](https://testdino.com/blog/ai-test-generation-tools/) - Practical guide to choosing AI test generators.
- [Playwright Test Agents: AI Testing Explained](https://bug0.com/blog/playwright-test-agents) - Deep dive into the Planner, Generator, Healer pattern.
- [Modern Test Automation with LLM and Playwright MCP](https://kailash-pathak.medium.com/modern-test-automation-with-ai-llm-and-playwright-mcp-model-context-protocol-0c311292c7fb) - Setting up MCP for test automation.
- [20 Open-Source Projects Redefining AI + Playwright Testing](https://bug0.com/blog/20-underdog-open-source-projects-pushing-limits-ai-playwright) - Roundup of emerging AI Playwright projects.
- [Best 12 Generative AI Testing Tools 2026](https://hashnode.com/blog/best-generative-ai-testing-tools-2026) - Ranked review of top GenAI testing platforms.
- [Give your AI eyes: Introducing Chrome DevTools MCP](https://addyosmani.com/blog/devtools-mcp/) - Deep dive on Chrome DevTools MCP by Addy Osmani.
- [State of AI in Software Testing 2026](https://www.browserstack.com/resources/state-of-ai-in-software-testing) - BrowserStack's industry report on AI adoption trends in QA.
- [The Test Pyramid in the AI Era](https://martinfowler.com/articles/practical-test-pyramid.html) - Classic reference, still relevant.

## Courses and Tutorials

Learning resources for AI-powered testing.

- [Generative AI in Software Testing](https://www.udemy.com/course/generative-ai-in-software-testing/) - Comprehensive course on Copilot, Claude Code, MCP, and AI agents for QA.
- [Test Automation University](https://testautomationu.applitools.com/) - Free courses including AI testing modules from Applitools.
- [Chrome DevTools MCP Tutorial](https://www.datacamp.com/tutorial/chrome-devtools-mcp) - DataCamp's hands-on guide to Chrome DevTools MCP with AI assistants.

## Newsletters and Communities

- [Software Testing Weekly](https://softwaretestingweekly.com/) - Weekly testing newsletter with strong AI coverage.
- [Test Guild](https://testguild.com/) - Podcast and community for automation testing.
- [Ministry of Testing](https://www.ministryoftesting.com/) - Global testing community with AI-focused tracks.

## Benchmarks and Datasets

- [BenchClaw](https://github.com/Agnuxo1/BenchClaw) 🆓 - Multi-dimension AI benchmark with 17-judge evaluation tribunal for scientific paper generation. Evaluates IMRaD structure, citation quality, methodological rigor, and reproducibility across 10 dimensions with uncertainty quantification and P2P verification.
- [HELM](https://github.com/stanford-crfm/helm) 🆓 - Stanford CRFM's open-source Python framework for holistic, reproducible, and transparent evaluation of LLMs and multimodal models across dozens of scenarios covering accuracy, robustness, efficiency, bias, and safety.
- [LiveBench](https://github.com/livebench/livebench) 🆓 - Contamination-free LLM benchmark (ICLR 2025 Spotlight) that releases new questions monthly from recent sources across 18 tasks in math, coding, and reasoning, scored with objective verifiable answers instead of LLM judges.
- [SWE-bench](https://github.com/princeton-nlp/SWE-bench) - Benchmark for evaluating LLMs on real software engineering tasks, including test fixes.
- [HumanEval](https://github.com/openai/human-eval) - Evaluating large language models trained on code.
- [WebArena](https://github.com/web-arena-x/webarena) - Self-hostable web environment for building and evaluating autonomous agents on realistic, multi-site tasks.
- [OSWorld](https://github.com/xlang-ai/OSWorld) 🆓 - NeurIPS 2024 benchmark for evaluating multimodal AI agents on open-ended tasks in real computer environments, supporting VMware, Docker, and AWS virtualization.
- [tau-bench](https://github.com/sierra-research/tau-bench) - Benchmark for evaluating tool-using language agents through dynamic conversations with simulated users and domain-specific APIs.
- [AgentBench](https://github.com/THUDM/AgentBench) 🆓 - ICLR 2024 benchmark for evaluating LLMs as autonomous agents across eight environments including OS, database, web browsing, and game tasks.

## Related Awesome Lists

- [awesome-test-automation](https://github.com/atinfo/awesome-test-automation) - General test automation across languages.
- [awesome-testing-tools](https://github.com/ZoranPandovski/awesome-testing-tools) - General testing tools.
- [awesome-ai-agent-testing](https://github.com/chaosync-org/awesome-ai-agent-testing) - Testing AI agents themselves.
- [awesome-ai-pentest](https://github.com/insidetrust/awesome-ai-pentest) - AI-assisted penetration testing.
- [awesome-llm-security](https://github.com/corca-ai/awesome-llm-security) - LLM security tools and resources.
- [awesome-mutation-testing](https://github.com/theofidry/awesome-mutation-testing) - Mutation testing resources.

## Contributing

Contributions are welcome. Please read the [contribution guidelines](contributing.md) before opening a pull request.
