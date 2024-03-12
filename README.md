

<!-- README.md is generated from README.Rmd. Please edit that file -->

# tidymodels-pipelines

<!-- badges: start -->
<!-- badges: end -->

## How to build site locally.

All examples on this website uses CRAN version of R packages, and they
should be installed as such.

### Docker

Installing Docker should be fairly straightforward. Please refer to [Get
Started](https://www.docker.com/get-started/) for how to.

### Setting up Posit Connect

For the smoothest experience, we recommend that you authenticate using
environment variables. The two variables you will need are
`CONNECT_SERVER` and `CONNECT_API_KEY`.

> **Tip**
>
> The function
> [usethis::edit_r_environ()](https://usethis.r-lib.org/reference/edit.html)
> can be very handy to open `.Renviron` file to specify your environment
> variables.

`CONNECT_SERVER` is the URL of the posit connect page. So if your
connect server is accessed through
`https://example.com/connect/#/content/` then you can find
`CONNECT_SERVER` by removing `connect/` and everything that follows it,
leaving you with `https://example.com/`.

`CONNECT_API_KEY` is created through your Connect server. 1. Click on
your name in the upper right upper right. 1. Click `API keys`. 1. Click
`New API Key`. 1. Give your API a key, click \``Create Key`.

Once you have those two, you can add them to your `.Renviron` file in
the following format:

``` markdown
CONNECT_API_KEY=xxxxxxxxxxxxxxxxxxxxxxxxxxxx
CONNECT_SERVER=https://example.com/
```

Note that you don’t want to put quotes around the values.

### Setting up Amazon S3

For the smoothest experience, we recommend that you authenticate using
environment variables. The two variables you will need are
`AWS_ACCESS_KEY_ID` and `AWS_SECRET_ACCESS_KEY`.

> **Warning**
>
> Depending on your S3 setup, you will need to use additional variables
> to connect. Please see
> <https://github.com/paws-r/paws/blob/main/docs/credentials.md> and
> this [pins issue](https://github.com/rstudio/pins-r/issues/608) for
> help if the following paragraphs doesn’t work for you.

> **Tip**
>
> The function
> [usethis::edit_r_environ()](https://usethis.r-lib.org/reference/edit.html)
> can be very handy to open `.Renviron` file to specify your environment
> variables.

You can find both of these keys in the same location.

1.  Open the [AWS Console](https://console.aws.amazon.com/)
2.  Click on your username near the top right and select
    `Security Credentials`
3.  Click on `Users` in the sidebar
4.  Click on your username
5.  Click on the `Security Credentials` tab
6.  Click `Create Access Key`
7.  Click `Show User Security Credentials`

Once you have those two, you can add them to your `.Renviron` file in
the following format:

``` markdown
AWS_SECRET_ACCESS_KEY=xxxxxxxxxxxxxxxxxxxxxxxxxxxx
AWS_ACCESS_KEY_ID=xxxxxxxxxxxxxxxxxxxxxxxxxxxx
```
