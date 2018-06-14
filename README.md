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
   `wkhtmltopdf --margin-bottom 20mm --margin-top 10mm --minimum-font-size 14 _site/index.html resume.pdf`
   This should have generated the PDF version of the site.

For more information about building a resume using the Jekyll themes, see
https://github.com/sharu725/online-cv
