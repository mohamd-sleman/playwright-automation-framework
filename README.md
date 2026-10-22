# Playwright Automation Framework

A personal learning workspace for practicing UI, API, and AI test automation
with **Playwright**, **Selenium**, **pytest**, and **DeepEval** in Python. Each
numbered folder is a self-contained exercise named after its topic — they are
not meant to import from one another.

## Setup

```bash
python -m venv .venv
source .venv/bin/activate        # Windows: .venv\Scripts\activate
pip install -r requirements.txt
playwright install
```

Some lessons read credentials from a `.env` file (see `07_pom_env_config/.env`
for an example using the public SauceDemo test account).

## Running tests

Each folder is independent, so run pytest from inside it:

```bash
cd 06_page_object_model
pytest
```

## Folder guide

| Folder | Topic |
| --- | --- |
| `01_python_basics/` | Plain Python and pytest practice: conditionals, API-result validation, fixtures/parametrize. |
| `02_api_testing/` | API testing with `requests` against reqres.in (raw scripts + pytest tests). |
| `03_selenium_basics/` | Selenium WebDriver basics: locators, login flows, waits. |
| `04_playwright_basics/` | Playwright sync API basics: page actions, API requests. |
| `05_playwright_assertions_tracing/` | Playwright assertions (`expect`), Inspector, tracing, hybrid UI+API tests. |
| `06_page_object_model/` | Page Object Model with Playwright + pytest fixtures (login, inventory, checkout). |
| `07_pom_env_config/` | POM continued: `.env`-based config, fixtures, checkout page object. |
| `08_api_login_fixtures/` | Fast login via cookie injection, side-menu page object, inventory homework. |
| `09_ai_testing_deepeval/` | LLM answer-relevancy testing with DeepEval (cloud and local Ollama models). |
| `10_rag_and_ai_red_teaming/` | RAG relevancy tests and promptfoo red-teaming configs. |
| `11_llm_tracing_phoenix/` | LLM tracing with Arize Phoenix + OpenInference, trace export to CSV. |
| `12_full_stack_testing/` | Combined API + UI + AI test in one flow. |
| `trace.zip` | Sample Playwright trace, viewable with `playwright show-trace trace.zip`. |

## Notes

- Folders are numbered in course order and named after their content.
- `__pycache__/`, `.pytest_cache/`, `.env`, and generated `traces_*.csv` are
  git-ignored; see `.gitignore`.
