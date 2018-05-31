---
layout: post
title: 安裝Python與Packages
subtitle: How to Install Python and Packages
date: 2018-05-31
author: Chien-Jens
tags: Python Install Package
comments: true
signature: true
---

## Step1. 
- 從<a href="https://www.python.org/downloads/" target="_blank">Python</a>選擇符合自己電腦版本的安裝檔。

<br/>

## Step2. 
- 開啟安裝檔。
- 先勾選 **Add PythonX.X to PATH** `X.X會根據下載版本的不同而改變`
- 再選擇 **Cutomize installation**
![placeholder](/img_posts/pyinstall01.jpg "step2.")

<br/>

## Step3. 
- 點選**Next** <br/>
![placeholder](/img_posts/pyinstall02.jpg "step3.")

<br/>

## Step4.
- `<改變安裝路徑>`
- 原先Default的路徑會藏在C槽的深處，為了之後方便起見，<br/>
**強烈建議**自行在適當位置建一個新資料夾，將Python安裝在那個地方！
- 更改完畢後點選Install。
![placeholder](/img_posts/pyinstall03.jpg "step4.")

<br/>

## Step5. 
- 就等他安裝完成吧！

<br/>

## Step6. `<以下為安裝所需Package的步驟>`
- 點選**開始**→搜尋**cmd**→以系統管理員身分執行cmd<br/>
![placeholder](/img_posts/pyinstall04.jpg "step6.")

<br/>

## Step7.
- 改變路徑至Python內的**Scripts**資料夾<br/>
Ex: 如安裝Python於C槽的Python資料夾中(C:/Python)，<br/>
則Scripts會位於C:/Python/Scripts
- 在cmd輸入`cd C:/Python/Scripts`
![placeholder](/img_posts/pyinstall05.jpg "step7.")

<br/>

## Step8. 
- 透過`pip install`的方式安裝套件
- 資料科學常用套件為：<br/>
&nbsp;&nbsp;1. scikit-learn<br/>
&nbsp;&nbsp;2. pandas<br/>
&nbsp;&nbsp;3. numpy
<br>則可以透過：<br/>
&nbsp;&nbsp;`pip install scikit-learn`<br/>
&nbsp;&nbsp;`pip install pandas`<br/>
&nbsp;&nbsp;`pip install numpy`<br/>
來安裝這些套件。
- 資料科學套件當然還有很多，且**大部分**都可透過`pip install`來安裝，<br/>
但有些套件確實需要使用別的方法才能安裝成功，於最後再進行補充說明！
![placeholder](/img_posts/pyinstall06.jpg "step8.")

<br/>

## Step9. `<此步驟為安裝Sypder IDE>`
- 如自己有慣用或預計要使用的IDE，則可忽略這一步！
- 我一開始使用了Python內建的IDLE約一年，的確是比較累一點點，<br/>
後來就載了Sypder IDE，介面確實比較友善。

- 同`Step7.`，接著輸入`pip install spyder`
- 安裝完畢後到Scripts資料夾中尋找**spyder3**應用程式
- 可透過右鍵將**spyder3**釘選到工作列以方便使用~<br/>
<del>截圖的電腦是我第一次裝Python的電腦，**無腦的按Next**後果就是像我圖中的路徑一樣冏</del>
![placeholder](/img_posts/pyinstall07.jpg "step9.")

<br/>

## Step10. 
- 打開Python，透過`import XXX`的方式確認套件是否安裝成功。

-------------------------------------------------------------------------------------


## 補充說明
有些套件的確透過`pip install`無法有效安裝，<br/>
此時就需要嘗試另一種方式：**下載whl檔進行安裝**
- <a href="https://www.lfd.uci.edu/~gohlke/pythonlibs/" target="_blank">這個地方</a>幾乎擁有你安裝不了的東西(至少我是這樣XDD)
- 在上述網址`ctrl+F`找尋你要的package
- 尋找相對應的版本，如果你的Python是3.6，就找檔名含有`cp36-cp36m`的 <br/>
然後再根據自己OS的不同選擇`win32` or `amd64` 下載
- **下載後的檔案請放到scripts資料夾中**
- 接著同`Step7.`，<br/>
然後輸入`pip install XXX‑X.X.X‑cpXX‑cpXXm‑win_XX.whl` <br/>
`<XX則是你下載的完整檔名，記得加上副檔名.whl>`
- 等他安裝完成就可以了~

<br/>

以上是Python安裝的小小心得~ <br/>
我是新手~希望可以幫到更新的新手XDD
