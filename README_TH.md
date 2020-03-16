# Tokyo COVID-19 Task Force website

![](https://github.com/tokyo-metropolitan-gov/covid19/workflows/production%20deploy/badge.svg)

[![Tokyo COVID-19 Task Force website](https://user-images.githubusercontent.com/1301149/75629392-1d19d900-5c25-11ea-843d-2d4376e3a560.png)](https://stopcovid19.metro.tokyo.lg.jp/)


### [日本語](./README.md) | [English](./README_EN.md) | [Spanish](./README_ES.md) | [Korean](./README_KO.md) | [Chinese (Taiwan)](./README_ZH_TW.md) | [Chinese (Simplified)](./README_ZH_CN.md) | [Vietnamese](./README_VI.md) | [Thai](./README_TH.md)


## การร่วมพัฒนา (How to Contribute)

เปิดรับการพัฒนาและอัพเดทต่างๆ!
โปรดอ่าน [How to contribute](./.github/CONTRIBUTING_TH.md)

## จรรยาบรรณ (Code of Conduct)

โปรดอ่าน [Code of conduct for developers](./.github/CODE_OF_CONDUCT_TH.md)

## ลิขสิทธิ์ (License)
ซอฟต์แวร์อยู่ภายใต้ลิขสิทธิ์ [the MIT License](./LICENSE.txt).

## สำหรับนักพัฒนา (For Developers)

### การติดตั้งโปรแกรมเพื่อการพัฒนา (How to Set Up Environments)

- ต้องการ Node.js เวอร์ชั่น: 10.19.0 หรือสูงกว่า

**ใช้ yarn**
```bash
# install dependencies
$ yarn install

# serve with hot reload at localhost:3000
$ yarn dev
```

**ใช้ docker**
```bash
# serve with hot reload at localhost:3000
$ docker-compose up --build
```

### การแก้ปัญหา `Cannot find module ****` error

**ใช้ yarn**
```bash
$ yarn install
```

**ใช้ docker**
```bash
$ docker-compose run --rm app yarn install
```

[please translate me]
### VSCode + Remote Cotainersで開発する場合

1. VSCodeの拡張機能「[Remote Development](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack)」を導入します。
2. [この画像（外部サイト）](https://code.visualstudio.com/docs/remote/containers#_quick-start-try-a-dev-container)のように左下部の「Open Folder in Container」でこのリポジトリのルートを選択すれば環境構築が始まります。

[Topic]
- 設定を変更したい場合は、`.devcontainer/devcontainer.json`を修正してください。<br/>
    詳細は[devcontainer.jsonのリファレンス](https://code.visualstudio.com/docs/remote/containers#_devcontainerjson-reference)を参照してください。
- Remote Container実行時のみ有効な拡張機能「ESlint」を導入していますが、必要に応じて`devcontainer.json`の`extensions`に追加してください。<br/>
    詳細な手順は[こちら（外部サイト）](https://code.visualstudio.com/docs/remote/containers#_managing-extensions)を参照してください。
- 開発環境を再構築する場合は、左下部の「Rebuild Container」を実行してください。
[/please translate me]

### ขั้นตอนการ Deploy ไปยัง Production (Deployment to Staging & Production Environments)

ถ้า 'master' ได้รับการแก้ไขหรือปรับปรุง HTML จะถูกสร้างและส่งไปยัง 'production' โดยอัตโนมัติ
และ เว็บไซต์ (https://stopcovid19.metro.tokyo.lg.jp/) จะได้รับการอัพเดท

ถ้า 'staging' ได้รับการแก้ไขหรือปรับปรุง HTML จะถูกสร้างและส่งไปยัง 'gh-pages' โดยอัตโนมัติ
และ เว็บไซต์ (https://stg-covid19-tokyo.netlify.com/) จะได้รับการอัพเดท

ถ้า 'development' ได้รับการแก้ไขหรือปรับปรุง HTML จะถูกสร้างและส่งไปยัง 'dev-pages' โดยอัตโนมัติ
และ เว็บไซต์ (https://dev-covid19-tokyo.netlify.com/) จะได้รับการอัพเดท