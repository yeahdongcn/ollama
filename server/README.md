# Server

🙊

## Installation

If using Apple silicon, you need a Python version that supports arm64:

```bash
wget https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-MacOSX-arm64.sh
bash Miniforge3-MacOSX-arm64.sh
```

Get the dependencies:

```bash
pip install llama-cpp-python
pip install -r requirements.txt
```

## Running

Put your model in `models/` and run:

```bash
python server.py
```

## API

### `POST /generate`

model: `string` - The name of the model to use in the `models` folder.
prompt: `string` - The prompt to use.