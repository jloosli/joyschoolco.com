# joyschoolco.com

## Development

Joyschoolco.com is built with [Hugo](https://gohugo.io/). To run a local server for development, use the following command:

```bash
docker compose up --build server
```

This will start a local server at `http://localhost:1313` and watch for changes to the site files. Any changes made will automatically refresh the browser.

## Deployment

The site is deployed using github pages. Any changes pushed to the `main` branch will trigger a deployment to github pages.

## Dependencies

- [Hugo](https://gohugo.io/) - Static site generator
- [Ananke Theme](https://github.com/theNewDynamic/gohugo-theme-ananke) - Hugo theme used for the site
- [Tachyons](https://tachyons.io/) - CSS framework used for styling
- [Docker](https://www.docker.com/) - Containerization platform used for development and deployment
- [GitHub Actions](https://github.com/features/actions) - CI/CD platform used for automating workflows
- [GitHub Pages](https://pages.github.com/) - Hosting service for the deployed site
- [Cloudflare](https://www.cloudflare.com/) - DNS and CDN service used for the domain joyschoolco.com

## Customization

The files in the `layouts` directory are customizations of the Ananke theme. The main layout changes have been:

- Remove `.measure-wide` and `.tc-l` classes from the main content areas to make it wider and left-aligned.
- Add `.mw8` class to the main content areas to limit the maximum width to 80 characters for better readability.
