+++
title = "How we work"
description = "The tools, formats and archives behind a Viten Hub study — for technical teams and researchers who want to know what is under the hood."
+++

# How we work

This page is for technical teams and researchers who want to know what is under the hood. Everything we use is open source and open standard, so nothing you receive depends on Viten Hub continuing to exist.

## The code

- **Python.** The analysis is written as plain, documented Python scripts. When a method is worth reusing on its own, we package it as a Python library that others can install and reuse.
- **Tests.** The code comes with automated tests, so a result that stops reproducing is caught straight away.
- **Pinned environments.** Every software dependency is fixed to an exact version, and the study can also run inside a container, so it gives the same result on a laptop, a server or the cloud — today and in years to come.

## The online report

The scripts are rendered as a [Jupyter Book](https://jupyterbook.org): a website that shows the method, code, figures and results together, with the deviations from the original study and the limitations spelled out. Readers need only a web browser.

## Archiving and citation

- The code lives in a **GitHub** repository, and each release is archived on **[Zenodo](https://zenodo.org)** with its own DOI, so it can be cited like a paper.
- On each release, the code is also saved to **[Software Heritage](https://www.softwareheritage.org)**, the universal archive of source code, and the online report to the **[Internet Archive](https://web.archive.org)**, so it stays readable even if a link breaks.

## The findable record

Each study's claim, method, result, verdict and limitations are published on the open **[Science Live](https://sciencelive4all.org)** platform as **nanopublications**: small, machine-readable statements, each with a permanent identifier and a named author. We follow the **[FORRT](https://forrt.org)** framework for replication and reproduction studies, which records:

- what the original study claimed
- what we did differently
- what held, what didn't, and within which limits

Because the record is open and machine-readable, it can be searched by people and by AI assistants. It stays public and is not locked inside a Viten Hub system.

## AI tools {#ai-tools}

We build **[MCP](https://modelcontextprotocol.io) servers**. MCP (Model Context Protocol) is the open standard that lets AI assistants such as Claude or ChatGPT use external tools and data sources.

- **[Replication Radar](https://doi.org/10.5281/zenodo.21850976)** searches the [OpenAIRE Graph](https://graph.openaire.eu) of publications, software and data. It shows which papers have already been replicated, what was found, and which software and data a paper relies on. It won Theme B: Build at the [OpenAIRE AI Hackathon 2026](https://innovation.openaire.eu/component/content/article/openaire-ai-hackathon.html).
- **[FORRT Research MCP](https://doi.org/10.5281/zenodo.22869401)** lets an AI assistant search past replication studies on Science Live and help write up new ones.

Both are open source, installable from PyPI, and listed in the official MCP Registry.

## Get in touch

Questions about any of this? Email **contact@vitenhub.no**.
