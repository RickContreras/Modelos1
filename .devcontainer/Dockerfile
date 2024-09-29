# Usar la imagen base de Python 3.12.5
FROM mcr.microsoft.com/vscode/devcontainers/python:3.12

# Establecer el directorio de trabajo
WORKDIR /workspace

# Copiar el archivo de requisitos
COPY requirements.txt /workspace/requirements.txt

# Instalar las dependencias
RUN pip install --upgrade pip && \
    pip install -r /workspace/requirements.txt

# Exponer el puerto para Jupyter Notebook
EXPOSE 8888

# Comando para iniciar Jupyter Notebook
CMD ["jupyter", "notebook", "--ip=0.0.0.0", "--no-browser", "--allow-root"]