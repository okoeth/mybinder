# A Sample Application For Binder
This sample application uses a binder compatible Dockerfile so that the repo can be immediately run with the (Binder)[https://mybinder.org] service.

In case you want to run the service locally with docker use the following command (replacing XXX and YYY with the respective info from your Strava API keys:
```
docker run -t -i --rm -p 8888:8888 -e JUPYTER_LAB_ENABLE=yes -e STRAVA_ID=XXX -e STRAVA_SECRET=YYY -v "$PWD":/home/jovyan/work mybinder
```

In case you run the notebooks in Binder, the Strava API keys need to be provided in the notebooks.
