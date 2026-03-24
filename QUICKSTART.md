# Guía Rápida de Inicio

## Estado del Proyecto

✅ **Ambiente virtual creado**: `venv/`
✅ **Todas las dependencias instaladas**
✅ **Notebook EDA listo**: `notebooks/01_eda.ipynb`

## Uso Rápido

### 1. Activar el Ambiente Virtual

```bash
# En macOS/Linux
source venv/bin/activate

# En Windows
venv\Scripts\activate
```

Verás `(venv)` al inicio de tu terminal cuando esté activado.

### 2. Iniciar Jupyter Notebook

```bash
jupyter notebook
```

Esto abrirá Jupyter en tu navegador. Navega a `notebooks/01_eda.ipynb`.

### 3. Ejecutar el EDA

Una vez abierto el notebook:
- Ejecuta todas las celdas: Menu → Cell → Run All
- O ejecuta celda por celda: `Shift + Enter`

Las visualizaciones se guardarán automáticamente en `figures/`.

### 4. Desactivar el Ambiente (cuando termines)

```bash
deactivate
```

## Estructura del Proyecto

```
Tarea02/
├── venv/                  ← Ambiente virtual (NO subir a git)
├── data/                  ← Dataset original
├── notebooks/             ← Jupyter notebooks
│   └── 01_eda.ipynb      ← Análisis principal
├── src/utils/             ← Funciones reutilizables
├── figures/               ← Visualizaciones generadas
└── reports/               ← Reportes futuros
```

## Librerías Instaladas

- **Análisis**: pandas, numpy, scipy
- **Visualización**: matplotlib, seaborn, plotly
- **Jupyter**: notebook, ipykernel, ipywidgets

## Solución de Problemas

### Error al activar el ambiente

```bash
# Eliminar y recrear
rm -rf venv
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

### Jupyter no encuentra el kernel

```bash
source venv/bin/activate
python -m ipykernel install --user --name=venv
```

### Puerto ocupado

```bash
# Especificar un puerto diferente
jupyter notebook --port=8889
```

## Próximos Pasos

1. ✅ Ejecutar el notebook completo
2. Revisar las visualizaciones en `figures/`
3. Personalizar el análisis según necesidades
4. Exportar reportes si es necesario

## Notas Importantes

- El dataset contiene información sensible
- Algunos datos están marcados como "CONFIDENCIAL"
- Usar con fines académicos únicamente
- No compartir información confidencial

---

**¿Necesitas ayuda?** Revisa el README.md para más detalles.
