---
layout: section
---

# 變數

## 儲存資料的箱子

---

# 變數是什麼？

<iframe class="mx-auto pt-2" width="640" height="360" src="https://www.youtube.com/embed/GTNLZJD1Nio?si=urngIv0O7SPfWYhF" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---

# 變數 [Variable]{.font-mono}

* 儲存資料的地方
* 儲存進去的資料被稱為「值 [Value]{.font-mono}」
* 一次只能儲存**一筆**資料

---

# 變數 [Variable]{.font-mono}（續）

<SlidevVideo controls class="w-160 mx-auto">
    <source src="/variable-demo.mp4" type="video/mp4" />
    <p>你的瀏覽器沒有支援線上撥放影片，你可以從 <a href="/variable-demo.mp4">這裡</a> 下載</p>
</SlidevVideo>

---

# 變數可以被拿出來使用嗎？

## 當然可以！{.pl-4 .text-rose-600 v-click}

當我們建立起變數，把值放到變數中之後：{v-click}

::v-clicks
* 跟電腦「註冊」了這個變數名稱，這個變數名稱就變成一種「指令」。
* 只要撰寫這個「指令」，就是跟電腦說我們需要把資料從變數中「**複製**」出來使用。
::

---

# 使用變數

所以我們要輸出變數，就可以直接用 `print()`{.font-mono} 來處理。

電腦處理的過程大概如以下：

::div{.kg .font-mono .mt-4 .px-8}

````md magic-move {lines:true}
```py{*|1|2}
variable = 10
print(variable)
```
```py
print(10)
```
````
::

::p {.w-full .absolute .bottom-22 .text-center v-click="['1', '+1']"}
建立變數 `variable`{.font-mono}，並把數字資料 `10`{.font-mono} 存到變數中
::

::p {.w-full .absolute .bottom-22 .text-center v-click="['2', '+1']"}
將變數 `variable`{.font-mono} 放到 `print`{.font-mono} 中輸出
::

::p {.w-full .absolute .bottom-14 .text-center v-click="3"}
電腦執行時，會把 `variable`{.font-mono} 中存放的資料取出， \
交給 `print`{.font-mono} 輸出
::

<style scoped>
.kg * {
    font-size: 1.4rem;
    line-height: 2rem;
}
</style>

---

# 【重要】專業術語

::v-clicks
* 定義一個變數，我們稱為「宣告 [declare]{.font-mono}」 \
    意思是：跟電腦說，我們需要一個儲存資料的空間，並命名為某個名字。
* 將「值」存進變數中，我們稱為「賦值 [assigned]{.font-mono}」 \
    意思是：跟電腦說，我們將一個值放進這個儲存資料的空間中。
* 使用某個變數，我們稱為「呼叫 [call]{.font-mono}」
    意思是：跟電腦說，我們要將變數中的資料「**複製**」出來使用。
::

---

# 【重要】專業術語（續）

::center-flex-block {.gap-6 .pb-12}
:::div{.text-3xl}
在 [Python]{.font-mono .inline} 中，我們撰寫 `variable=5`{.font-mono .inline} 時，
:::
:::div{.text-3xl}
我們就是在進行「宣告」加上「賦值」。
:::
:::div{.text-3xl}
兩個願望，一次滿足 [(๑¯∀¯๑)]{.font-mono}
:::
::

---

# 宣告變數名稱時的注意事項

設定變數時，需要特別注意以下事項：{.pt-2}

::::div{.pl-14}
:::v-clicks
1. 第一個字**不能**{.text-rose-600 .text-3xl}用數字（半形）命名。
    ::p {.text-2xl}
    這跟語法解析器（[Parser]{.font-mono}）解析程式語法有關，容易造成錯誤。
    ::
2. **不能**{.text-rose-600 .text-4xl}使用「保留字 [Reserved Word]{.font-mono}」命名變數。
    ::p {.text-2xl}
    在 [Python]{.font-mono} 中會造成你無法使用那個關鍵字；其他程式語言則可能會在編譯時發生錯誤。
    ::
3. 不介意中文，但**不建議**{.text-rose-600 .text-5xl}中文。 
    ::p {.text-2xl}
    編解碼（[Encoding/Decoding]{.font-mono}）原始碼時可能產生問題。
    ::
:::
::::

---

