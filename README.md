# monero-crypto-miner

**IMPORTANT**: Before use please switch off your antivirus app or run it in a docker or vm to avoid removing of the file.

## Docker Version

1. copy config_template to config
```
cp -r config_template config
```
2. Replase Values in the config file on the line 94
3. Build docker
```
docker build . -t monero-miner
```
4. Run docker
```
docker run monero-miner
```