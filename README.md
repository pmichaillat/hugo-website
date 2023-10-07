# Minimalist Hugo Template for Academic Websites

This repository contains a [Hugo](https://github.com/gohugoio/hugo) template to create a personal academic website. The template uses the [PaperMod theme](https://github.com/adityatelange/hugo-PaperMod) but modifies it in various ways to be more minimalist and better suited for academic websites. The website is hosted on [GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/about-github-pages).

## Documentation

The template is documented at https://pascalmichaillat.org/b/.

## Illustration

The website produced by the template can be viewed at https://pascalmichaillat.org/hugo-website/.

## Installation

### On your local machine

+ Install [Hugo](https://gohugo.io/installation/). On a Mac, this can be done with [Homebrew](https://brew.sh): run `brew install hugo` in the terminal. If you already have Hugo but it is outdated, run `brew upgrade hugo`.
+ Since the website is hosted on GitHub Pages, it is convenient to install [GitHub Desktop](https://desktop.github.com). The website can be updated from your local machine via GitHub Desktop without going to GitHub.
+ Clone the template repository to your local machine. This can be done in two steps:
	1. Click "Use this template" and then "Create a new repository" at the top of the repository.
	2. Once the new repository is created on your GitHub account, open GitHub Desktop and click "File" and then "Clone repository". Find the newly created repository under the "GitHub.com" tab and clone it.
+ Update the `baseURL` parameter in `config.yml` with the website URL that you plan to use. By default the URL is `https://username.github.io`.

### On your GitHub account

+ The first time that you push your repository to GitHub, you need to allow GitHub Actions and GitHub Pages so the website can be built and deployed to GitHub Pages.
+ The first step is to [ask GitHub to publish the website with a GitHub Action](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site#publishing-with-a-custom-github-actions-workflow). GitHub offers a ready-made action to publish a Hugo website, called `Deploy Hugo site to Pages`. This action must be enabled in the [Pages Settings](https://github.com/pmichaillat/hugo-website/settings/pages) of your GitHub repository. You can view the workflow triggered by the action in the `.github/workflows/hugo.yml` file.
+ Once the GitHub Actions are enabled, GitHub will build and publish the website as soon as the repository is updated. 
+ If you would like to update the deployment action (for instance because it became outdated and fails to deploy the site), you can find the [most recent action on GitHub]( https://github.com/actions/starter-workflows/blob/main/pages/hugo.yml). You can place this file directly in the `.github/workflows` folder to replace the old `hugo.yml` file—but make sure to set `push: branches` to `["main"]`.

## Usage

### Local development

Navigate to the website directory (`cd`) and run in the terminal:

```bash
hugo server
```

The command builds the website on your machine and makes it available at http://localhost:1313, rebuilding automatically as you edit. You can modify the content of the repository and develop your website entirely on your machine.

### Online deployment

Once your website is ready to be made public, commit your content and template changes and push them to the website repository on GitHub. It is convenient to use GitHub Desktop for this Git operation.

On each push, the [GitHub Actions workflow](https://github.com/pmichaillat/hugo-website/actions/workflows/hugo.yml) invokes Hugo to generate the website and deploys the output to [GitHub Pages](https://github.com/pmichaillat/hugo-website/deployments/github-pages). During the workflow, Hugo processes your content, templates, and other project files and generates a static website.

## Performance

The website performs well on mobile and desktop devices. Here is an overview of the mobile performance from [PageSpeed Insights](https://pagespeed.web.dev/):

<img width="470" alt="mobile" src="https://github.com/pmichaillat/hugo-website/assets/85443660/1488df3e-19bb-4f9f-8a86-11f361414d92">

And here is an overview of the desktop performance:

<img width="453" alt="desktop" src="https://github.com/pmichaillat/pmichaillat.github.io/assets/85443660/eff134d2-6097-4bc2-bfd7-4f5c18571789">

## Software

+ The website is built with Hugo v0.147.2 via GitHub Actions.
+ The website was developed locally with Hugo v0.147.2 on macOS Sequoia. 
+ The website was tested on the following browsers:
	+ Safari 18.4 on macOS Sequoia
	+ Mobile Safari on iOS 18  
+ Other Hugo versions, operating systems, and web browsers may require minor adjustments. Please [report any issues](https://github.com/pmichaillat/hugo-website/issues) to help improve compatibility.

## License

This repository is licensed under the [MIT License](LICENSE.md).

## Related resources

+ [latex-cv](https://github.com/pmichaillat/latex-cv) - This LaTeX template produces a minimalist academic CV, which you can post on your website. The CV should be named `cv.pdf` and placed in the `static` folder. It will be accessible from the homepage via a social icon.

## Real-world implementations

+ [Pascal Michaillat's website](https://pascalmichaillat.org/) ([source code](https://github.com/pmichaillat/pmichaillat.github.io))
+ [Dylan Balla-Elliott's website](https://www.dballaelliott.com) ([source code](https://github.com/dballaelliott/site))
+ [Rosa van den Ende's website](https://rosavandenende.github.io) ([source code](https://github.com/rosavandenende/rosavandenende.github.io))
+ [Samia Kabir's website](https://samiakabir.com) ([source code](https://github.com/SamiaKabir/samiakabir.github.io))
+ [Dylan Laplace Mermoud's website](https://dylanlaplacemermoud.github.io) ([source code](https://github.com/DylanLaplaceMermoud/dylanlaplacemermoud.github.io))
+ [Maarten Goos's website](https://maartengoos.com) ([source code](https://github.com/MaartenGoos/website))
+ [Aryan Ahadinia's website](https://aryanahadinia.github.io) ([source code](https://github.com/AryanAhadinia/AryanAhadinia.github.io))
+ [Jun Wong's website](https://junwong.org) ([source code](https://github.com/junwong97/junwong97.github.io))
+ [Erling Rennemo Jellum's website](https://erlingrj.github.io) ([source code](https://github.com/erlingrj/erlingrj.github.io))
+ [Yangkeun Yun's website](https://yangkeunyun.github.io) ([source code](https://github.com/yangkeunyun/yangkeunyun.github.io))
+ [Maghfira Ramadhani's website](https://maghfiraer.github.io) ([source code](https://github.com/maghfiraer/maghfiraer.github.io))
+ [Ismael Moreno-Martinez's website](https://ismaelmorenomartinez.eu) ([source code](https://github.com/ismaelmorenomartinez/ismaelmorenomartinez.github.io))
+ [Lucas Warwar's website](https://lucaswarwar.github.io) ([source code](https://github.com/lucaswarwar/lucaswarwar.github.io))
+ [Franz Louis Cesista's website](https://leloykun.github.io) ([source code](https://github.com/leloykun/leloykun.github.io))
+ [Gabe Sekeres's website](https://gabesekeres.com) ([source code](https://github.com/gsekeres/hugo_site))
+ [Kevin Roice's website](https://kevroi.github.io) ([source code](https://github.com/kevroi/kevroi.github.io))
+ [Daniel Barbosa's website](https://dacbarbosa.github.io) ([source code](https://github.com/dacbarbosa/dacbarbosa.github.io))
+ [Wei Zhang's website](https://weizhang-econ.github.io) ([source code](https://github.com/weizhang-econ/weizhang-econ.github.io))
+ [Ben Hermann's website](http://benhermann.eu) ([source code](https://github.com/bhermann/bhermann.github.io))
+ [Franco Corona's website](http://fcorona.me) ([source code](https://github.com/exibios/exibios.github.io))
+ [Tom George's website](https://tomge.org) ([source code](https://github.com/TomGeorge1234/TomGeorge1234.github.io))
+ [Yucheng Zhou's website](https://yuchengzhou.com) ([source code](https://github.com/YuchengZ-Fin/YuchengZ-Fin.github.io))
+ [Rui Sousa's website](https://ruiagmsousa.github.io) ([source code](https://github.com/ruiagmsousa/ruiagmsousa.github.io))
+ [Stefano Sangiovanni's website](https://ste-sangiovanni.github.io) ([source code](https://github.com/ste-sangiovanni/ste-sangiovanni.github.io))
+ [Seth Watts's website](https://www.sethbwatts.com) ([source code](https://github.com/sBwatts/hugo-website))
+ [Louise Demoor's website](https://louisedemoor.github.io/website/) ([source code](https://github.com/louisedemoor/website))
+ [Giwon Bahg's website](https://giwonbahg.github.io) ([source code](https://github.com/giwonbahg/giwonbahg.github.io))
+ [Arthur Douillard's website](https://arthurdouillard.com)
+ [Benjamin Hattemer's website](https://benjaminhattemer.com)
+ [Kostas Bimpikis's website](https://stanford.edu/~kostasb/)
+ [Pragathi Praveena's website](https://pragathipraveena.com)
+ [Qiwei He's website](https://www.qiwei-he.com)
+ [Pierre Bardier's website](https://pierrebard.github.io/pierre-bardier/)
+ [Marek Wiewiórka's website](https://marekwiewiorka.org)
+ [Eran Shmuëli's website](https://eranshmueli.com)
+ [Bo Wang's website](https://bowang.finance)