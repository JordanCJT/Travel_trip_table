# 中国行程表

一个不需要服务器的行程网页：时间表、地址、备注和路线地图。行程数据放在 `itinerary.xlsx` 里，用 Excel 或 WPS 编辑就行。

## 文件

- `index.html` 网页本身
- `itinerary.xlsx` 行程表（编辑这个）
- `vendor/xlsx.full.min.js` 读取 Excel 用的库（不要删）
- `.nojekyll` 让 GitHub Pages 原样发布文件

## 放到 GitHub 上（只做一次）

1. 登录 github.com，点右上角 “+” → New repository，起个名字（例如 `china-trip`），选 Public，创建。
2. 在新仓库页面点 “uploading an existing file”（或 Add file → Upload files），把这个文件夹里的所有文件拖进去。`vendor` 文件夹和 `.nojekyll` 也要上传。点 Commit changes。
3. 进入仓库的 Settings → Pages。Source 选 “Deploy from a branch”，Branch 选 `main`，文件夹选 `/ (root)`，点 Save。
4. 等 1 到 2 分钟，页面顶部会出现网址，格式是 `https://你的用户名.github.io/china-trip/`。把这个网址发到 WhatsApp 群。

注意：Public 仓库任何人知道网址都能看到行程。行程里有航班、酒店之类的私人信息时，请不要写进表格。

## 修改行程

- **在自己电脑上改：** 用 Excel 打开 `itinerary.xlsx`，改完保存。想先看效果，可以双击打开 `index.html`，点 “载入我的表格” 选择这个文件。
- **让大家看到新版本：** 在 GitHub 仓库里点 `itinerary.xlsx` → 右上角 “…” → Delete，再 Add file → Upload files 上传新的同名文件。或者直接把新文件拖进仓库页面，选择覆盖。1 到 2 分钟后，同一个网址就会显示新内容。
- **家人修改后：** 把改好的 `itinerary.xlsx` 发给负责更新的人，由他上传到 GitHub。

## 表格怎么填

见 `itinerary.xlsx` 里的“说明”工作表。简单说：天数、时间、地点、城市、地址、备注、纬度、经度，地点必填，其他可以留空。
