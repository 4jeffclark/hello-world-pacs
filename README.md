# Hello World APP

Distribution repo for the **Hello World** AgentPlaybookPack — a minimal pack that produces a greeting report for a named recipient.

## Pack

| Pack | Entry |
| --- | --- |
| [hello-world.app/](hello-world.app/) | [`pack.app.yaml`](hello-world.app/pack.app.yaml) |

## Try it

- *Run hello world for Alice.*
- *Run hello world for Bob with a friendly sign-off and welcome banner.*

Report assembly (`Report.md` structure and Inputs Resolved appendix) is agent responsibility; the core skill produces greeting text only.

## APP standard (execution agents)

Read in order from the [APP Standards Workbench](https://github.com/4jeffclark/agent-playbook-pack):

1. [Authoring standard](https://github.com/4jeffclark/agent-playbook-pack/blob/main/standard/app-authoring.md)
2. [Execution guide](https://github.com/4jeffclark/agent-playbook-pack/blob/main/standard/app-execution.md)
3. [Post-run checklist](https://github.com/4jeffclark/agent-playbook-pack/blob/main/standard/post-run-checklist.md)

Then consume this repo's pack manifests and referenced layer artifacts.

## Authors

Validate manifests after changes (from a clone of [agent-playbook-pack](https://github.com/4jeffclark/agent-playbook-pack)):

```bash
pip install pyyaml jsonschema
python /path/to/agent-playbook-pack/standard/validate-manifests.py \
  hello-world.app/pack.app.yaml \
  hello-world.app/layer3-playbooks/hello-world/hello-world.app.yaml
```

## About

Published from the [APP Standards Workbench](https://github.com/4jeffclark/agent-playbook-pack) reference instance.
