# Havior
This is the source code for our paper "Save It for the “Hot” Day: An LLM-Empowered Visual Analytics System for Heat Risk Management". (The source code will be released later.)

## News
The paper can be accessed in arXiv: https://arxiv.org/abs/2406.03317.


## Running the project


### Downloading the data

First download data.zip from [Google Drive](https://drive.google.com/file/d/1AFw4MEzdIadtAbKamLH4cTNyovrRQqw5). Unzip the archive and put it under the `./server/data` folder. This archive contains all climate data and pre-calculated heat risk data on 2022-07-24. (We only provide partial data for the sake of data privacy.)
### Docker

Make sure that:
- `docker` is installed on the machine and docker daemon is running
- `docker compose` plugin is available
- Port 5100 is not occupied by other process

(Optional) update the Mapbox token in `./client/Dockerfile`.

Then, in the root directory, run the following command:

```bash
docker compose up --build -d
```

You can then access the web ui from http://127.0.0.1:5100/?mode=2023 .

