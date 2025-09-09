# Critical AI Literacy in Practice

This repository contains research materials and documentation for the project "Critical AI Literacy in Practice: Lessons from Current DH Projects". The research examines how digital humanities scholars can engage critically with AI tools while maintaining scholarly rigor and ethical standards.

[![GitHub issues](https://img.shields.io/github/issues/maehr/critical-ai-literacy-in-practice.svg)](https://github.com/maehr/critical-ai-literacy-in-practice/issues)
[![GitHub forks](https://img.shields.io/github/forks/maehr/critical-ai-literacy-in-practice.svg)](https://github.com/maehr/critical-ai-literacy-in-practice/network)
[![GitHub stars](https://img.shields.io/github/stars/maehr/critical-ai-literacy-in-practice.svg)](https://github.com/maehr/critical-ai-literacy-in-practice/stargazers)
[![Code license](https://img.shields.io/github/license/maehr/critical-ai-literacy-in-practice.svg)](https://github.com/maehr/critical-ai-literacy-in-practice/blob/main/LICENSE-AGPL.md)
[![Data license](https://img.shields.io/github/license/maehr/critical-ai-literacy-in-practice.svg)](https://github.com/maehr/critical-ai-literacy-in-practice/blob/main/LICENSE-CCBY.md)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.17086256.svg)](https://doi.org/10.5281/zenodo.17086256)

## About the Project

This research explores critical AI literacy in digital humanities practice through case studies from Swiss institutions. We demonstrate how scholars can engage with AI tools responsibly while maintaining academic integrity and ethical standards.

### Key Research Questions

- How can digital humanities scholars develop critical AI literacy?
- What frameworks guide responsible AI implementation in research?
- How do current DH projects in Switzerland use AI tools ethically?
- What lessons can we learn from existing practices?

### Core Findings

- **AI is pervasive** in academic research and requires critical engagement
- **Historical understanding** of AI development provides essential context
- **Critical AI literacy frameworks** can guide responsible implementation
- **Swiss DH projects** demonstrate practical approaches to ethical AI use

## Critical AI Literacy Framework

Our research identifies six key components of critical AI literacy for digital humanities scholars:

### 1. Technical Literacy

Understanding how AI systems work, their capabilities and limitations, particularly large language models and their training processes.

### 2. Epistemological Awareness

Questioning what counts as knowledge and how AI shapes knowledge production in scholarly research.

### 3. Ethical Evaluation

Considering consent, privacy, transparency, and accountability in AI-assisted research workflows.

### 4. Social Impact Assessment

Examining power structures, equity issues, and broader implications of AI adoption in academia.

### 5. Practical Application

Developing workflows that maintain scholarly rigor while leveraging AI capabilities effectively.

### 6. Continuous Learning

Staying informed as AI technology evolves rapidly and adapting practices accordingly.

## Swiss Digital Humanities Projects Using AI

This research documents several innovative approaches to AI integration in Swiss DH projects:

### Re-Experiencing History with AI (University of Zurich)

The AIncient Studies Lab has developed an interactive platform for generating historically grounded visualizations of Classical antiquity using fine-tuned image and video generation models.

### Mini-Muse: Cultural Archive Access (SUPSI & ETH Library)

A pilot project exploring NLP and data visualization for exploratory access to digitized historical publications in the E-Periodica archive.

### Alt Text Generation (Stadt.Geschichte.Basel, University of Basel)

An open-source pipeline that enhances Dublin Core metadata by generating WCAG-compliant alt texts for historical sources and objects.

### Humanities Data Benchmark (RISE, University of Basel)

An open benchmark suite testing large language and multimodal models on humanities-relevant visual tasks, providing public leaderboards for model performance.

## Educational Initiatives

### University of Bern: Decoding Inequality

A critical examination of AI systems with focus on inequality and bias issues.

### University of Zurich: ChatGPT and Beyond

Interdisciplinary approaches to AI literacy combining practical skills with critical analysis.

## Repository Structure

The structure of this repository follows best practices for open research:

- `presentation/`: RevealJS presentation materials and slides
- `documentation/`: Additional research documentation
- `analysis/`: Research analysis scripts and notebooks
- `data/`: Research data and findings
- `src/`: Source code for tools and utilities

## Presentation

This repository includes a comprehensive presentation on Critical AI Literacy in Practice. The presentation covers:

- Historical context of AI development from Turing to modern LLMs
- Critical AI literacy frameworks for digital humanities
- Case studies from Swiss institutions
- Practical approaches to responsible AI implementation

To view the presentation locally:

```bash
# Preview the presentation
cd presentation
quarto preview
```

## Getting Started

### For Most Users: Reproducible Setup with GitHub Codespaces

1. **[Use this template](https://github.com/new?template_name=open-research-data-template&template_owner=maehr)** for your project in a new repository on your GitHub account.

   <div align="center">
     <img src=".github/docs/assets/img_use.png" alt="Use the repository" style="width: 540px; margin: 1em 0;" />
   </div>

2. Click the green **`<> Code`** button at the top right of this repository.

3. Select the **“Codespaces”** tab and click **“Create codespace on `main`”**.
   GitHub will now build a container that includes:
   - ✅ Node.js (via `npm`)
   - ✅ Python with `uv`
   - ✅ R with `renv`
   - ✅ Quarto

   <div align="center">
     <img src=".github/docs/assets/img_codespace.png" alt="Create Codespace" style="width: 540px; margin: 1em 0;" />
   </div>

4. Once the Codespace is ready, open a terminal and preview the documentation:

   ```bash
   uv run quarto preview
   ```

   <div align="center">
     <img src=".github/docs/assets/img_terminal.png" alt="Terminal window showing command" style="width: 540px; margin: 1em 0;" />
   </div>

> **Note:** All dependencies (Node.js, Python, R, Quarto) are pre-installed in the Codespace.

<details>
<summary>👩‍💻 <strong>Advanced</strong> Local Installation</summary>

#### Prerequisites

- [Node.js](https://nodejs.org/en/download/)
- [R](https://cran.r-project.org/) and Rtools (on Windows)
- [uv (Python manager)](https://github.com/astral-sh/uv#installation)
- [Quarto](https://quarto.org/docs/get-started/)

> _Note: `uv` installs and manages the correct Python version automatically._

#### Local Setup Steps

```bash
# 1. Install Node.js dependencies
npm install
npm run prepare

# 2. Setup Python environment
uv sync

# 3. Setup R environment
Rscript -e 'install.packages("renv"); renv::restore()'

# 4. Preview documentation
uv run quarto preview
```

</details>

## Project Setup Checklist (for all users)

After creating your project from this template (either via Codespaces or local setup), complete the following steps to customize and finalize your project:

- [ ] **Enable GitHub Security Alerts**: Go to your repository's "Security" tab on GitHub and enable security alerts.
- [ ] **Protect the Main Branch**: In your repository settings on GitHub (under "Branches"), protect your `main` branch.
- [ ] **Update Project Details**: Replace placeholders like `FULLNAME`, `USERNAME`, `REPO_NAME`, `SHORT_DESCRIPTION`, and `[INSERT CONTACT METHOD]` in `.github/ISSUE_TEMPLATE/config.yml`, `_brand.yml`, `CODE_OF_CONDUCT.md`, `package.json`, `README.template.md`, and `SECURITY.md`.
- [ ] **Set Up Zenodo Integration**: Follow the [Zenodo guide](https://docs.github.com/en/repositories/archiving-a-github-repository/referencing-and-citing-content) to connect your repository to Zenodo for long-term archiving and to get a DOI.
- [ ] **Set Up Zenodo DOI Badge**: Replace `GITHUB_REPO_ID` with `id`from `https://api.github.com/repos/USERNAME/REPO_NAME`. This will automatically update with your Zenodo DOI once you make a release.
- [ ] **Add Zenodo DOI to README**: Once you have your Zenodo DOI, add it to the `README.md` file by replacing `ZENODO_RECORD`.
- [ ] **Add Favicons**: Add favicons to the root directory (see [favicon.io](https://favicon.io/)).
- [ ] **Address TODOs**: Search for `TODO` comments throughout the project files and complete the tasks.
- [ ] **Finalize README**: Delete this `README.md` and rename `README.template.md` to `README.md`.
- [ ] **Format Files**: Run `npm run format` to ensure all files are formatted.
- [ ] **Commit Changes**: Run `npm run commit` to save your changes with a standardized commit message.
- [ ] **Generate Changelog**: Run `npm run changelog` and copy the output into the `CHANGELOG.md` file.
- [ ] **Customize Documentation**: Customize your documentation using [Quarto's features](https://quarto.org/docs/websites/#workflow).
- [ ] **Enable GitHub Pages**: In your repository settings on GitHub (under "Pages"), configure GitHub Pages to publish from the `gh-pages` branch.
- [ ] **Publish Documentation**: Run `quarto publish gh-pages` to publish your documentation website.

**Optional:**

- [ ] **Add Citation File**: Create a `CITATION.CFF` file (see [citation-file-format.github.io](https://citation-file-format.github.io/)).
- [ ] **Add Zenodo Metadata File**: Create a `.zenodo.json` file for Zenodo metadata ([Zenodo developer docs](https://developers.zenodo.org/?python#add-metadata-to-your-github-repository-release)).

## Use

These research materials are openly available under open licenses and can be used for educational and research purposes. If you use this research in your work, please cite as specified in `CITATION.cff`.

The following citation formats are also available through _Zenodo_:

- [BibTeX](https://zenodo.org/record/17086257/export/hx)
- [CSL](https://zenodo.org/record/17086257/export/csl)
- [DataCite](https://zenodo.org/record/17086257/export/dcite4)
- [Dublin Core](https://zenodo.org/record/17086257/export/xd)
- [DCAT](https://zenodo.org/record/17086257/export/dcat)
- [JSON](https://zenodo.org/record/17086257/export/json)
- [JSON-LD](https://zenodo.org/record/17086257/export/schemaorg_jsonld)
- [GeoJSON](https://zenodo.org/record/17086257/export/geojson)
- [MARCXML](https://zenodo.org/record/17086257/export/xm)

_Zenodo_ provides an [API (REST & OAI-PMH)](https://developers.zenodo.org/) to access the data. For example, the following command will return the metadata for the most recent version:

```bash
curl -i https://zenodo.org/api/records/17086257
```

## Support

This project is maintained by [@maehr](https://github.com/maehr). Please understand that we can't provide individual support via email. We also believe that help is much more valuable when it's shared publicly, so more people can benefit from it.

| Type                                   | Platforms                                                                                   |
| -------------------------------------- | ------------------------------------------------------------------------------------------- |
| 🚨 **Bug Reports**                     | [GitHub Issue Tracker](https://github.com/maehr/critical-ai-literacy-in-practice/issues)    |
| 📊 **Report bad data**                 | [GitHub Issue Tracker](https://github.com/maehr/critical-ai-literacy-in-practice/issues)    |
| 📚 **Docs Issue**                      | [GitHub Issue Tracker](https://github.com/maehr/critical-ai-literacy-in-practice/issues)    |
| 🎁 **Feature Requests**                | [GitHub Issue Tracker](https://github.com/maehr/critical-ai-literacy-in-practice/issues)    |
| 🛡 **Report a security vulnerability** | See [SECURITY.md](SECURITY.md)                                                              |
| 💬 **General Questions**               | [GitHub Discussions](https://github.com/maehr/critical-ai-literacy-in-practice/discussions) |

## Roadmap

No changes are currently planned.

## Contributing

All contributions to this repository are welcome! If you find errors or problems with the data, or if you want to add new data or features, please open an issue or pull request. Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct and the process for submitting pull requests.

## Versioning

We use [SemVer](http://semver.org/) for versioning. The available versions are listed in the [tags on this repository](https://github.com/maehr/critical-ai-literacy-in-practice/tags).

## Authors and acknowledgment

- **Moritz Mähr** - _Initial work_ - [maehr](https://github.com/maehr)

See also the list of [contributors](https://github.com/maehr/critical-ai-literacy-in-practice/graphs/contributors) who contributed to this project.

## License

The data in this repository is released under the Creative Commons Attribution 4.0 International (CC BY 4.0) License - see the [LICENSE-CCBY](LICENSE-CCBY.md) file for details. By using this data, you agree to give appropriate credit to the original author(s) and to indicate if any modifications have been made.

The code in this repository is released under the GNU Affero General Public License v3.0 - see the [LICENSE-AGPL](LICENSE-AGPL.md) file for details. By using this code, you agree to make any modifications available under the same license.
