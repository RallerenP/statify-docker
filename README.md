# Statify Docker

Build and compose files to run the 'Statify' project.

# Configuration

## .env

``GIT_BRANCH`` - Branch to checkout when building statify project.

``SECRET`` - Secret code to enable admin access for logged in user. Make this complex.

``BACKEND_PORT`` *optional* - Public port to access the backend api. Default: 3000

``FRONTEND_PORT`` *optional* - Public port to access the frontend. Default: 5000

## .env.frontend

This file will be mounted into the frontend container.

``VITE_BACKEND_URL`` - URL to access the API.

## Firebase Service Account

Generate the service account key, and place it in a file called ``firebaseServiceAccount.json`` in the root.
