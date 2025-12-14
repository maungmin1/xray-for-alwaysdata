# xray for Alwaysdata

在 Alwaysdata Deploying an Xray node on a virtual host

## Project Features

* This project deploys xray on Alwaysdata, using the following solution: xray + WebSocket + VMess/Vless/Trojan/Shadowsocks + TLS
* The path can be customized or uses the default value: the UUID for vmess and vless, or the password for trojan and shadowsocks.
* If you encounter internet access issues after deployment, please check if the domain name is blocked. If so, you can use Cloudflare CDN or worker libraries to resolve the issue.

## deploy

* register [Alwaysdata](https://www.alwaysdata.com/)
*Create a web project
* Enter its SSH key and type the following command to download the project files.

```shell
wget -N https://github.com/Misaka-blog/xray-for-alwaysdata/raw/main/web.sh && chmod +x web.sh
```

* In the website settings, configure the startup items and environment variables as shown in the image below.

![image](https://user-images.githubusercontent.com/122191366/230263139-b461e5a4-c52a-4afe-b4ce-e36903ed6372.png)

* Environment variables used in the project
  | Variable name | Required | Default value | Remarks|
  | ------------ | ------ | ------ | ------ |
  | UUID         | No | de04add9-5c68-8bab-950c-08cd5320df18 | Can be generated online: https://www.uuidgenerator.net/ |
  | VMESS_WSPATH | No | /vmess | Starts with /|
  | VLESS_WSPATH | No | /vless | Starts with / |
  | TROJAN_WSPATH | No | /trojan | Starts with / |
  | SS_WSPATH | No | /shadowsocks | Starts with / |
  | NEZHA_SERVER | No | | IP address or domain name of the Nezha Probe server |
  | NEZHA_PORT | No | | The port of the Nezha Probe server|
  | NEZHA_KEY    | No | | Nezha Probe Client Only Key |

## Disclaimer

* This program is for educational purposes only and is not for profit. Please delete it within 24 hours of downloading. It may not be used for any commercial purposes. The text, data, and images are all copyrighted. If you reproduce it, please indicate the source.
* Use of this program requires adherence to the deployment disclaimer. Users must comply with the laws and regulations of the deployment server's location, its country, and the user's country. The program author is not responsible for any misconduct by the user.

## sponsor

Love Power：https://afdian.net/a/Misaka-blog

![afdian-MisakaNo の 小破站](https://user-images.githubusercontent.com/122191366/211533469-351009fb-9ae8-4601-992a-abbf54665b68.jpg)

