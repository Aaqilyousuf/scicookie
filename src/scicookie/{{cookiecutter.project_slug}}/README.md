{% set is_open_source = cookiecutter.project_license != 'Other' -%}
# {{ cookiecutter.project_name }}

{% if cookiecutter.build_system == "poetry" -%}
[![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
{%- elif cookiecutter.build_system == "flit" -%}
![Flit](https://img.shields.io/badge/Build%20system-Flit-turquoise)
{%- elif cookiecutter.build_system == "mesonpy" -%}
![meson-python](https://img.shields.io/badge/Build%20system-meson_python-indigo)
{%- elif cookiecutter.build_system == "setuptools" -%}
![setuptools](https://img.shields.io/badge/Build%20system-setuptools-teal)
{%- elif cookiecutter.build_system == "pdm" -%}
[![pdm-managed](https://img.shields.io/endpoint?url=https%3A%2F%2Fcdn.jsdelivr.net%2Fgh%2Fpdm-project%2F.github%2Fbadge.json)](https://pdm-project.org)
{%- elif cookiecutter.build_system == "hatch" -%}
[![Hatch](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
{%- elif cookiecutter.build_system == "maturin" -%}
![maturin](https://img.shields.io/badge/Build%20system-maturin-blue)
{%- elif cookiecutter.build_system == "scikit-build-core" -%}
![scikit-build-core](https://img.shields.io/badge/Build%20system-scikit_build_core-orange)
{%- elif cookiecutter.build_system == "pybind11" -%}
![pybind11](https://img.shields.io/badge/Build%20system-pybind11-brown)
{%- elif cookiecutter.build_system == "pixi" -%}
[![Pixi Badge](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/prefix-dev/pixi/main/assets/badge/v0.json&style=flat-square)](https://pixi.sh)
{% endif -%}
{% if cookiecutter.command_line_interface == "Click" -%}
![CLI](https://img.shields.io/badge/CLI-click-violet)
{%- elif cookiecutter.command_line_interface == "Argparse" -%}
![CLI](https://img.shields.io/badge/CLI-argparse-blue)
{% endif -%}
{% if cookiecutter.documentation_engine == "mkdocs" -%}
![Mkdocs](https://img.shields.io/badge/Documentation%20engine-Mkdocs-orange)
{% if cookiecutter.mkdocs_theme == "material" -%}
[![Built with Material for MkDocs](https://img.shields.io/badge/Material_for_MkDocs-526CFE?style=for-the-badge&logo=MaterialForMkDocs&logoColor=white)](https://squidfunk.github.io/mkdocs-material/)
{% endif -%}
{%- elif cookiecutter.documentation_engine == "sphinx(rst)" -%}
![Sphinx](https://img.shields.io/badge/Documentation%20engine-Sphinx-orange?logo=sphinx)
{%- elif cookiecutter.documentation_engine == "sphinx(myst)" -%}
![Sphinx](https://img.shields.io/badge/Documentation%20engine-Sphinx-orange?logo=sphinx)
{%- elif cookiecutter.documentation_engine == "jupyter-book" -%}
[![Jupyter Book Badge](https://jupyterbook.org/badge.svg)]
{%- elif cookiecutter.documentation_engine == "quarto" -%}
![quarto](https://img.shields.io/badge/Documentation%20engine-quarto-turquoise?logo=quarto)
{% endif -%}
{% if cookiecutter.use_conda == "yes" -%}
![Conda](https://img.shields.io/badge/Virtual%20environment-conda-brightgreen?logo=anaconda)
{%- else -%}
![virtualenv](https://img.shields.io/badge/Virtual%20environment-virtualenv-blue)
{% endif -%}
{% if cookiecutter.use_black == "yes" -%}
[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
{%- elif cookiecutter.use_ruff_formatter == "yes" -%}
[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
{%- elif cookiecutter.use_prettier == "yes" -%}
[![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square)](https://github.com/prettier/prettier)
{% endif -%}
{%- if cookiecutter.use_bandit == "yes" -%}
[![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
{% endif -%}
{%- if cookiecutter.use_coverage == "yes" -%}
![coverage](https://img.shields.io/badge/Code%20coverage%20testing-coverage.py-blue)
{% endif -%}
{%- if cookiecutter.use_flake8 == "yes" -%}
![flake8](https://img.shields.io/badge/code%20quality-flake8-blue)
{% endif -%}
{%- if cookiecutter.use_ruff_linter == "yes" -%}
[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
{% endif -%}
{%- if cookiecutter.use_isort == "yes" -%}
[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
{% endif -%}
{%- if cookiecutter.use_vulture == "yes" -%}
![vulture](https://img.shields.io/badge/Find%20unused%20code-vulture-blue)
{% endif -%}
{%- if cookiecutter.use_mccabe == "yes" -%}
![McCabe](https://img.shields.io/badge/Complexity%20checker-McCabe-blue)
{% endif -%}
{%- if cookiecutter.use_mypy == "yes" -%}
![mypy](https://img.shields.io/badge/Static%20typing-mypy-blue)
{% endif -%}
{%- if cookiecutter.use_pytest == "yes" -%}
![pytest](https://img.shields.io/badge/Testing-pytest-cyan?logo=pytest)
{%- elif cookiecutter.use_hypothesis == "yes" -%}
![hypothesis](https://img.shields.io/badge/Testing-hypothesis-maroon)
{% endif -%}
{%- if cookiecutter.use_shellcheck == "yes" -%}
![ShellCheck](https://img.shields.io/badge/Analysis%20of%20shell%20scripts-ShellCheck-brightgreen)
{% endif -%}
{%- if cookiecutter.use_pre_commit == "yes" -%}
[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
{% endif -%}
{%- if cookiecutter.use_containers == 'Docker' -%}
![Docker](https://img.shields.io/badge/Containerization-Docker-blue?logo=docker)
{% endif %}
{%- if cookiecutter.use_makim == "yes" -%}
![Makim](https://img.shields.io/badge/Automation%20task-Makim-blue)
{%- elif cookiecutter.use_make == "yes" -%}
![Make](https://img.shields.io/badge/Automation%20task-Make-blue)
{% endif %}
{%- if cookiecutter.use_github_actions == "yes" -%}
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-CI-blue?logo=githubactions)
{%- elif cookiecutter.use_circleci == "yes" -%}
![CircleCI](https://img.shields.io/badge/CircleCI-CI-blue?logo=circleci&labelColor=grey)
{%- elif cookiecutter.use_azure_pipelines == "yes" -%}
![Azure pipelines](https://img.shields.io/badge/Azure%20Pipelines-CI-blue)
{%- elif cookiecutter.use_gitlab_ci == "yes" -%}
![GitLab CI](https://img.shields.io/badge/GitLab%20CI-CI-orange?logo=gitlab)
{% endif %}

{{ cookiecutter.project_short_description }}

{% if is_open_source -%}

- Software License: {{ cookiecutter.project_license }}
{%- endif %}

- Documentation: {{ cookiecutter.documentation_url }}

{% if cookiecutter.communication_platform != "None" %}
## Communication

Platform: **{{ cookiecutter.communication_platform }}**
Link: {{ cookiecutter.communication_link }}
{% endif -%}

{% if cookiecutter.donate_url %}
## 💝 Support the Project

[![Donate]({{ cookiecutter.donate_url }})]({{ cookiecutter.donate_url }})
{% endif %}

{% if cookiecutter.use_data_ai_libs %}
## 📊 Data / AI Libraries

You have selected the following data science & AI libraries:

{% if cookiecutter.use_altair == "yes" %}
- altair
{% endif %}
{% if cookiecutter.use_beautifulsoup4 == "yes" %}
- beautifulsoup4
{% endif %}
{% if cookiecutter.use_bokeh == "yes" %}
- bokeh
{% endif %}
{% if cookiecutter.use_dash == "yes" %}
- dash
{% endif %}
{% if cookiecutter.use_folium == "yes" %}
- folium
{% endif %}
{% if cookiecutter.use_ibis_framework == "yes" %}
- ibis-framework
{% endif %}
{% if cookiecutter.use_jupyterlab == "yes" %}
- jupyterlab
{% endif %}
{% if cookiecutter.use_langchain == "yes" %}
- langchain
{% endif %}
{% if cookiecutter.use_matplotlib == "yes" %}
- matplotlib
{% endif %}
{% if cookiecutter.use_nltk == "yes" %}
- nltk
{% endif %}
{% if cookiecutter.use_numpy == "yes" %}
- numpy
{% endif %}
{% if cookiecutter.use_openai == "yes" %}
- openai
{% endif %}
{% if cookiecutter.use_pandas == "yes" %}
- pandas
{% endif %}
{% if cookiecutter.use_panel == "yes" %}
- panel
{% endif %}
{% if cookiecutter.use_plotly == "yes" %}
- plotly
{% endif %}
{% if cookiecutter.use_polars == "yes" %}
- polars
{% endif %}
{% if cookiecutter.use_pytorch_cpu == "yes" %}
- pytorch(cpu)
{% endif %}
{% if cookiecutter.use_pytorch_gpu == "yes" %}
- pytorch(gpu)
{% endif %}
{% if cookiecutter.use_quarto_cli == "yes" %}
- quarto-cli
{% endif %}
{% if cookiecutter.use_rago == "yes" %}
- rago
{% endif %}
{% if cookiecutter.use_requests == "yes" %}
- requests
{% endif %}
{% if cookiecutter.use_scikit_learn == "yes" %}
- scikit-learn
{% endif %}
{% if cookiecutter.use_scipy == "yes" %}
- scipy
{% endif %}
{% if cookiecutter.use_scrapy == "yes" %}
- scrapy
{% endif %}
{% if cookiecutter.use_seaborn == "yes" %}
- seaborn
{% endif %}
{% if cookiecutter.use_statsmodels == "yes" %}
- statsmodels
{% endif %}
{% if cookiecutter.use_tensorflow == "yes" %}
- tensorflow
{% endif %}
{% if cookiecutter.use_xgboost == "yes" %}
- xgboost
{% endif %}

{% endif %}

## Features

TBD


## Credits

This package was created with
[scicookie](https://github.com/osl-incubator/scicookie) project template.
