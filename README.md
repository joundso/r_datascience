# Rdatascience

This repo holds several files for my personal dockerized R environment for data science. It is not maintained and from time to time adjusted to my needs.

## Usage

:bulb: If you want to mount folders from your host system to with the container, make sure they are correctly described in the [`docker-compose.yml`](./docker-compose.yml) file. If you don't want to mount anything, ignore this.

```bash
git clone https://github.com/joundso/docker_images.git Rdatascience
cd Rdatascience
docker-compose up -d
```

- On your host-machine, you can now open a webbrowser and go to page [`localhost:8787`](http://localhost:8787) to see RStudio server. Login with the user-password-combination specified in [`Dockerfiles/rdsc_base_j.dockerfile`](./Dockerfiles/rdsc_base_j.dockerfile) and start working. Default username is `user`, default password is `password`.

- When you deploy a shiny app, it will be accessible via [`localhost:3838`](http://localhost:3838).

## More Infos

- About RStudio Server: <https://www.rstudio.com/products/rstudio/download-server/>
- About Shiny: <https://www.rstudio.com/products/shiny/>
- RStudio and Shiny are trademarks of RStudio, Inc.

## Contributions

Big thanks to the [inspiration of this fork](https://github.com/kapsner)!
