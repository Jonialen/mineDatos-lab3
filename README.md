# mineDatos-lab3

Laboratorio 3 – Modelos de Regresión Lineal  
CC3074 Minería de Datos | UVG Semestre I 2026

## Requisitos

- Python 3.14+
- [uv](https://github.com/astral-sh/uv) (recomendado) o pip

## Instalación

### Con uv
```bash
uv sync
```

### Con pip
```bash
pip install -r requirements.txt
```

## Ejecutar

### Jupyter Notebook (clásico)
```bash
uv run jupyter notebook
# o con pip:
jupyter notebook
```

### JupyterLab
```bash
uv run jupyter lab
# o con pip:
jupyter lab
```

### VS Code
1. Instala la extensión **Jupyter** de Microsoft.
2. Abre `lab3.ipynb`.
3. Selecciona el intérprete: `Ctrl+Shift+P` → *Python: Select Interpreter* → elige `.venv` (uv) o el entorno de pip.

## Uso

Abre `lab3.ipynb` y ejecuta las celdas en orden.  
El dataset debe estar en `data/listings.RData`.
