# TRWM Explained

## Introduction

TRWM (Technique Results Weaknesses Mitigations) is a systematic approach for capturing the details of a digital forensic technique *and* then enumerating over its potential weaknesses and mitigations.

It was orignally supported by TRWM Helper Workbooks (Google Sheets workbooks) but now is best conducted using a prototype webapp (see below). 

A class exercise that works through the process is provided in the [Class Exercises](../class-exercises/README.md) section. Further examples are provided in links [below](#techniques-currently-mapped-using-trwm).

This approach is systematic, thorough, and has the advantage that the resulting worksheet can be programatically turned into JSON code ready to be added to the repository.

## Process Overview

The process was created to have a systematic approach to enumerating weaknesses for a technique to try and improve completeness. Inspired by approaches such as STRIDE, and realising that we already had ASTM error classes, it was possible to construct a workflow that allows these error classes to be used as prompts, along with the expected output or results of a forensic technique to make the process more thorough.

An overview of the steps are as follows (with a detailed work-through in the [Class Exercises](../class-exercises/README.md) section.


## Latest Version

The latest version of the prototype TRWM helper web app is available below:

https://trwm.hargs.co.uk

<img width="1382" height="622" alt="image" src="https://github.com/user-attachments/assets/c7ecfe6e-441b-4437-a035-7648fb2fb21f" />


## Older Versions

Older versions used Google Workbooks - for reference are linked below:
* [v2.51](https://docs.google.com/spreadsheets/d/1pu2TXWQXvIeIh6hNHao3n-Svr66FQP-Yze0pAqH4fyA)
* [v2.2](https://docs.google.com/spreadsheets/d/1iCbKCQunwdX-urLs-F6Eyv-ZE4N9r7xtRNpDnHXO-6g/edit?usp=sharing)
* [v2.3](https://docs.google.com/spreadsheets/d/19YdHzjUb5PPkiNb2LsGamFuTHtA0h59jB0i_LFhmpX0/edit?usp=sharing)
* [v2.4](https://docs.google.com/spreadsheets/d/1ctI8DzcYjiVg0uFhNpl6OKtRDoKMnw8_ky1gWk_TXWU/edit?usp=sharing)
* [v2.41](https://docs.google.com/spreadsheets/d/1riHTxltuFKWo5zJoLWk70tcZHcv-bydsavEMxqg1TUo/edit?usp=sharing)

## Techniques currently mapped using TRWM

* T1073: Calendar app examination ([worksheet](https://docs.google.com/spreadsheets/d/1BuEC6BZoMSduKWIsfebTjGTULrS2wA3izrawjFvwj0g/edit?usp=sharing))
* T1076: Log file examination  ([worksheet](https://docs.google.com/spreadsheets/d/1Cy4AJcpRU4m9Y0wXRugV3p0dTmdlJO2IA7Bg5BHwjko/edit?usp=sharing))
* T1128: AI companion app examination ([worksheet](https://docs.google.com/spreadsheets/d/1b3WqCrhdfSfCc69LI1e3202Pi6m4ARDoNRvLswqQ_H0/edit?usp=sharing))
  
