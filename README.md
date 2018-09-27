# `IODC 2018`

A quick fix for your [IODC](https://www.opendatacon.org/#/) FOMO.

Try it on [shinyapps.io](https://behindbars.shinyapps.io/iodc2018/) 

To run this on your own, you need to create an OAuth twitter token for [`rtweet`][rtweet].

To have this app recognize your twitter PAT, you have a couple options:

1. You can follow all of the steps in [Using OAuth to Access Twitter APIs](https://rud.is/books/21-recipes/using-oauth-to-access-twitter-apis.html), 

2. You can save your `twitter_token` to `rtweet.rds` in the app directory

3. You can code up another alternative by setting `.TWITTER_PAT` in a file called `twitter_secrets.R`.

(The first one is the best answer.)

### Required packages

I used the following packages to make this, all of which can all be installed from CRAN:

```r
packages = c("shiny", "rtweet", "dplyr", "stringr",
             "purrr", "httr", "DT", "shinythemes", 
             "glue", "simpleCache")
install.packages(packages)
```


