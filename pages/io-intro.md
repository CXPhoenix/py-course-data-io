---
layout: section
---

# 所有程式設計的基礎

## I/O {.font-mono}

---

# 什麼是 [I/O]{.font-mono}

所謂「[I/O]{.font-mono}」是指在電腦中最基本的兩個動作：**Input**{.font-mono} 和 **Output**{.font-mono}。

* **Input**{.font-mono} \
    要處理的資料「存放進」記憶體中，讓電腦可以進行後續處理。
* **Output**{.font-mono} \
    將記憶體中的資料「推出去」，展示處理好的資料，或是將資料存放到其他地方。

---

# 什麼是 [I/O]{.font-mono} （續）

<SlidevVideo controls class="w-160 mx-auto">
    <source src="/io-demo.mp4" type="video/mp4" />
    <p>你的瀏覽器沒有支援線上撥放影片，你可以從 <a href="/io-demo.mp4">這裡</a> 下載</p>
</SlidevVideo>

---

::center-flex-block {.text-3xl .pb-18}
:::div
基本上，學程式的第一件事情，就是學習 [I/O]{.font-mono style="display: inline;"}
:::
::

---

# 學習 Python 第一式

::center-flex-block {.font-mono .text-4xl .pb-18}
print("Hello World")
::

---

# ["Hello World"]{.font-mono} 的起源

* 這幾乎是所有程式設計人的共同回憶 [(ｏﾟﾛﾟ)┌┛Σ(ﾉ´*ω*`)ﾉ]{.font-mono}
* [1972]{.font-mono} 年，美國貝爾實驗室的 [Brian Wilson Kernighan]{.font-mono} 所著的「[A Tutorial Introduction to the Language B]{.font-mono}」以輸出這串文字作為教學內容。
* [1978]{.font-mono} 年，[Kernighan]{.font-mono} 正式於「[C]{.font-mono} 語言程式設計([The C Programming Language]{.font-mono})」以輸出這串文字作為基本輸入輸出的教學內容。

---

# ["Hello World"]{.font-mono} 的起源

::center-flex-block{.text-3xl .pb-16}
:::div
所以這段文字~~折磨了~~訓練無數程式設計師寫下第一行程式
:::
::

---

# print("Hello World") {.font-mono}

請在以下地方打上 `print("Hello World")`{.font-mono}
::div{.font-mono}
```py {monaco-run} { lineNumbers: 'on', autorun: false, height: '8rem', outputHeight: '4rem', editorOptions: { fontSize: 18 } }

```
::

---

# print("Hello World") {.font-mono .text-5xl}（續）

::p {.pt-4}
`print()`{.font-mono .text-5xl}
::

::p {.pl-8}
這個指令會把 `()`{.font-mono} 中的資料輸出到「標準輸出 [Standard Output]{.font-mono}」中。
::

::div {.mx-10 .mt-2 .p-1 .bg-yellow-200 .rounded-lg}
標準輸出 [Standard Output]{.font-mono}

:::div {.px-2}
電腦把資料「傳出去」的目標位置。基本上，通常指的就是「螢幕」。

所謂「標準」，就是指在沒有任何其他設定的情況下，預設的設定值。 {.text-xl .pl-8}

::::p{.text-xl .pl-8}
所以比起「標準」兩個字，我覺得用「**預設輸出**」更貼近真實情況。
::::
:::
::

---
layout: image
---

# print("Hello World") {.font-mono .text-5xl style="display: inline;"}（續）

![print函式](/print-function.png)


<!-- url: https://www.runoob.com/python3/python-func-print.html -->

---

# 補充：[stdio]{.font-mono}

* 所謂 [stdio]{.font-mono} 指的就是 **Standard Input/Output**{.font-mono} 
    ::p {.pt-3 .leading-9 style="text-indent: 2em;"}
    在電腦系統中，其實這類型的輸入輸出都是將資料放到「**檔案**」中，所以我們把資料**輸出**到 [Standard Output]{.font-mono} 時，其實就是在把資料寫入 [stdout]{.font-mono} 這個檔案中。
    ::
    ::p {.pt-3 .leading-9 style="text-indent: 2em;"}
    所以可不可以把 `print()`{.font-mono} 輸出到其他地方？當然可以！但是你得自己研究一下。
    ::

---

# `print`{.font-mono style="display: inline;"} 出資料

剛剛印出「[Hello World]{.font-mono}」有沒有發現前後都有[雙引號]{.underline .underline-offset-4}？

::::v-click
:::div {.mx-8 .mt-2 .p-1 .space-y-3 .bg-yellow-100 .rounded-lg}
::p{style="text-indent: 2em;"}
在 [Python]{.font-mono} 中，你所打的文字都會被認為是「指令」，也就是命令電腦的東東。
::
::p{style="text-indent: 2em;"}
如果要呈現「文字資料」，就得用 `"`{.font-mono} 或 `'`{.font-mono} 前後包起來才行。
::
:::
::::

::div {.mt-4 .px-8 .text-xl v-click}
例如你想要電腦讀文字資料「復興高中」，那麼你就得在程式碼中 [key]{.font-mono} 進 `"復興高中"`{.font-mono}
::

---

# `print`{.font-mono style="display: inline;"} 出資料（續）

那要印出數字呢？也需要這麼麻煩嗎？

## 那就給你試試看啦！ {.text-center}

::div {.font-mono}
```py {monaco-run} {lineNumbers: 'on', autorun: false, height: '6rem', editorOptions: { fontSize: 16 } }

```
::

---

# RECAP{.font-mono}

* 所謂 [I/O]{.font-mono} 指的是「輸入」與「輸出」這兩件事情。
* 輸出 ["Hello World"]{.font-mono} 是幾乎所有資訊人的共同回憶。
* `print()`{.font-mono} 會把 `()`{.font-mono} 中的資料傳到「標準輸出」。
* 對 [Python]{.font-mono} 來說，除了數字外，所有的字都是「指令」；所以如果要讓 [Python]{.font-mono} 知道這個東西是「文字資料」，那你要用 `"`{.font-mono} 或 `'`{.font-mono} 把文字包起來。