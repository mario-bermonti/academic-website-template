
# Table of Contents

-   [Academic Website Template](#org47a7a88)
-   [Building your website](#orgb548cc7)
-   [Modifying the website](#org3f81932)
    -   [Important note](#org293d8a5)
    -   [Adding the website's basic information](#org6f396ce)
    -   [Adding content](#org8425039)
    -   [Further customization](#org7d46d5a)
-   [Contributing to this project](#org898dde0)
-   [Other options](#org5267997)
-   [Author](#orgfbf1c29)
-   [License](#org78e7d2b)


<a id="org47a7a88"></a>

# Academic Website Template

This template was designed to provide an easy way to create academic 
websites. The goal is to lower the barrier to create webpages
for scholars with limited knowledge about programming.

This is achieved by separating content from form. This way you can simply
add your content and everything else is done for you. This template is
heavily influenced by [Academic pages](https://github.com/academicpages/academicpages.github.io) and [Simon Ho's website](https://www.simonho.ca/).

This website template is created with [Jekyll](https://jekyllrb.com/) - a static site generator -
and uses the [minimal mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/). The template was created so that 
it's easy to deyloy to [Github Pages](https://pages.github.com/), but you can make simple
modifications to deploy it on other services (see the [Jekyll documentation](https://jekyllrb.com/docs/deployment/)).


<a id="orgb548cc7"></a>

# Building your website

1.  Create your own copy of this website by [forking](https://guides.github.com/activities/forking/) this GitHub repo
2.  [Unwatch](https://docs.github.com/en/github/managing-subscriptions-and-notifications-on-github/managing-your-subscriptions#unwatch-a-repository) the repo
3.  [Rename the repo](https://docs.github.com/en/enterprise/2.14/user/articles/renaming-a-repository) to <https://username.github.io> ([see step 3 of this guide](https://docs.github.com/en/github/working-with-github-pages/creating-a-github-pages-site-with-jekyll#creating-a-repository-for-your-site))
4.  Your website should be live at
    <https://username.github.io> ([see step 7 of this guide](https://docs.github.com/en/github/working-with-github-pages/creating-a-github-pages-site-with-jekyll#creating-a-repository-for-your-site))


<a id="org3f81932"></a>

# Modifying the website


<a id="org293d8a5"></a>

## Important note

There are two ways to modify your website. I will discuss them very
briefly [here](docs/how-to-modify-website.md) to help you make your decision. 


<a id="org6f396ce"></a>

## Adding the website's basic information

This information is configured in
the `_config.yml` file. Here you can add information like the website's name,
your name, links to your research platforms, and many other information. 
Explore the different options to find everything that can be modified.


<a id="org8425039"></a>

## Adding content

Most pages incorporate their content from two sources: the actual 
file (e.g., `Research.md`) and the `yaml` file with the same name that 
can be found in the `_data` directory. 

This helps facilitate the process of adding new information because
the `yaml` files are very easy and intuitive to use, even if you don't know
any programming. These files follow a *bullet* or outline format and just
require you to *list* the contents you want displayed in the page.

For example, the Research page presents all the information that you include
in the `Research.md` file and then it includes the research projects
you have listed in the `research.yml` file. This makes it easier to 
continually add new research projects in the `yaml` file and keep your 
webpage updated.

Below you will find a description of how to modify your website. If you
prefer a more detailed version of this documentation please refer to
the [long version of this documentation](docs/add-content-long-version.md).

-   Add content to existing pages

    The Research, Publications, Talks, and Software pages get their contents from
    their `markdown` and associated `yaml` file. So you have to modify
    both files.

-   Featured rows

    The Home and Research pages contain a feature row to highlight your
    interests. To modify these rows, you have to provide the required
    information in each page. You can check the [theme's webpage](https://mmistakes.github.io/minimal-mistakes/docs/helpers/#feature-row)
    for more details.

-   Add and remove pages

    Just create a `markdown` file in the `_pages` directory, add the
    metadata, and content. You also have to modify the `navigation.yml` 
    file.
    
    To remove pages, just delete the page from the `_pages` directory and
    delete the entry from the `navigation.yml`.

-   Adding files for download

    Add the files you need to be available in the website (e.g., CV, pdf
    for downloading) in the `downloads` directory.

-   Blog

    To modify the blog's home page, just add your content to the `blog.md`
    file in `_pages`.
    
    Blog posts are in the `_posts` directory. You can remove the ones
    that are there for illustration purposes. They are all from the 
    minimal mistakes theme project template.
    
    To add new blog posts, just create a new `markdown` file that meets the
    name and metadata requirements and add your content. See the [Jekyll's](https://jekyllrb.com/docs/posts/) 
    webpage for more details.


<a id="org7d46d5a"></a>

## Further customization

The website has many more features. Please read
[Jekyll's](https://jekyllrb.com/docs/) and [minimal mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/quick-start-guide/) documentation for 
learning how to modify how the website looks and how it's structured.


<a id="org898dde0"></a>

# Contributing to this project

All contributions are welcome!

You can help out by writing documentation or tutorials on how to modify
certain things, report bugs or errors in code or documentation, fixing bugs,
or by providing ideas. This is a beginner friendly project!

You are welcome to communicate any errors by [submitting an
issue](https://github.com/mario-bermonti/academic-website-template/issues) on Github.

To fix bugs, clone the repository, add your contribution, 
and submit a [pull request](https://github.com/mario-bermonti/academic-website-template/pulls).

If have suggestions on how to improve the website design (e.g., default
tabs, theme, etc.), please open an [issue on Github](https://github.com/mario-bermonti/academic-website-template/issues) or [email me](mailto:mbermonti1132@gmail.com). Please
keep in mind that the template should be general enough so that any features
work for most people, so only suggestions that will benefit most people will be
incorporated.


<a id="org5267997"></a>

# Other options

-   [Matthew Kirby's Academic template](https://github.com/matthewkirby/academictemplate) (I actually discovered this one too late)
-   [Academic pages](https://academicpages.github.io) (it didn't work for me)


<a id="orgfbf1c29"></a>

# Author

This project was developed by Mario E. Bermonti-Pérez as part of
his academic research and activities. Feel free to contact me
at [mbermonti@psm.edu](mailto:mbermonti@psm.edu) or [mbermonti1132@gmail.com](mailto:mbermonti1132@gmail.com)


<a id="org78e7d2b"></a>

# License

This project is based on the [minimal mistakes starter repository](https://github.com/mmistakes/minimal-mistakes/) 
and is licensed under the MIT license, just as the original project.

Please read the [License](./LICENSE) file for more details.

