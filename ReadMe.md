# Website README


## Wish list:

* get Posts up and running
* det Data up and running
* improve research page; develop callout box for abstract of papers, organize by theme, etc
* revive bio page?




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