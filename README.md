# legolilypadsd15
To create your lilypad workflow use the command above
creatad using [google](www.google.com).
## To build
```bash
docker build . -f Dockerfile -t espinosa1991/legolilypadsd15:0.0.3 --target runner
```
## To run
```bash
docker run -it --gpus all -v $PWD/outputs:/outputs -e PROMPT='a lilypad in space' -e STEPS=30 espinosa1991/legolilypadsd15:0.0.3
```
## To publish
```bash
docker push espinosa1991/legolilypadsd15:0.0.3
```
## To run your worklow at lilypad
```bash
export WEB3_PRIVATE_KEY=<walletprivatekey>
lilypad run <this github repo:realease tag> -i Prompt="an astronaut floating against a white background
```
