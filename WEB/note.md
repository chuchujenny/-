# 第二天啟軒三個練習目的:
1.資料處理
2.事件處理
3.取得資料

(作業參考寫法在手機相片裡)

#database
database寫完指令可以刪除沒關係~因為他已經存入硬碟了

ppt.P52 
若要輸入多筆資料，要加'分號'
INSERT INTO Customer(id, first_Name, last_Name)
VALUES (1, 'Steven','Jobs');

INSERT INTO Customer(id, first_Name, last_Name)
VALUES (2, 'Elon','Musk')

# 教材連結:

## DAY1
早上至青~~~[簡單web的html (有pdf)](https://www.icloud.com/keynote/0s68Z2LE4Lj3giuMSDiaKsxEA#X-Village_Web_Course_intro)
https://www.icloud.com/keynote/0ArIvYcrYEmyRW9HOHFdu2d3A#X-Village_HTML_and_CSS_Web_Course



下午伯駿~~[html與CSS (有pdf)](https://www.icloud.com/keynote/0AA7I3OGHU9qjNE7VHCAlJusA#css_layout)
Keynote 版
超連結要 點擊播放後才可以 使用
另外也可以點擊左上角的按鈕，再點"顯示發表人附註"，會有更詳細的說明在下面

[參考用github:](https://github.com/Sirius207/X-Village-CSS-Layout/tree/master/code)
https://sirius207.github.io/X-Village-CSS-Layout/code/2.3.3/
https://css-tricks.com/fighting-the-space-between-inline-block-elements/

## DAY2
早上啟軒~~[JS (有pdf)](https://www.icloud.com/keynote/09a5IjB3IHrCHfcoeMjfxYLJw#X-Village_JavaScript_Web_Course)
[答案:](https://github.com/x-village/x-village-web-js-course/tree/solution)

下午博安~~[Database(有pdf)](https://www.icloud.com/keynote/06TwNe9cNNMPVB_avwU0DpaHA#Database)
## DAY3

博安~~只有pdf檔 flask
李唯~~ [進階flask與powerman](https://www.icloud.com/keynote/0boYz4dEgGj-KW3qMw6xv58gA#CRUD_in_Flask)
https://speakerdeck.com/xvillage
https://github.com/x-village/web-acccounting-example/blob/master/views.py
## 作業
[作業要求](https://hackmd.io/u4sfbja6QeqqPCGVyJpceQ)
[作業前端程式碼](https://gist.github.com/Sirius207/47166f886011768ae4b5a23a52eecfc5)
[CRUD補充簡報](https://hackmd.io/p/ByNEty38m#/)

## 參考資料
補充一些前端的教學資源(有些有出現在簡報內)

Make a Website (第一天早上的內容)
https://www.codecademy.com/learn/make-a-website

CSS 排版 (第一天下午的內容)(也是有中文版)
http://learnlayout.com/ 

Javascript
JavaScript 101 快速入門教學
https://blog.techbridge.cc/2017/01/14/javascript101-tutorial/

jQuery
https://www.codecademy.com/learn/learn-jquery


=====================================
[Flask 作業補充]

Q1: 有辦法編輯index.html後，不要重開 flask 就可以看到更改的樣子嗎？
A: 在寫 Todo List 時(用flask 跑)，如果希望編輯 index.html 後 "不用重開 flask ，只要重新刷新頁面 " 就可以看到更新後的結果的話，可以先在終端機下一行
export FLASK_ENV=development 
(或者你是 windows 就用下面這一行)
SET FLASK_ENV=development 

上面這一行的意義是設定環境變數 為 開發模式

接下來再下 flask run 就會看到 debug mode: on 顯示，這時就可以直接刷新不用重開了

Ref: http://flask.pocoo.org/docs/1.0/quickstart/#debug-mode
在終端機直接執行 flask run 這時運作的會是 production模式

---

Q2: 前端設定了 "點擊工作項目後把工作項目劃掉" 跟 "點擊刪除按鈕後刪除工作項目" 兩種事件，但後者 "點擊刪除按鈕" 時也會觸發前者"劃掉的事件" (因為刪除按鈕在工作項目內)，有辦法避免嗎？

A: 看下面這篇
https://blog.hellojcc.tw/2015/11/05/dom-element-event-flow/

或者看 JS 30 的 day 25也可
https://javascript30.com/
https://guahsu.io/2017/10/JavaScript30-25-Event-Capture-Propagation-Bubbling-and-Once/

實務上再 Google 一下 jquery event stopPropagation 的用法
https://www.google.com.tw/search?q=jquery+event+stoppropagation&rlz=1C5CHFA_enTW728TW728&oq=jquery+event+stop&aqs=chrome.0.0j69i57j69i60l2j0l2.7676j0j1&sourceid=chrome&ie=UTF-8