# DBBS Claude Code workshop data

Two small public datasets for the hands-on part of the DBBS Claude Code workshop at Washington University School of Medicine. Pick the one closest to your field.

| Folder | Data | Size |
|---|---|---|
| `airway-rnaseq/` | Bulk RNA-seq of human airway smooth muscle cells treated with dexamethasone, albuterol, or both. 4 donors, 16 samples, gene counts. | 6 MB |
| `moving-pictures-16s/` | 16S rRNA amplicon data from the gut, palms and tongue of two people. 34 samples, 770 sequence variants. | 0.3 MB |

Each folder has a `README.txt` that describes every file, where it came from, and what to know before you analyze it.

## Workshop pages

- [Workshop guide](https://claude.ai/artifact/WRifNQs15PVYCqwgS8SYXR): Claude Code features with short exercises, and the steps for the data project.
- [Terminal cheat sheet](https://claude.ai/artifact/DATRJWZRb4dNvoe6wobtJj): the few terminal commands you need to find a folder and start Claude Code.
- [Git and GitHub cheat sheet](https://claude.ai/artifact/Bek9aLSPmZD8Fkghfk6hFY): what git and GitHub do when Claude Code manages them, and what to ask Claude.
- [Project wheel](https://claude.ai/artifact/JjtCTRf3nRBpPtYwKDoAZ8): spin for a one-day data project in genomics or microbiology.
- [Software project wheel](https://claude.ai/artifact/PeUu4yiXDVj2YJy7LRjV3p): spin for a one-day scientific software project to build.
- [Airway RNA-seq results explorer](https://claude.ai/artifact/8eQrrHBAyDJjgvKVRMfovU): interactive reference analysis of the airway data, with a volcano plot, any gene across all 16 samples, PCA and a results table.
- [Moving Pictures 16S results explorer](https://claude.ai/artifact/CfS48EWPE4ASCTjJ9u3ACJ): interactive reference analysis of the microbiome data, with composition, diversity, ordination and genus comparisons between body sites.
- [Advanced module](https://claude.ai/artifact/GCeakGrgaBtDPPkbkR4rZA): build a data validator skill, build a skill for your computing cluster, and review the PyDESeq2 source code with Claude. The `validation-challenge/` folder holds its data.

## Getting the files

You need a copy of this repository on your computer. Choose one of these three ways.

### Option 1: ask Claude Code to get it

Start Claude Code in your workshop folder and type:

```
Use git clone to copy https://github.com/shandley/dbbs-claude-code-workshop into a folder called data/raw here.
```

Claude needs `git` for this. If `git` is missing, Claude will tell you; use Option 3 instead.

### Option 2: clone it yourself

In a terminal, from your workshop folder:

```
git clone https://github.com/shandley/dbbs-claude-code-workshop data/raw
```

This creates `data/raw/` containing both dataset folders. On a Mac without `git`, macOS offers to install the developer tools the first time you run it; accept, wait for the install, then run the command again. On Windows, install Git for Windows from https://git-scm.com/downloads/win first.

### Option 3: download a zip (no git needed)

1. Open https://github.com/shandley/dbbs-claude-code-workshop in your browser.
2. Click the green **Code** button, then **Download ZIP**.
3. Unzip the file and move its contents into `data/raw/` in your workshop folder. You can ask Claude to do this step: "Unzip ~/Downloads/dbbs-claude-code-workshop-main.zip into data/raw."

You do not need a GitHub account, a login, or the GitHub `gh` tool for any of these. If you are asked for a GitHub username or password, the address was mistyped; copy it again from this page.

## Check that it worked

Your workshop folder should look like this:

```
dbbs-workshop/
  data/
    raw/
      airway-rnaseq/
      moving-pictures-16s/
      README.md
```

## Sources

Both datasets are public. If you use them beyond the workshop, cite the original studies:

- Himes BE, Jiang X, Wagner P, et al. RNA-Seq transcriptome profiling identifies CRISPLD2 as a glucocorticoid responsive gene that modulates cytokine function in airway smooth muscle cells. PLoS One. 2014;9(6):e99625. https://doi.org/10.1371/journal.pone.0099625 (GEO GSE52778)
- Caporaso JG, Lauber CL, Costello EK, et al. Moving pictures of the human microbiome. Genome Biology. 2011;12(5):R50. https://doi.org/10.1186/gb-2011-12-5-r50 (subset from the QIIME 2 Moving Pictures tutorial)
