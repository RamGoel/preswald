---
title: "preswald run"
icon: octicons/code-24
description: "Launch a local development server for your data app."
---

# `preswald run <file_name>`

The `preswald run` command launches a local development server for your application, enabling you to test and interact with your app in a browser.

## Arguments

- **`file_name` (str):**  
  The path to the Python script that contains your application code. This is the script the development server will execute.

## Options

- **`port` (int):**  
  The port on which to run the Preswald server. Default is 8501
- **`log-level` (str):**  
  The log level for the Preswald server. Options are DEBUG, INFO, WARNING, ERROR, CRITICAL. Default is INFO
- **`disable-new-tab` (bool):**  
  Flag which controls whether or not a new browser window pops up to show the rendered data app. Default is false, which means that a new window will pop up.


---

## Example Usage

To launch the development server for your app:

```bash
preswald run hello.py
```

or

```bash
preswald run hello.py --port 8504 --log-level DEBUG --disable-new-tab
```

After running the command, your application will be available locally at:

```plaintext
http://localhost:8501
```

## Detailed Explanation

### 1. **Launching the Server**

When you run the command, `preswald` starts a local development server using the specified Python script. This allows you to quickly preview and debug your app in a controlled environment.

### 2. **Supported Script Format**

Any Python file containing valid application logic can be used.

### 3. **Localhost Access**

The app is hosted on `localhost`, which is a local server accessible only from your machine. Use the provided URL to interact with your app through a browser.

### 4. **Stopping the Server**

To stop the server, press `Ctrl+C` in the terminal where the command is running.

### 5. **Error Handling**

If the script cannot be executed (e.g., due to missing dependencies or syntax errors), `preswald` will provide helpful error messages to guide you.

---

Use the `preswald run` command to test, iterate, and debug your app effortlessly in a local environment.