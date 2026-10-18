# Unraid templates

Community Applications templates for [Legejo](https://github.com/jularboolean/legejo), a self-hosted library for EPUB books.

| Template | Image |
|---|---|
| [`templates/legejo.xml`](templates/legejo.xml) | [`slurvdjur/legejo:1`](https://hub.docker.com/r/slurvdjur/legejo) |

## Legejo on Unraid

Install Legejo from **Apps** (search for Legejo), or add this repository's template by its raw URL. Then open the WebUI on port 3000 and sign in with the admin user and password from the template. If the password was left empty, it is printed once in the container log on the first start.

Everything Legejo keeps, the SQLite database included, is in the appdata folder (`/mnt/user/appdata/legejo` by default), so backing that folder up backs up the library.

The template uses the `1` tag: updates within Legejo 1.x arrive as image updates in Unraid. All settings are described in the [Legejo README](https://github.com/jularboolean/legejo#configuration); any `LEGEJO_*` variable can be added to the container.

## License

The templates are MIT licensed. Legejo itself is AGPL-3.0.
