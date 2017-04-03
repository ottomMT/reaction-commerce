# Reaction Commerce configuration for Triton

This repo is setup to run Reaction Commerce, MongoDB, and Nginx as a reverse
proxy. Use the `docker-compose.yml` file for a local setup, and `production.yml`
for production.

Before deployment tweak the container labels & network aliases if applicable,
and the `REACTION_EMAIL`, `REACTION_USER` & `REACTION_AUTH` env variables. If
you modify the CNS container labels you will also need to update the Nginx
configuration.

When the reaction commerce container first starts, it logs a url+token that you
need to login for the first time.
