---
title: "Installation"
date: 2023-03-31
weight: 2
draft: true
---

Les étapes suivantes sont là pour vous aider à initialiser votre nouveau site Web. Si vous ne connaissez pas du tout Hugo, nous vous suggérons fortement d'en savoir plus en suivant ce [excellente documentation pour les débutants](https://gohugo.io/overview/quickstart/).

### Create your project

Hugo provides a `new` command to create a new website.

```
hugo new site <new_project>
```

### Install the theme

Install the **GoDocs** theme by following [this documentation](https://gohugo.io/themes/installing/)

This theme's repository is: https://github.com/themefisher/godocs.git

Alternatively, you can [download the theme as .zip](https://github.com/themefisher/godocs/archive/master.zip) file and extract it in the `themes` directory

Or you can check this video documentation for installing this template:
{{< youtube Srt3lTmRxzQ >}}

### Basic configuration

When building the website, you can set a theme by using `--theme` option. However, we suggest you modify the configuration file (`config.toml`) and set the theme as the default.

```toml
# Change the default theme to be use when building the site with Hugo
theme = "godocs"
```


### Create your first content pages

Then, create content pages inside the previously created chapter. Here are two ways to create content in the chapter:

```
hugo new installation/first-content.md
hugo new installation/second-content/_index.md
```

Feel free to edit thoses files by adding some sample content and replacing the `title` value in the beginning of the files. 

### Launching the website locally

Launch by using the following command:

```
hugo serve
```

Go to `http://localhost:1313`

### Build the website

When your site is ready to deploy, run the following command:

```
hugo
```

A `public` folder will be generated, containing all static content and assets for your website. It can now be deployed on any web server.

{{< notice "info" >}}
This website can be automatically published and hosted with [Netlify](https://www.netlify.com/) (Read more about [Automated HUGO deployments with Netlify](https://www.netlify.com/blog/2015/07/30/hosting-hugo-on-netlifyinsanely-fast-deploys/)). Alternatively, you can use [Github pages](https://gohugo.io/hosting-and-deployment/hosting-on-github/)
{{< /notice >}}