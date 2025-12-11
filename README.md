# Gemini CLI

本仓库主要是 添加了 apiEndpoint 用于配置成自定义的gemini上游代理

```shell
npm install && npm run bundle
```

卸载官方版本

```shell
npm uninstall -g @google/gemini-cli
```

```shell
sudo ln -s "$(pwd)/bundle/gemini.js" /usr/local/bin/gemini
```

配置文件 ~/.gemini/settings.json

```json
{
  "security": {
    "auth": {
      "selectedType": "gemini-api-key"
    }
  },
  "model": {
    "name": "gemini-2.5-pro",
    "apiEndpoint": "https://xxxxxxxxx"
  },
  "ui": {
    "theme": "Default"
  }
}
```
