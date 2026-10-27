# SOAI Architecture Overview

This document describes the high-level architecture of the SOAI Digital Self system.

## Core Architecture

```mermaid
flowchart TD

    USER["You / User"]
    INBOX["Digital Self Inbox<br/>Unified Input"]
    ROUTER["Master Router<br/>Routing Agent"]
    COG["Cognitive Recorder<br/>Cognitive Data Recorder"]
    EMB["Embodied Recorder<br/>Embodied Data Recorder"]
    DS["DIGITAL_SELF"]

    USER --> INBOX
    INBOX --> ROUTER

    ROUTER --> COG
    ROUTER --> EMB

    COG --> DS
    EMB --> DS
