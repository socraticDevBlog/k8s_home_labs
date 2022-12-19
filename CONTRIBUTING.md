# contributing to this project?

Either you've spotted a bug in current lab files or you've been asked to add or
improve a lab, you will observe standard contributing practices:

- lint your code before submitting;
- open an atomic PR and add details (in english) describing what your
  contribution is about.

## web presence

A major aspect of this codebase is the website.

This web presence is intended to make this project easier to use for cloud
developers (our end-users).

Being efficient (not lazy), we are using [GitHub Pages Jekyll static site
generator](https://pages.github.com/).

This technology turns `README.md` markdown files into nicely formatted and
styled `html` pages.

### codebase scaffolding rationale

At project's root, there are some boilerplate files required for our web
presence:

| filename    | function                                                     |
| ----------- | ------------------------------------------------------------ |
| _config.yml | read by Jekyll to generate static site                       |
| CNAME       | use for DNS and TLS purposes to serve Page with a pretty URL |
| 404.md      | to have a styled, pretty 404 not found page                  |

Every directory hold either a tool or a lab we want to showcase.

Every directory should have a `README.md` file. This file will get displayed to
this project's website.

\* Make sure to add a link to this directory's `README.md` from the project's
root `README.md` file: the homepage.