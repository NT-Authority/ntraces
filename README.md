# NTRACES

NTRACES aims to collect as many stack traces as possible for different Windows behaviors, across multiple Windows versions. For example, a stack trace for `NTFS Cached File Reads`.

## Goal

The goal is to give you and your AI agent a **starting point**. If you want to understand the flow of a particular piece of functionality, look at its traces and start reading the code at those locations, following the calls forward or backward as you like.

The traces can also be fed to an AI agent as context when you ask it to reverse engineer a specific Windows feature.

## How traces are made

1. Write a small test program that triggers the behavior.
2. Capture a stack trace with your preferred method (WinDbg, Sysmon, etc.).
3. Submit the trace.

## Current state and plans

Traces are currently stored as plain text files. This is a proof of concept. I plan to move to a structured format and build:

- A custom renderer for viewing traces more comfortably
- A search engine for searching across all traces
- A Trace Diff Tool to compare functionality between multiple windows versions
- Go beyond stack traces, since they miss important context

I believe many of today's problems have become data problems: the more data we have in a problem space, the better we can do, and the better our AI agents can do too. :D

> **Status:** This project is in its very early stages. There is only one trace so far, but I wanted to publish the idea anyway.