# TRWM Explained

## Introduction

TRWM (Technique Results Weaknesses Mitigations) is a systematic approach for capturing the details of a digital forensic technique *and* then enumerating over its potential weaknesses and mitigations.

It is supported by TRWM Helper Workbooks (which are Google Sheets workbooks).

A class exercise that works through the process is provided in the [Class Exercises](../class-exercises/README.md) section. Further examples are provided in links [below](#techniques-currently-mapped-using-trwm).

This approach is systematic, thorough, and has the advantage that the resulting worksheet can be programatically turned into JSON code ready to be added to the repository (see the experimental code `trwm2json.py`). 

## Process Overview

The process was created to have a systematic approach to enumerating weaknesses for a technique to try and improve completeness. Inspired by approaches such as STRIDE, and realising that we already had ASTM error classes, it was possible to construct a workflow that allows these error classes to be used as prompts, along with the expected output or results of a forensic technique to make the process more thorough.

An overview of the steps are as follows (with a detailed work-through in the [Class Exercises](../class-exercises/README.md) section.

* View the latest TRWM Helper worksheet (listed [below](#latest-version)).
* This Google Workbook will be read only, but you can use the menu option `File->Make a copy`, to create your own version that will be editable.
* Work through the numbered worksheets, starting with a description of the technique, then the results that are the output of the technique. These can be mapped to CASE Ontology classes where possible, or use the 'Potential CASE classes' field to document others. 
* The next worksheets will then automatically prompt for what different types of error could look like for each result type. These will be aggregated on sheet 3b. This compiled list allows you to:
    * check your wording of the weaknesses, in particular that they 'stand alone' in their descriptions and don't rely on being read in the context of the technique. For example, "message not recovered" may be better reworded as "chat message not recovered" to ensure context is preserved in the weakness name.
    * You can also use this page to add references that support the weaknesses identified. 
* The next sheet (4_Mitigations) will auto populate the weaknesses in a new table. This allows mitigations to be considered and identified for each of the weaknesses. Dropdown boxes are provided for existing mitigations in the knowledge base, but note that they are not automatically synchronised from the repository unfortunately so be mindful of the 'last updated' date. You can also add new mitigations here by typing text in the dropdown boxes instead.
* The mitigation summary worksheet (4b) can be used to check wording and provide references for mitigations.
* This completed worksheet can be shared using the menu item `File->Share with others`, and a URL generated so that "Anyone with the link" can view the file. This shared URL can be added to an issue raised in the repository Issue Tracker using the TRWM template.
* Once reviewed, IDs will be issued for the technique if it is new, and any new weaknesses and mitigations. You can then add these IDs to the worksheet ready for implementation.
* A compact summary of all the details is provided at the end, along with three files with "_tsv" prefix. These files can be separately downloaded using the menu item `File->Download->Tab Separated Values (.tsv)`. These can be used in conjunction with the `trwm2json.py` script which will generate JSON files ready to be added to the repository.
* If you haven't already, you can create a fork of the repository, make your changes, and submit a pull request as detailed in the [project readme](https://github.com/SOLVE-IT-DF/solve-it/blob/main/CONTRIBUTING.md#contributing-directly-via-the-code-repo).

## Latest Version

The latest version of the TRWM Helper Worksheet is available below:

* [v2.51](https://docs.google.com/spreadsheets/d/1pu2TXWQXvIeIh6hNHao3n-Svr66FQP-Yze0pAqH4fyA)


## Older Versions

Older versions for reference are linked below:
* [v2.2](https://docs.google.com/spreadsheets/d/1iCbKCQunwdX-urLs-F6Eyv-ZE4N9r7xtRNpDnHXO-6g/edit?usp=sharing)
* [v2.3](https://docs.google.com/spreadsheets/d/19YdHzjUb5PPkiNb2LsGamFuTHtA0h59jB0i_LFhmpX0/edit?usp=sharing)
* [v2.4](https://docs.google.com/spreadsheets/d/1ctI8DzcYjiVg0uFhNpl6OKtRDoKMnw8_ky1gWk_TXWU/edit?usp=sharing)
* [v2.41](https://docs.google.com/spreadsheets/d/1riHTxltuFKWo5zJoLWk70tcZHcv-bydsavEMxqg1TUo/edit?usp=sharing)

## Techniques currently mapped using TRWM

* T1073: Calendar app examination ([worksheet](https://docs.google.com/spreadsheets/d/1BuEC6BZoMSduKWIsfebTjGTULrS2wA3izrawjFvwj0g/edit?usp=sharing))
* T1076: Log file examination  ([worksheet](https://docs.google.com/spreadsheets/d/1Cy4AJcpRU4m9Y0wXRugV3p0dTmdlJO2IA7Bg5BHwjko/edit?usp=sharing))
* T1128: AI companion app examination ([worksheet](https://docs.google.com/spreadsheets/d/1b3WqCrhdfSfCc69LI1e3202Pi6m4ARDoNRvLswqQ_H0/edit?usp=sharing))
  
