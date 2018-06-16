This theme is designed by Xiaoying Riley at [3rd Wave Media](http://themes.3rdwavemedia.com/).
Visit her [website](http://themes.3rdwavemedia.com/) for more themes.

It was made into a Jekyll Theme by @sharu725.
Styling using Sass was done by @nelsonmestevao. Thanks a lot!
[A new theme](https://github.com/sivaraam/online-cv/commit/72cee73e056adeb82358ca6b84f2aa9cfcd84988)
that suits the tastes of @sivaraam was added and used to create his resume.

A PDF version of the resume could be created using [wkhtmltopdf](https://wkhtmltopdf.org/).
The steps to generate the PDF are as follows:

1. Install wkhtmltopdf. This could be done using one of the binaries found in
   the [downloads page](https://wkhtmltopdf.org/downloads.html) of the site.
1. Generate the Jekyll site: `jekyll build`
1. Generate the PDF file using wkhtmltopdf. Typical command to be executed from
   the root directory of the project:
   `wkhtmltopdf --no-outline --margin-bottom 20mm --margin-top 10mm --minimum-font-size 14 _site/index.html resume.pdf`
   This should have generated the PDF version of the site.

### Note about not generating the PDF outline
The way in which the page is currently laid out (the sidebar in¬ particular) tricks
wkhtmltopdf into generating the outline with an incorrect nesting. So, it's better
to generate the PDF without the outline for now.

Typically, this a TODO seen from two perspectives:

1. Helping wkhtmltopdf to fix the issues with sidebars (if there is one ;-)
2. Changing the layout of the site to avoid this issue

It would be nice to achieve the former.
