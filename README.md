# A short & quick demo of creating MB1L docker image on a local machine.


- You need to go to [docker.com](https://www.docker.com/).

-   create an account and then log in locally with

```docker login```

- Then, just push the image with

```docker push MB1L```

- Then, from the root of the repository, they’d run this:

```docker run --rm -p 8787:8787 -e DISABLE_AUTH=true -v $(pwd):/home/rstudio/shceof```

- This would download the image if necessary and then run it. And then they’d go to ``localhost:8787`` on any browser to be greeted with an RStudio session with all the things:

![online-rstudio](https://user-images.githubusercontent.com/47132064/177157758-7ade9514-c465-4047-ae2d-51068d8ce582.png)
