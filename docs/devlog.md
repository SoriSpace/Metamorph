# Metamorph — devlog

Una entrada por ticket cerrado.

## 2026-08-14 — META-001 — Levantar Plane en sorilab

**Did:** Plane corriendo en el puerto 8081, accesible por Tailscale

**Learned:** LISTEN_HTTP_PORT publica el puerto al host, SITE_ADDRESS es el interno del contenedor. Son dos cosas distintas y hay que tocar la primera si el 80 esta ocupado

**Trap:** setup.sh v1.4.1 no lee el release de GitHub porque el grep asume un espacio en el JSON. Hay que parchear la linea 60 para usar python3

**Obvious next step:** crear los proyectos en Plane con los identificadores AUTOPSY, MORPH, S3, IAM, ORIBOT, META, RETRO, ALFA
