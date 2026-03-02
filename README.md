# Personal website and portfolio built with [Quarto][quarto]

[![Quarto Publish](https://github.com/sayalaruano/sayalaruano.github.io/actions/workflows/deploy.yml/badge.svg)][deploy-ga]

## Live Site

The website is automatically rendered and deployed to: **[sayalaruano.github.io][personal-website]**

## Structure 

The `main` branch contains the source files for the Quarto website. You can find a quick overview of the key folders and files below:

* **`*.qmd`**: Main pages of the website located in the root directory (e.g., `index.qmd`, `about.qmd`, `cv.qmd`, etc).
* **`styles.scss`**: Custom SASS/CSS styling used to personalize the website theme.
* **`_quarto.yml`**: Quarto configuration file defining the website structure, navigation, and build settings.
* **`projects/`**: Collection of project pages, each with its own `.qmd` file and associated assets.
* **`talks/`**: Directory for talk pages, following the same structure as projects.
* **`images/`**: Folder for all images used in the website.
* **`_extensions/`**: Custom Quarto extensions, if any, for additional functionality.

> [!NOTE]
> Rendered files (the `/docs/` folder) are intentionally omitted from this branch via `.gitignore`. The live HTML files and assets are generated 
> automatically and stored in the `gh-pages` branch, which is used for deployment. 

## How it Works?

This repo uses a GitHub Actions workflow to automate the rendering and deployment process. Here's how it works:

1. **Edit**: Modify `.qmd`, `.scss`, or `.md` files in the `main` branch.
2. **Push**: Commit and push your changes to the `main` branch on GitHub.
3. **Automate**: GitHub Actions detects the change, installs Quarto, renders the site using your custom styles, and pushes the output to the `gh-pages` branch.

## Local Development

If you want to preview changes locally:

1. Install the [Quarto CLI][quarto-cli].
2. Run the preview server in the root directory:

   ```bash
   quarto preview
   ```

## Migration Note

This project was recently migrated from a **Hugo (Apéro/Blogdown)** framework to **Quarto**. The original Hugo source code is preserved in the `hugoapero-version` branch for reference. 

## License

The code in this repository is licensed under the **MIT License**, allowing you to use, modify, and distribute it freely as long as you include the original copyright and license notice.

The documentation and other creative content are licensed under the **Creative Commons Attribution 4.0 International (CC BY 4.0) License**, meaning you are free to share and adapt it with proper attribution.

Full details for both licenses can be found in the [LICENSE](LICENSE.md) file.

## Learn More

If you want to create your own website, I recommend to check the [Quarto documentation][quarto-docs], Sam Shanny-Csik [Quarto website tutorial][quarto-website-tutorial], the [Quarto Gallery][quarto-gallery], and the [Awesome Quarto repository][awesome-quarto-repo] for inspiration and resources.

## Acknowledgements

Thanks to the Quarto team and its community for providing an excellent open-sourceframework for building websites. The design and structure were inspired by various online portfolios and personal websites, including those of [Sam Shanny-Csik][sam-shanny-website] and [Beatriz Milz][bea-milz-website].

[quarto]: https://quarto.org/
[deploy-ga]: https://github.com/sayalaruano/sayalaruano.github.io/actions/workflows/deploy.yml
[personal-website]: https://sayalaruano.github.io/
[quarto-cli]: https://quarto.org/docs/get-started/
[quarto-docs]: https://quarto.org/docs/
[quarto-website-tutorial]: https://ucsb-meds.github.io/creating-quarto-websites/
[quarto-gallery]: https://quarto.org/gallery/
[awesome-quarto-repo]: https://github.com/mcanouil/awesome-quarto
[sam-shanny-website]: https://samanthacsik.github.io/
[bea-milz-website]: https://beatrizmilz.com/
