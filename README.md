# Minimalist Hugo Template for Academic Websites

This repository contains a [Hugo](https://github.com/gohugoio/hugo) template to create a personal academic website. The template uses the [PaperMod theme](https://github.com/adityatelange/hugo-PaperMod) but modifies it in various ways to be more minimalist and more adapted to academic websites. The website is hosted on [GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/about-github-pages).

## Documentation

The template is documented at https://pascalmichaillat.org/d5/.

## Illustration

The website produced by the template can be viewed at https://pascalmichaillat.org/hugo-website/.

## Installation

### On your local machine

+ Clone the repository to your local machine
+ Install [Hugo](https://gohugo.io/installation/). On a Mac, this is easily done with [Homebrew](https://brew.sh): simply run `brew install hugo` in the terminal.
+ Since the website is hosted on GitHub Pages, it is convenient to install [GitHub Desktop](https://desktop.github.com). The website can conveniently be updated from your local machine via GitHub Desktop without going to GitHub.
+ Update the `baseURL` parameter in `config.yml` with the website URL that you plan to use. By default the ULR is `https://username.github.io`.

### On your GitHub account

+ The first time that you push your repository to GitHub, you need to allow GitHub Actions and GitHub Pages so the website can be built and deployed to GitHub Pages.
+ The first step is to [ask GitHub to publish the website with a GitHub Action](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site#publishing-with-a-custom-github-actions-workflow).  GitHub offers a ready-made action to publish a Hugo website, called `Deploy Hugo site to Pages`. This action must be enabled in the [Pages Settings](https://github.com/pmichaillat/hugo-website/settings/pages) of your GitHub repository. You can view the workflow triggered by the action in the `.github/workflows/hugo.yml` file.
+ Once the GitHub Actions are enabled, GitHub will build and publish the website as soon as the repository is updated. 
+ If you would like to update the deployment action (for instance because it became outdated and fails to deploy the site), you can find the [most recent action on GitHub]( https://github.com/actions/starter-workflows/blob/main/pages/hugo.yml). You can place this file directly in the `.github/workflows` folder to replace the old `hugo.yml` file—but make sure to set `push:
    branches` to `["main"]`.

## Usage

### Development

Navigate to the website directory and run `hugo server` in the terminal. The command builds the website on your machine and makes it available at http://localhost:1313. You can modify the content of the repository and develop your website entirely on your local machine.

### Compilation

Once your website is ready to be made public, run `hugo` in the terminal from the website directory. When you run the `hugo` command, Hugo processes your content, templates, and other project files and generates a static website. The resulting output is placed in the `public` folder.

### Deployment

With GitHub Desktop, commit the changes and push them to the website repository on GitHub. Then, the [GitHub Action](https://github.com/pmichaillat/hugo-website/actions/workflows/hugo.yml) builds the website and deploys it to [GitHub Pages](https://github.com/pmichaillat/hugo-website/deployments/github-pages).

## Performance

Despite the modifications to the PaperMod theme, the website continues to perform well on mobile and desktop devices. Here is an overview of the mobile performance from [PageSpeed Insights](https://pagespeed.web.dev/):

<img width="470" alt="mobile" src="https://github.com/pmichaillat/hugo-website/assets/85443660/1488df3e-19bb-4f9f-8a86-11f361414d92">

And here is an overview of the desktop performance:

<img width="453" alt="desktop" src="https://github.com/pmichaillat/pmichaillat.github.io/assets/85443660/eff134d2-6097-4bc2-bfd7-4f5c18571789">

## Software

The website was built with Hugo v0.128.2 on an Apple Silicon Mac running macOS Sonoma 14.5. The website was tested and validated on Safari 17.5 on a Mac and on Safari on an iPhone with iOS 17.5.[^1]

[^1]:  The updates to Hugo v0.120 and then to Hugo v0.123 introduced some issues with previous versions of the template. The issue caused by the update to Hugo v0.120 is [#1325 in the PaperMod repo](https://github.com/adityatelange/hugo-PaperMod/issues/1325). The issue caused by the update to Hugo v0.123 is [#1449 in the PaperMod repo](https://github.com/adityatelange/hugo-PaperMod/issues/1449). These issues are now resolved

While the template should also work on other operating systems and with other versions of Hugo, compatibility cannot be guaranteed. Users on Windows or Linux systems, or those using different Hugo versions, may need to make minor adjustments. Similarly, the website should work with other browsers, but minor adjustments might be necessary for perfect compatibility. [Please report](https://github.com/pmichaillat/hugo-website/issues) any compatibility issues or bugs to help improve cross-platform support.

## License

The content of this repository is licensed under the terms of the MIT License.

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
+ [Kostas Bimpikis's website](https://stanford.edu/~kostasb/)
+ [Pragathi Praveena's website](https://pragathipraveena.com)
+ [Qiwei He's website](https://www.qiwei-he.com)
+ [Pierre Bardier's website](https://pierrebard.github.io/pierre-bardier/)
+ [Marek Wiewiórka's website](https://marekwiewiorka.org)
