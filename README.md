# Vale for RISC-V documentation
This repository provides RISC-V specification authors with Vale rulesets that implement RISC-V International's recommended language and style guidelines.

## Introduction
[Vale](https://vale.sh/docs) is a command-line tool that brings code-like linting to prose. RISC-V International uses Vale to implement the rules defined by the Doc-Sig and approved by the TSC.

The rules are outlined in the [Authoring and Editing RISC-V
Specifications](https://github.com/riscv/docs-dev-guide) guide.

## Adding the Vale Workflow

RISC-V International has implemented a reusable Vale workflow th


## Running Vale on a GitHub repository
Follow these steps to add and enable Vale to your GitHub repository.

1. Install [Vale][1] with `brew install vale` (macOS) or `choco install vale` (Windows).
1. Copy the .vale.ini file from this repository to the root of your specification's repository.
1. Copy the vale-using-reusable.yml workflow file from this repository to the .github/workflows directory of you specification's repository.
    * This workflow will be triggered on any pushes or pull requests to your repository.
1. Download the RISC-V Vale rules to your repository locally but no need to add them to Git.
    * open a terminal and change to the root of your extensions repository
    * run the command `vale sync`




[1]: https://vale.sh/
[2]: https://marketplace.visualstudio.com/items?itemName=ChrisChinchilla.vale-vscode