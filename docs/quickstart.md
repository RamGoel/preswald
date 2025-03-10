---
title: "Quickstart"
icon: octicons/zap-24
description: "Get up and running with the Preswald SDK in under 5 minutes"
---

<Steps>

  <Step title="Install the Preswald SDK">

```bash
pip install preswald
```

<Tip>Need the latest version? Upgrade anytime:</Tip>

```bash
pip install --upgrade preswald
```

</Step>

  <Step title="Set Up Your First Project">

Run these commands to bootstrap your first Preswald app:

```bash
preswald init my_project
cd my_project
```

This will create a scaffolded project with the following:

- **`hello.py`**: A starter Python script to get you going.
- **`preswald.toml`**: Your app’s configuration settings.
- **`secrets.toml`**: A secure place for sensitive data.
- **`.gitignore`**: Pre-configured to exclude sensitive files from version control.

</Step>

  <Step title="Write Your First App">

Open `hello.py` and edit it with the following content:

```python
from preswald import text

text("# Welcome to Preswald")
```

#### Run It Locally

Launch your app locally with this command:

```bash
preswald run hello.py
```

Open your browser and navigate to **[http://localhost:8501](http://localhost:8501)**. Your app will be live, ready for you to explore and iterate on.

</Step>

  <Step title="Deploy Your App">

When you're ready to deploy your app, Preswald gives you flexibility:

#### Deploy Locally

If you just want to test your container locally:

```bash
preswald deploy --target local hello.py
```

Or simply:

```bash
preswald deploy hello.py
```

This performs a local "dry run" by building the container locally.

</Step>

</Steps>