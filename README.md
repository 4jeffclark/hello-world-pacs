# Hello World PACS

Distribution repo for the **Hello World** PACS stack — a minimal capability stack that produces a greeting report for a named recipient.

## Pack

| Pack | Entry |
| --- | --- |
| [hello-world.pacs/](hello-world.pacs/) | [`pack.pacs.yaml`](hello-world.pacs/pack.pacs.yaml) |

## Try it

- *Run hello world for Alice.*
- *Run hello world for Bob with a friendly sign-off and welcome banner.*

Report assembly (`Report.md` structure and Inputs Resolved appendix) is agent responsibility; the core skill produces greeting text only.

## PACS standard (execution agents)

Read in order from the [PACS Standards Workbench](https://github.com/4jeffclark/pacs-workbench):

1. [Authoring standard](https://github.com/4jeffclark/pacs-workbench/blob/main/standard/pacs-authoring.md)
2. [Execution guide](https://github.com/4jeffclark/pacs-workbench/blob/main/standard/pacs-execution.md)
3. [Post-run checklist](https://github.com/4jeffclark/pacs-workbench/blob/main/standard/post-run-checklist.md)

Then consume this repo's pack manifests and referenced layer artifacts.

## Authors

Validate manifests after changes (from a clone of [pacs-workbench](https://github.com/4jeffclark/pacs-workbench)):

```bash
pip install pyyaml jsonschema
python /path/to/pacs-workbench/standard/validate-manifests.py \
  hello-world.pacs/pack.pacs.yaml \
  hello-world.pacs/layer3-playbooks/hello-world/hello-world.pacs.yaml
```

## About

Published from the [PACS Standards Workbench](https://github.com/4jeffclark/pacs-workbench) reference instance.
