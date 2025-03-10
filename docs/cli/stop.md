---
title: "preswald stop"
icon: octicons/code-24
description: "Stop a deployed app."
---

# `preswald stop`

The `preswald stop` command stops an already deployed app.

Note: `preswald deploy` creates a `.env.structured` in the current directory for Structured Cloud deployments. This is used under the hood to stop Structured deployments.

## Arguments

- **`file_name` (str):**  
  The path to the Python script that contains your application code. This is the script of which app was deployed.

## Options

- **`--target`**: Specifies the deployment target. Options include:
  - `structured`: Structured Cloud. Requires Structured API Key.
  - `gcp`: Google Cloud Platform. Requires GCloud CLI installed.
  - `local` (default): Locally without deploying to the cloud.


## Example Usage

```bash
preswald stop --target structured hello.py
```