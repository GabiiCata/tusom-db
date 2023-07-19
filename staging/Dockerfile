# Utiliza una imagen base de PostgreSQL
FROM postgres:13.1

# Variables de entorno para configurar la base de datos
ENV POSTGRES_USER postgres
ENV POSTGRES_PASSWORD password
ENV POSTGRES_DB tusomdb

# Copia un archivo SQL con los comandos para inicializar la base de datos
COPY init.sql /docker-entrypoint-initdb.d/

# Expone el puerto de la base de datos (opcional, pero puede ser útil para acceder a la base de datos desde fuera del contenedor)
EXPOSE 5432
