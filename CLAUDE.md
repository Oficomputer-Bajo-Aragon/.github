# CLAUDE.md

Repo `.github` de la organización **Oficomputer-Bajo-Aragon**. `profile/README.md` es la portada
pública de la org en GitHub: lo ven clientes y posibles clientes.

> Responde siempre en **español**.

## Mantener el README de perfil al día

Cada vez que se cree o se suba un repositorio nuevo a la org (o cambie uno existente de forma relevante):

1. `gh repo list Oficomputer-Bajo-Aragon --limit 100 --json name,description,isPrivate,primaryLanguage`
   y leer el README del repo: `gh api repos/Oficomputer-Bajo-Aragon/<repo>/readme -H "Accept: application/vnd.github.raw"`.
2. Añadir o actualizar su sección en **"📂 Nuestros proyectos"** con el mismo formato que las demás:
   emoji + nombre del programa, **Cliente**, 🔒 *repositorio privado* (o enlace al repo si es público),
   resumen de 2–4 líneas orientado al cliente y línea de tecnologías. Si dos repos son el mismo programa
   para clientes distintos, van en una sola sección.
3. Si el repo usa una tecnología nueva, añadir su badge en **"🧰 Tecnologías"**.
4. Si no está claro quién es el cliente, preguntarlo.

## Reglas de contenido

- **Nunca nombrar programas de terceros** (AniwinNET, ANIWIN, Aniwin…): decir siempre **"ERP"**.
  Comprobar antes de commitear: `grep -ri aniwin profile/` no debe devolver nada.
- No publicar datos internos: servidores, hosting, rutas, bases de datos, credenciales, ni detalles de despliegue.
- Repos privados: sin enlace (daría 404 a los visitantes).
- Contacto: tel/WhatsApp +34 978 831 554 (`https://wa.me/34978831554`), tienda@oficomputer.com,
  Comunidad General de Aragón, 1, 44600 Alcañiz (Teruel).
