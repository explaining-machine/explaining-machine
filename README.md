# Explaining-Machine
A machine that explains meanings.

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: Are language models seeking the Truth, machine?" \
  | uvx explaining-machine \
    --provider-api-key sk-proj-... \
    --github-token ghp_... 
```

Or, with a local pip installation:
```bash
pip install explaining-machine
```
Set the environment variables:
```bash
export PROVIDER_API_KEY="sk-proj-..."
export GITHUB_TOKEN="ghp_..."
```
Then:
```bash
explaining-machine -a multilogue.txt
```
Or:
```bash
explaining-machine multilogue.txt > response.txt
```
Or:
```bash
explaining-machine -a multilogue.txt > tmp && echo tmp > multilogue.txt
```

Or use it in your Python code:
```Python
# Python
import explaining_machine
```
