# juxtorpus

> [!WARNING]
> **This tool is archived and no longer supported or maintained.**
> It was developed by the Australian Text Analytics Platform (ATAP), the previous phase of the
> Language Data Commons of Australia (LDaCA). It is preserved as a frozen Docker image so that it
> keeps launching on BinderHub as it last worked, but it will not be updated or fixed.
> For current LDaCA text analytics tools, please use
> [Wordflow](https://australian-text-analytics-platform.github.io/LDaCa_Text_Analytics_Tools/) and
> [LADAL](https://ladal.edu.au).

Compare and analyse two corpus.

To run the corpus demo notebook (`notebooks/demos/corpus.ipynb`), click the button below to launch it on the
ARDC BinderHub. Australian Access Federation (AAF) or Reannz Tuakiri (NZ) authentication is required.

[![Binder](https://binderhub.rc.nectar.org.au/badge_logo.svg)](https://binderhub.rc.nectar.org.au/v2/gh/Australian-Text-Analytics-Platform/juxtorpus/archived?labpath=notebooks%2Fdemos%2Fcorpus.ipynb)

## Development

To set up the dev environment...

```shell
./init.dev.sh
```

## Run locally with Docker

The frozen environment of this tool is published as the Docker image
[`milysun/atap-juxtorpus`](https://hub.docker.com/r/milysun/atap-juxtorpus). With [Docker](https://docs.docker.com/get-docker/) installed, run:

```bash
docker run --rm -p 8888:8888 milysun/atap-juxtorpus:6381ee847911 jupyter lab --ip=0.0.0.0 --port=8888
```

then open the `http://127.0.0.1:8888/lab?token=...` link printed in the terminal.
On Apple Silicon Macs add `--platform linux/amd64` after `docker run`.
