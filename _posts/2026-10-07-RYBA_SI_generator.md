---
layout: post
title: RYBA can now prepare your computational Supporting Information
subtitle: From ORCA outputs to editable Word tables
thumbnail-img: ../assets/projects/RYBA/LOGO.png
tags: [RYBA, ORCA, software, computational chemistry, tutorial, supporting information]
author: Tomáš
---

Finished calculations still need to become something a reader can inspect: molecular structures, coordinates, energies and a clear description of the methods. Copying these from individual output files into a document takes time and makes transcription errors rather easy. I added the Supporting Information generator to RYBA to handle this part of the work.

You can find the program on the [download page](https://nevesely.science/downloads/). For an introduction to its other tools, see the [earlier RYBA post](https://nevesely.science/2026-09-04-RYBA_introduction/).

## From output files to a Word document

The basic workflow is straightforward:

1. Load your ORCA output files into RYBA.
2. Open the Reports workspace, choose **Supporting information**, and add the active calculation or all loaded results.
3. Rename and arrange the molecular records, select the properties you want to report, and review the preview and scientific checks.
4. Click **Export Word** to obtain an editable `.docx` document.

Each molecular record can contain a structure image and a table with the element and Cartesian x, y and z coordinates. Optional properties include electronic energy, enthalpy, the selected Gibbs free energy, zero-point energy, charge, multiplicity and imaginary frequencies. A molecular summary table brings the selected values together in one place.

For excited-state calculations, you can also export a separate table of excitation energies, wavelengths and oscillator strengths. Choose how many states to include and whether to show singlets, triplets or both, where those assignments are available in the output. Selected GOAT conformers and their ensemble summary can be included as well.

## The details that matter for reproducibility

**General methodology is written once**, with separate profiles for different calculation protocols. Detected methods, basis sets, solvent models and ORCA versions become editable text, rather than being repeated above every coordinate table.

The molecular records also allow independent sources for geometry, electronic energy, thermochemistry, frequencies and excited states. This accommodates the common workflow of optimizing at one level and calculating a higher-level single-point energy afterward. Combined electronic and thermal contributions are labelled explicitly as composite values.

The energy choices distinguish **ORCA's printed Gibbs free energy**, **Grimme qRRHO** and **Cramer–Truhlar frequency-floor corrections**. Correction settings and standard-state conventions can be reported. Relative-energy comparisons are guarded against incompatible compositions, levels of theory, temperatures and correction conventions. Missing data remain visibly missing; an unavailable oscillator strength is not turned into zero.

The export provides an organized starting point for the computational section of a paper. You can still edit its prose, tables and images in Word. All processing happens locally.
