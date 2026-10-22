# 中国行程表

一个不需要服务器的行程网页：时间表、地址、备注、路线地图，以及可以直接复制到 WhatsApp 群的每日行程文字。可以直接在网页的“编辑”页修改行程，不用先导入 Excel。`itinerary.xlsx` 是网页打开时默认显示的行程。

## 文件

- `index.html` 网页本身
- `itinerary.xlsx` 网页默认显示的行程（可以用 Excel 或 WPS 编辑）
- `vendor/xlsx.full.min.js` 读取 Excel 用的库（不要删）
- `.nojekyll` 让 GitHub Pages 原样发布文件

## 放到 GitHub 上（只做一次）

1. 登录 github.com，点右上角 “+” → New repository，起个名字（例如 `china-trip`），选 Public，创建。
2. 在新仓库页面点 “uploading an existing file”（或 Add file → Upload files），把这个文件夹里的所有文件拖进去。`vendor` 文件夹和 `.nojekyll` 也要上传。点 Commit changes。
3. 进入仓库的 Settings → Pages。Source 选 “Deploy from a branch”，Branch 选 `main`，文件夹选 `/ (root)`，点 Save。
4. 等 1 到 2 分钟，页面顶部会出现网址，格式是 `https://你的用户名.github.io/china-trip/`。把这个网址发到 WhatsApp 群。

注意：Public 仓库任何人知道网址都能看到行程。行程里有航班、酒店之类的私人信息时，请不要写进表格。

## 修改行程

1. 打开网页，点“编辑”页。点“添加一行”添加，直接在格子里改，点“删除”删掉（删除后几秒内可以点“撤销”）。
2. 改动会**自动保存在这台设备的浏览器里**。刷新、关掉再打开都还在。
3. 家人用自己的手机或电脑打开同一个网址，看到的是网站上的版本。每个人的修改只保存在自己的设备上，不会互相同步。
4. **要让所有人看到你的修改：** 在“编辑”页点“导出 Excel”，得到 `itinerary.xlsx`。到 GitHub 仓库里 Add file → Upload files，上传这个文件覆盖旧的，1 到 2 分钟后同一个网址就会显示新内容。
5. 想放弃自己设备上的修改，点页面上方黄色提示里的“恢复为网站版本”。

注意：清除浏览器数据，或换了设备，设备上保存的修改会丢失。重要的修改请记得导出 Excel 备份。

也可以先在 Excel 里改好 `itinerary.xlsx`，在“编辑”页点“导入表格”选择它，或复制表格内容粘贴进去。

## 表格怎么填

见 `itinerary.xlsx` 里的“说明”工作表。简单说：天数、时间、类别、地点、城市、地址、备注、纬度、经度，地点必填，其他可以留空。类别可选景点、早餐、午餐、晚餐、住宿、交通、其他、标题。

## 复制到 WhatsApp

改好行程后，打开网页的“分享文字”，可以选择是否显示地址和备注，然后点“复制这一天”或“复制全部行程”，粘贴到 WhatsApp 群。
