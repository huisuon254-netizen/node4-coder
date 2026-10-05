# NATION coder node

OpenHands-based coder engine. deploy_roles.py pushes the code and installs deps.
The codespace intentionally ships no .devcontainer/devcontainer.json: this
Codespaces setup resolves any devcontainer to an Alpine/musl base, where the
ollama binary cannot run (glibc fcntl64 is missing). With no devcontainer the
default Ubuntu 24.04 image is used, matching node1.
