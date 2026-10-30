

  "name": "dsh-skin-sakura",
  "version": "0.3.2",
  "description": "DSH Web GUI 背景皮肤：给工作区与首页换一张背景（不碰侧边栏与窗口标题栏），设置里可调",
  "keywords": [
    "dsh",
    "dsh-plugin",
    "theme",
    "wallpaper",
    "skin"
  ],
  "license": "MIT",
  "type": "module",
  "main": "index.js",
  "repository": {
    "type": "git",
    "url": "git+https://github.com/beiqiping-boop/DeepSeek-Harness-pulg-in.git"
  },
  "homepage": "https://github.com/beiqiping-boop/DeepSeek-Harness-pulg-in#readme",
  "bugs": {
    "url": "https://github.com/beiqiping-boop/DeepSeek-Harness-pulg-in/issues"
  },
  "exports": {
    ".": "./index.js",
    "./client": "./client.js",
    "./package.json": "./package.json"
  },
  "files": [
    "index.js",
    "client.js",
    "cordis.patch.yml",
    "LICENSE",
    "README.md",
    "CHANGELOG.md"
  ],
  "dsh": {
    "bundle": {
      "patch": "./cordis.patch.yml"
    },
    "client": {
      "platform": "web",
      "inject": [
        "@deepseek-ai/dsh-client-runtime",
        "@deepseek-ai/dsh-client-ui-settings",
        "@deepseek-ai/dsh-client-ui-settings-plugins"
      ]
    }
  }
}
