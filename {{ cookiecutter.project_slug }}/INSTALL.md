# INSTALLATION

## Conda environment

You must install anaconda or mamba first.

Then you can create the environment localy with the makefile using the command :

```bash
make create_conda_env
```

And activate it with :

```bash
conda activate ./.conda
```

> To remove the long prefix in your shell prompt, modify the env_prompt setting in your .condarc file:
> 
> ```bash
> conda config --set env_prompt '({name})'
> ```

## Pip environment

You can create the environment localy with venv :

```bash
python -m venv ./.venv
```

Activate it with :

```bash
source ./.venv/bin/activate
```

And install requirements :

```bash
pip install -r requirements.txt
```

## Export your environment

### Anaconda

To export your environment, use the command :

```bash
conda env export --no-builds > environment.yml
```

### Pip

To export your environment, use the command :

```bash
pip freeze > requirements.txt
```

> Can be done inside an anaconda environment.