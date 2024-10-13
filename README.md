<p style="font-size:14px" align="right">
<a href="https://t.me/airdropasc" target="_blank">Join our telegram <img src="https://user-images.githubusercontent.com/50621007/183283867-56b4d69f-bc6e-4939-b00a-72aa019d1aea.png" width="30"/></a>
</p>

<p align="center">
  <img height="300" height="auto" src="https://user-images.githubusercontent.com/109174478/209359981-dc19b4bf-854d-4a2a-b803-2547a7fa43f2.jpg">
</p>


# BRINXAI : DEPIN + AI CRYPTO PROJECT Earn Point Be Join CLI (ratio convert 1 Point = 0.7694 Tokens)

## Official Link
- [Discord](https://discord.gg/UFMxhNvT)
- [Twitter](https://x.com/BrinxAi_Labs/status/1838989932368642293)
- [Documentation](https://brinxai.gitbook.io/brinxai-depin-ai/worker-nodes-setup)

## Spek VPS Minimum

|  Hardware/VPS |  Minimum |
| ------------ | ------------ |
| CPU  | 4 or more physical CPU cores  |
| RAM | At least 6GB of memory (RAM) |
| Penyimpanan  | At least 300GB of SSD disk storage |
| Internet | At least 10mbps network bandwidth |

## Use Auto Install
```
curl -s https://data.zamzasalim.xyz/file/uploads/brinxai.sh | bash
```
## After sukses instalation
- Register on website : https://workers.brinxai.com/register.php?ref=4b1361b2
- Register with email
- Login
- Klik Add Node
- Node Name : brinxai
- Node IP Address : Submit your IP Vps
- Port : 5011
- Done
## Running More Models More Point
- Open Port
  ```
  sudo ufw allow 5003/tcp
  sudo ufw allow 5055/tcp
  sudo ufw allow 7000/tcp
  sudo ufw allow 3007/tcp
  sudo ufw enable
  ```
- Models text-ui service
  ```
  docker run -d --name text-ui --network brinxai-network --cpus=4 --memory=4096m -p 127.0.0.1:5003:5003 admier/brinxai_nodes-text-ui:latest
  ```
- Models stable-diffusion service
  ```
  docker run -d --name stable-diffusion --network brinxai-network --cpus=4 --memory=4096m -p 127.0.0.1:5055:5055 admier/brinxai_nodes-stabled:latest
  ```
- Models rembg service
  ```
  docker run -d --name rembg --network brinxai-network --cpus=2 --memory=2048m -p 127.0.0.1:7000:7000 admier/brinxai_nodes-rembg:latest
  ```
- Models upscaler service
  ```
  docker run -d --name upscaler --network brinxai-network --cpus=2 --memory=2048m -p 127.0.0.1:3007:3007 admier/brinxai_nodes-upscaler:latest
  ```
## Running Brinxai Relayer Node
```
bash <(curl -s https://data.zamzasalim.xyz/file/uploads/brinxai-relayer-node.sh)
```
## Kalo dah selesai maka tampilan dashboard akan seperti ini
<p align="center">
  <img src="https://github.com/zamzasalim/brinxai/blob/main/xx.png" alt="Image 1" width="400" />
  <img src="https://github.com/zamzasalim/brinxai/blob/main/xxx.png" width="350" />
</p>
