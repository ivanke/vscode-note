# Visual Studio Code note

![Visual Studio Code about](res/img/vscode_about.jpg)

## 設定 Settings
### 分類
vscode 的 Settings 依作用範圍的不同，分為兩類
- User
  - 作用範圍：全域
- Workspace
  - 作用範圍：工作目錄
  - vscode 會將設定存在該工作目錄的 **.vscode/settings.json** 檔案中
### 如何進入設定
1. 在 Command Palette 執行 "**settings**" 指令
   - Command Palette 快速鍵：**Ctrl+Shift+P**
2. 選擇 **Preferences: Open User Settings**，即可進入 **Settings** 畫面

![picture 6](res/img/162644d542071cf901263b98f04dbff5f59688e19cc5ccf27370552e787b2077.png)

### Settings GUI 與 JSON 切換
**Settings** 有分為 **GUI** 與 **JSON** 模式，可用 **Settings** 畫面右上角的按鈕切換

![picture 5](res/img/90a148fa365324ed82001ce7e86785dd7628833485ff33eaca558c2d71587311.png)

### Settings User 與 Workspace 切換
切換 **User** 與 **Workspace** 的 **Settings** 畫面

![picture 7](res/img/cf5707b389b51bf4d86e36cf1202d017019a48fd4e7a7d13d10c9c1be3283cbe.png)

### 快速鍵 (Windows)
#### 常用
1. Quick Open, Go to File: **Ctrl + P** 或 **Ctrl + E**
   - 加上 **>** 符號，會變成 Command Palette
   - 加上 **@** 符號，會變成 Go to Symbol
   - 加上 **:** 符號，會變成 Go to line
     - 功能：後面接第幾行數字就會跳至該行。
2. Command Palette: **Ctrl + Shift + P** 或 **F1**
   - 功能：show and run command
3. Go to Symbol: **Ctrl + Shift + O**
   - 功能：在 **@** 符號後加上關鍵字，可搜尋 Module、Class、Function、Variable... 等名稱。
4. User Settings: **Ctrl + ,**

#### 編輯
- 複製整行：**Ctrl + C**
  - 游標沒有圈選文字時才有作用
- 剪下整行：**Ctrl + X**
  - 游標沒有圈選文字時才有作用
- 刪除整行：**Ctrl + Shift + K**
- 移動整行 (往上／下移動)：**Alt + ↑/↓**
- 複製整行 (往上／下複製)：**Alt + Shift + ↑/↓**
- 新增游標後一行 (Insert Line Below)：**Ctrl + Enter**
- 新增游標前一行 (Insert Line Above)：**Ctrl + Shift + Enter**
- 依序選取相同的字串：**Ctrl + D**
- 同時選取相同的字串：**Ctrl + F2**
- 縮排：**Ctrl + ]**
- 取消縮排：**Ctrl + [**

##### 多行編輯 (multi-cursor and selection)
- 插入多個輸入游標：**Alt + Click**
- 垂直插入輸入游標：**Ctrl + Alt + ↑/↓**
- 選取多行：Shift + Alt + 按住滑鼠左鍵拖曳
  - 滑鼠拖曳時只有垂直移動的話，效果會與 **垂直插入輸入游標** 一樣

#### 摺疊程式碼
1. 摺疊該區塊程式碼：**Ctrl + Shift + [**
   - 英文：Fold (collapse) region
2. 取消摺疊（展開）該區塊程式碼：**Ctrl + Shift + ]**
   - 英文：Unfold (uncollapse) region
3. 摺疊所有程式碼：**Ctrl + K, Ctrl + 0**
4. 摺疊至第 n 層的程式碼：**Ctrl + K, Ctrl + [n]**
   - 會只把第一層 { } 部分摺疊：**Ctrl + K, Ctrl + 1**
   - 會只把第二層 { } 部分摺疊：**Ctrl + K, Ctrl + 2**
   - 會只把第三層 { } 部分摺疊：**Ctrl + K, Ctrl + 3**
   - 只針對指定的層級作折疊，不會影響到其它層級
5. 取消摺疊（展開）所有程式碼：**Ctrl + K, Ctrl + J**

#### 終端機
- 開啟終端機 (terminal)：**Ctrl + `**
- 建立一個新的終端機分機：**Ctrl + Shift + `**

#### Run and Debug
- start debugging：F5
  - 開始執行 debug 模式
- run without debugging：Ctrl + F5
  - 執行，但沒有 debug 功能
- stop debugging：Shift + F5
- toggle breakpoint：F9
  - 加一個中斷點
- step over：F10
  - 執行這一行
- continue：F5
  - 往下執行，直到下一個中斷點
- restart debugging：Ctrl + Shift + F5

#### 自定義
- 開啟 Keyboard Shortcuts 設定畫面
  - 方法一：快速鍵 **Ctrl + K, Ctrl + S**
  - 方法二：點擊左下角管理圖示(齒輪)，選擇 **Keyboard Shortcuts**
- 大小寫轉換
  - 轉換為大寫
    - 在 Keyboard Shortcuts 設定畫面使用關鍵字 **Uppercase** 搜尋
    - 找到 **Transform to Uppercase** 項目
    - 點擊左邊的 **Add Keybinding** (加號)
    - 按住 **Ctrl + Alt + U**，錄製按鍵完成後按 enter
  - 轉換為小寫
    - 搜尋 **Lowercase** 找到 **Transform to Lowercase** 項目
    - 按住 **Ctrl + Alt + L**，錄製按鍵完成後按 enter

參考
1. [官方 Visual Studio Code 快速鍵一覽表 | POY CHANG](https://blog.poychang.net/vscode-shortcuts/)
2. [十分鐘快速掌握 Markdown | 卡斯伯 Blog](https://www.casper.tw/development/2019/11/23/ten-mins-learn-markdown/)
