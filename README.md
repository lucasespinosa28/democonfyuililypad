# demolegolilypadsd15
To create your lilypad workflow use the command above
creatad using [createlilypadconfyui](https://github.com/lucasespinosa28/createlilypadconfyui).
## To build
```bash
docker build . -f Dockerfile -t espinosa1991/demolegolilypadsd15:0.0. --target runner
```
## To run
```bash
docker run -it --gpus all -v $PWD/outputs:/outputs -e PROMPT='a lilypad in space' -e STEPS=30 espinosa1991/demolegolilypadsd15:0.0.
```
## To publish
```bash
docker push espinosa1991/demolegolilypadsd15:0.0.
```
## To run your worklow at lilypad
```bash
export WEB3_PRIVATE_KEY=<walletprivatekey>
lilypad rungithub.com/lucasespinosa28/democonfyuililypad:v1.0-i Prompt="RAW photo, <lora:lego_v2.0.768-000035:0.8> LEGO BrickHeadz, a dragon in a cave, (high detailed skin:1.2), 8k uhd, dslr, soft lighting, high quality, film grain, Fujifilm XT3" -e STEPS=30
```
