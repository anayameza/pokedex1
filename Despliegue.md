# Despliegue de la Aplicación PokeDex1 en Azure

Este documento detalla el proceso de publicación de la aplicación PokeDex en la nube utilizando Microsoft Azure.

##  Requisitos previos

- Tener una cuenta en Azure (ver `README.md` alli te explico pasp a paso).
- Haber desarrollado localmente la aplicación PokeDex.
- Tener instalado:
  - Git
  - Node.js (si es una app frontend)
  - Azure CLI

## Pasos para el despliegue

### 1. Iniciar sesión en Azure
Ingrese con usuario y contraseña con la cuenta institucional creada

### 2. Crea un static webs apps 
en la barra del buscador escribe `static webs apps` y le das click.

### 3. Crear un grupo de recursos (opcional)
az group create --name pokedex-resource-group --location eastus

### 4. Configurar el despliegue desde GitHub 
az webapp deployment source config --name pokedex-app-demo --resource-group pokedex-resource-group --repo-url https://github.com/tuusuario/repositorio-pokedex --branch main --manual-integration

### 5. Ver la aplicación en línea
https://ashy-plant-02a757a10.6.azurestaticapps.net/ 

## ESTO FUE TODO CON EL Inge_Anaya
