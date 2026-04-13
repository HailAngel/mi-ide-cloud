FROM mcr.microsoft.com/devcontainers/python:3.11

# Mantenemos tus herramientas (htop, tree) y sumamos postgresql
RUN apt-get update && apt-get install -y \
    htop \
    tree \
    postgresql \
    postgresql-contrib \
    && apt-get clean

# Esto asegura que el sistema esté listo para usar la base de datos
ENV PATH="/usr/lib/postgresql/13/bin:$PATH"
