git 熟悉
---

參考 git 教學文件，請註冊/登入 github 並且創建一 repository 名稱任意。

0. 創 develop branch 並 init commit 設置一 python 檔案 main.py，內容
1. 確認 .gitignore 及相關的設定，別將文字編輯器暫存檔之類的檔案加進 git。
2. 在 develop branch，將當前 head 用 git merge 回 master branch。
3. 在 master branch 替 function 於首行加 print 使其能在 console 印出 hi。
4. 切到 develop branch，替 for loop 首行加 print 使其能在 console 印出 hello。
5. 將當前的 develop branch merge 回 master。
6. 附上 github 連結供我們確認 & 搞定！
> https://github.com/alamod951753/Practice_git.git

延伸：
1. main.py 裡 #benchmark 1. 與 #benchmark 2. 執行時間的差異是因為？
> 1st benchmark 是一個生成函數 generator，並無實際執行內部函數
2nd benchmark 因為有 list 會產生陣列數字，故執行次數較多

config 管理
---

參考 內容
1. 想請問這樣的 config 會如何進 git 與管理，config 的內容也要進 git 嗎？
> 使用 configparser，建制不同環境對應的 section及參數值，再進到 git 管理

python flask
---

參考 Flask 的 文件官網 和 Quickstart，試著新增一個 view。
1. 先照著文件官網架起 webserver 並能在本機透過瀏覽器連至 http://localhost/(domain name 不一定一樣, 也可用 ip 127.0.0.1)
2. 參考 Quickstart，新增一個 view 讓 http://localhost/3/4 可輸出 12，連結上的兩個數字相乘的結果，並有基本的防錯(比方說在連結給上字母等結果的話要輸出 only int is accepted)
3. 仿照 git 熟悉，也將結果上到 github 另一新 repository 並附上連結供我們確認，感謝！
> https://github.com/alamod951753/Practice_flask.git

延伸：
1. 文件官網中 @app.route("/") 的語法是如何達到的？
> app.route decorator 將路徑參數及執行函數，丟給根目錄 hello 函數

python sqlalchemy
---

參考 benchmark
1. 如果是 insert or update 的情形的話，benchmark script 該如何修改？ (部分 testcase 可能會直接無法用，可移除)
> 