# 宣告變數名稱時的習慣

撰寫 [Python]{.font-mono} 時，變數宣告有幾個比較習慣使用的命名風格：

::::div{.pl-14}
:::v-clicks
1. 小寫蛇式命名 [Lower Snake Case]{.font-mono}
    ::p{.text-2xl}
    e.g. `user_info`{.font-mono}、`one_time_password`{.font-mono}
    ::
2. 大寫駝峰式命名 [Upper Camel Case]{.font-mono}
    ::p{.text-2xl}
    e.g. `UserInfo`{.font-mono}、`OneTimePassword`{.font-mono}
    ::
3. 大寫蛇式命名 [Upper Snake Case]{.font-mono}
    ::p{.text-2xl}
    e.g. `USER_INFO`{.font-mono}、`ONE_TIME_PASSWORD`{.font-mono}
    ::
:::
::::

---

# 宣告變數名稱時的習慣（續）

以下命名方式在平常非常不建議：

::v-clicks
* 隨便命名：真的會忘記這個變數的用途。
* 與儲存的資料無關：然後你就忘記這個變數的用途。
* 命名時採用「駭客式命名 [L337 sp34k]{.font-mono}」： \
    `I d0n'7 b3l13v3 y0u c0u1d und3r574nd 7h15 l1n3!`{.font-mono}
::

---

# 宣告變數名稱時的習慣（續）

::center-flex-block {.gap-6 .pb-16}
:::div{.text-3xl}
但我在寫 [APCS]{.font-mono} 不想寫這麼多字，想省時間怎麼辦？
:::

:::div{.text-3xl v-click}
那就用 [Ninja Code]{.font-mono} 吧！
:::
::

::p{.absolute .bottom-12 .right-6 .-rotate-12 v-click}
`a=1`{.font-mono}、`N=input()`{.font-mono} 之類的
::

---
python:
    stdin: 
        - 恭喜你學會最基本的 I/O 讀寫
---

# 實作時間

::p {.pl-5}
你能否把輸入的資料放到變數後，在 `print()`{.font-mono} 出來？
::

::p {.text-lg .pl-8}
我把輸入的資料隱藏起來，所以試著讀取輸入、輸出看看會出來什麼吧 [ლ(・´ｪ`・ლ)]{.font-mono}
::

::div{.font-mono .pt-2 .px-6}
```py {monaco-run} { lineNumbers: 'on', height: '14rem', autorun: false, editorOptions: { fontSize: 16 } }
input()
```
::

---

# 實作時間（續）

::p {.pl-5}
變數一次只能存一筆資料，但是這是真的嗎？
::

::div{.font-mono .pt-2 .px-6}
```py {monaco-run} { lineNumbers: 'on', height: '14rem', autorun: false, editorOptions: { fontSize: 14 } }
var = 5
print(var)
var = 10
# 現在 var 變成多少？
```
::

---

# 補充：[APCS]{.font-mono} 的考法

::p{.pl-4 style="text-indent: 2em;" v-click}
雖然在 [APCS]{.font-mono} 中會有範例測試資料，但在實際上你提交給系統判斷（我們稱為 [Judger]{.font-mono} 系統）時，具體輸入什麼資料、會輸出什麼資料我們並不知道喔！
::

::p{.pl-4 style="text-indent: 2em;" v-click}
所以我們 [APCS]{.font-mono} 要拿高分，很考驗你如何幫電腦「**寫公式**{.text-rose-600}」，讓電腦只要按照「**公式**」就可以完成資料處理，算出所要求的解答。
::

::p{.pl-4 style="text-indent: 2em;" v-click}
我們把寫出來的公式稱為「**演算法**{.text-rose-600 .text-4xl}」。
::

---

# RECAP{.font-mono}

::v-clicks
* 變數，是儲存資料的地方，並且為這個空間給了一個名字。
* 當我們撰寫 `var=5`{.font-mono} 時，就是在進行「宣告」一個變數 `var`{.font-mono}，並把數字 `5`{.font-mono} 「賦值」給 `var`{.font-mono}。
* 變數，一次只能存一筆；若將原本的變數重新賦值，那麼舊的值就會消失不見。
* 我們可以直接在 `print()`{.font-mono} 中呼叫變數，讓 `print()`{.font-mono} 把變數中存的資料輸出。
::