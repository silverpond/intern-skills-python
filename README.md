# Internship Test – **word-meter**

A Silverpond internship is **not** about fetching coffee — you’ll be committing code that ends up in production.
This repository helps *prospective interns* self-assess and practise the core skills we need **before** you start.

---

## Core Skills You Should Already Have

| Skill | What We Expect |
| ----- | -------------- |
| **Python ≥ 3.11** | You’ve built at least one small project and can read/write idiomatic code. A public GitHub portfolio is a big plus. |
| **Python project basics** | You know how to work in an isolated environment (`venv`, `pip`, `poetry`, `uv` or `conda`) and install dependencies from a `pyproject.toml` or `requirements.txt`. |
| **Unix terminal** | Our GPU workstations run **NixOS** (for this test you can use Linux distros like Ubuntu). You should comfortably `ssh` in, list files, move/rename, and edit config. |
| **Git (SSH, not HTTPS)** | Common commands (`clone`, `pull`, `push`, `branch`, `merge`, `rebase`, `checkout`). |
| **Vim/NeoVim** | Even if you prefer VS Code, you *will* end up in Vim via an `ssh` session. Knowing basics (`i`, `:wq`, yanking, searching) avoids the “how do I exit?” meme. |
| **Remote development** | Have an SSH key pair set up locally; add the **public key** to GitHub *and* to our servers when invited. |
| **Password manager** | Use one. Always. |

---

## Your Task – Build & Test **word-meter**

`word-meter` is a tiny clone of Unix `wc`, focused on **word statistics** instead of byte/line counts.

### 1. Fork & Clone

```bash
git clone git@github.com:<your-handle>/intern-word-meter.git
cd intern-word-meter
````

### 2. Setup your Environment

### 3. Implement

* Create the package **`word_meter`**.

* Expose a CLI: `word-meter` (console-script **and** `python -m word_meter`).

* Features to support (minimum):

  | Flag / Command                    | Behaviour                                            |
  | --------------------------------- | ---------------------------------------------------- |
  | `cat file.txt \| word-meter`      | Read **stdin**, output `words={count} unique={count}`. |
  | `--top N`                         | Show the *N* most common words and their counts.     |

* Follow PEP 8, add type hints, docstrings, and logging. Ensure you run a code formatter.

### 4. Tests

* Use **`pytest`** + **`pytest-cov`**.
* Include tests for the CLI
* Provide instructions on how to run pytests as part of your submission


### 6. Create a Pull Request

*Open a PR back onto **your own fork’s** main branch* — we’ll review that link.
Add a short **README update** describing any extras (e.g. `--histogram`).

### 7. Record a Short Video (5–10 min)

* Screen-capture while you run the tool and the tests.
* Explain **why** you structured the code the way you did, how you approached edge-cases, and any trade-offs.
* No fancy editing required — clear audio + visible terminal is enough.

### 8. Submit

Email your Silverpond contact:

```
Subject: Internship – word-meter submission

Body:
• PR link: https://github.com/…
• Video link: https://youtu.be/…
```

---

## What We’re Assessing

| Aspect                      | Looking For                                              |
| --------------------------- | -------------------------------------------------------- |
| **Problem-solving process** | How you break tasks down, research, and iterate.         |
| **Command of tools**        | Git fluency, Python packaging, testing, coverage.        |
| **Communication**           | Clear verbal explanations during the video.              |
| **Code quality**            | Readable, idiomatic, sufficiently documented.            |
| **Tests & automation**      | Meaningful assertions, high coverage, reproducible runs. |

### Not Assessing

* Pixel-perfect video editing.

---

## A Note on ChatGPT & Copilots

LLMs can accelerate coding — *we use them too!*
But your submission **must** demonstrate personal understanding.
In the video, talk through decisions and pitfalls; code pasted without insight is easy to spot and will be rejected.

Good luck — we’re looking forward to your `word-meter`!
