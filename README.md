## `manifest.json`

```js
{
  "name": "Desktop Capture",
  "description": "Allow you to capture your desktop for use in video apps",
  "version": "0.1.0",
  "manifest_version": 2,
  // 要运行的 js 文件
  "background": {
    "scripts": ["extension.js"],
    // 表明运行的文件不会驻存 CPU，按需执行
    "persistent": false
  },
  "externally_connectable": {
    "matches": ["*://localhost/*"]
  },
  "permissions": ["desktopCapture"]
}
```

## `extension.js`