# Website README

## Course syllabi

Starting in fall 2025, I am using the following process to get syllabi for my classes:

- each class has a separate github repository where the syllabus fiiles are kept
- when the syllabus is updated in those repositories, a github action is used to copy the rendered site to two places:
    - the `docs/teaching` directory of this repo - `docs/teaching` directory has the rendered version of this site, so this makes the update syllabus publicly available
    - the `teaching` directory of this repo - the contents of teaching are automatically added to the rendered website in `docs/teaching`. by copying here, we ensure that if this website is rebuilt cleanly, we won't lose the syllabi 


## Wish list:

* get Posts up and running
* det Data up and running
* improve research page; develop callout box for abstract of papers, organize by theme, etc
* revive bio page?

## pdf version of CV

See <https://quarto.org/docs/output-formats/html-multi-format.html> for some helpful info.
I could only get the second format to work when I included a `_metadata.yml` file
inside the `cv` directory.



### NOTES leftover from previous version of website (many irrelevant):




This website is based on the template kindly provided by Karl Broman.
View the template [here](http://kbroman.org/simple_site).

To update:

* edit the appropriate .md files
* test the changes locally:
  * run `jekyll serve` to run a local jekyll server
  * dial up http://localhost:4000
* stage and commit the changes to the git repo
* push the repo to origin (github), which will make the changes live

For the DNS, I have

* www.dennisfeehan.com forwards to www.dennisfeehan.org (set via Hover's forwarding option)
* CNAME (file in this repo) points dfeehan.github.io to www.dennisfeehan.org
* DNS entry with Hover forwards www for www.dennisfeehan.org to dfeehan.github.io

The net result is that my default page is www.dennisfeehan.org

NB: see [this page](http://joshualande.com/jekyll-github-pages-poole/) for some help on setting up google analytics

NB: to change theme (eg site-wide headers, footers, etc), start by looking at _includes/themes/twitter/default.html

2017-04-22

* now I'm getting an SSL error, so I am switching DNS to CloudFlare; apparently,
  they have free SSL certs
