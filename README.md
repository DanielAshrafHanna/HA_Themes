# Solace Themes 


Installing this theme adds 1 theme:
- `solace-theme`


## Installation

1. Installation of the themes with HACS.

* Go to HACS -> Overflow memu (3 dots on upper right) -> Custom repositories then paste this link 


2. Add the following code to your `configuration.yaml` file (reboot required).

```yaml
frontend:
  ... # your configuration.
  themes: !include_dir_merge_named themes
  ... # your configuration.
```




## How does the code work

All the **28(!)** themes in [`themes/`](themes/) are **automatically generated** using [`create-themes.py`](create-themes.py) and the information in [`settings-light-dark.yaml`](settings-light-dark.yaml) is passed into [`template.jinja2`](template.jinja2).
The resulting file is [`themes/solace-themes.yaml`](themes/solace-themes.yaml) which contains all variants (different backgrounds and dark/light mode).
