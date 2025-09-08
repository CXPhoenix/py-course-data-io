---
layout: section
---

# 資料輸入

## `input()`{.font-mono style="display: inline;"} 的使用

---

::center-flex-block{classNames="gap-4"}
:::div{.text-4xl}
忘記 **I/O**{.font-mono} 的人記得看[這裡](/4){.text-sky-500 .underline .underline-offset-2}
:::

![wow](/wow.gif){.w-100}
::

---

# 用 `input()`{.font-mono} 進行資料輸入

:::v-clicks
::ul {.mt-2}
* 這邊的 `input()`{.font-mono} 是指「當程式運作時，從標準輸入（[Standard Input]{.font-mono}）讀取資料的一個**指令功能**。
* 所謂 [Standard Output]，通常指**鍵盤**{.text-rose-600 .text-4xl .underline .underline-offset-4}（或滑鼠，看系統）。
* 放在 `()`{.font-mono} 中的，是提示別人要輸入什麼資料。
* 不想放提示？當然也沒差！ \
    甚至 [APCS]{.font-mono} 考試時，**千萬不要放**{.text-rose-600 .text-4xl}。
::
:::

---

::center-flex-block{.pb-12}
但是輸入後的資料如何看到？

:::p
這就需要搭配 `print()`{.font-mono} 來處理了
:::
::

---

# `input()`{.font-mono} 輸入資料

::div{.pt-4 .mx-6}
※因為網頁版本關係，所以使用者的輸入會放在 `# stdin: `{.font-mono} 後面
::

::div {.font-mono .py-4 .px-4}
```py {monaco-run} { lineNumbers: 'on', height: '14rem', autorun: false, editorOptions: { fontSize: 14 } }
# stdin: Hello
# ==== code below... ====

```
::

---

# `input()`{.font-mono} 後的資料...？

::center-flex-block {.gap-6 .pb-12}
:::div {.text-3xl v-click}
難道 `input()`{.font-mono} 後只能輸出嗎？
:::
:::div {.text-3xl v-click}
又或者是，`input()`{.font-mono} 進來的資料會放在哪裡？
:::
:::div {.text-4xl v-click}
這就要講到「變數 [Variable]{.font-mono}」啦
:::
::

---

# RECAP{.font-mono}

::v-clicks
:::ul{.pt-2}
* `input()`{.font-mono} 是**程式執行時**，從 [Standard Output]{.font-mono} 讀入資料的功能。
* [Standard Output]{.font-mono} 標準輸入，通常是指從**鍵盤**進行的輸入。
* `input()`{.font-mono} 中的 `()`{.font-mono} 放的是「輸入提示」（用於提示執行程式的人這邊要輸入什麼）。
* 在 [APCS]{.font-mono} 考試時，**不要**{.text-rose-600 .text-4xl}放輸入提示。
* 如果要存放讀入的資料，需要搭配**變數**。
:::
::