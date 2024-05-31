# legolilypadsd15
To create your lilypad workflow use the command above
creatad using
## To build
```bash
docker build . -f Dockerfile -t espinosa1991/legolilypadsd15:0.0.3 --target runner
```
## To run
```bash
docker run -it --gpus all -v $PWD/outputs:/outputs -e PROMPT='RAW photo, <lora:lego_v2.0.768-000035:0.8> LEGO BrickHeadz, a dragon in a cave, (high detailed skin:1.2), 8k uhd, dslr, soft lighting, high quality, film grain, Fujifilm XT3' -e STEPS=30 espinosa1991/legolilypadsd15:0.0.3
```
## To publish
```bash
docker push espinosa1991/legolilypadsd15:0.0.3
```
## To run your worklow at lilypad
```bash
export WEB3_PRIVATE_KEY=<walletprivatekey>
lilypad run github.com/lucasespinosa28/legolilypad:0.01 -i Prompt="an astronaut floating against a white background
```
