# Bolt PC（2回目）
## 修正内容

### 1. header分でthemeのセクションが低くなっている。
 #### index.html
 - ```<main class="main-content">``` を追加しました。
 #### style.css
 - ```.main-content { padding-top: 70px; }``` を追加しました。
 - ```.theme-box { padding: 320px 0 250px 0; }```　を  ```padding: 250px 0 250px 0``` へ修正しました。
----------
### 2. class: theme　の見出しが pタグ になっている。
 #### index.html
 - ```<p class="main-theme-title"></p>``` を ```<h1 class="main-theme-title"></h1>``` へ修正しました。
----------
### 3.<ul><li>　を使用するところでsectionを使用している。
  #### index.html
  - worksセクションのclass: ```works-imgs``` の sectionタグをulタグへ変更しました。
  - worksセクションのclass: ```works-link``` をliタグで囲みました。
  - worksセクションのaタグに付与されていたclass: ```works-link``` を liタグへ移動させました。
  - skillsセクションのclass: ```skills-items``` のsectionタグをulタグへ変更しました。
  - skillsセクションのclass: ```skills-item``` をliタグで囲みました。
  - snsセクションのclass: ```sns-box```　のsectionタグをulタグへ変更しました。
  - snsセクションのclass: ```sns-icon-link``` をliタグで囲みました。
----------
### 4. 「Email Me!」のボタンの外でリンクが押せる状態になっている。
  #### style.css
  - ```.works-email-btn``` のプロパティ ```width: 140%;``` を削除しました。
  - ```.works-email-box``` のプロパティを修正しました。（内容： ```padding: 90px 190px 0 120px;``` → ```margin: 90px auto 0 auto;```）
  - ```.works-email-box``` のプロパティに ```width: 69%; align-items: baseline;``` の2つを追加しました。
----------
### 5. ```font-family: 'Raleway'``` が複数記述されている。
 #### index.html
 - class: ```.main-theme-title　.usability-text-content``` のあるタグに class:```font-Raleway``` を追加しました。
 #### style.css
 - ```.font-Raleway { font-family: 'Raleway'; }``` を新規に作成しました。
 - class: ```.main-theme-title　.usability-text-content```　から　```font-family: 'Raleway';``` を削除しました。
----------
### 6. imgタグのalt未記載。
  #### index.html
  - usabilityセクションのimgタグに ```alt="iphone"``` を追記しました。
  - worksセクションの各imgタグに ```alt="work(各写真の番号)" を追記しました。
  - skillsセクションの角imgタグに ```alt="(各スキルの名称)" を追記しました。
----------
### 7. footerのテキストにて、pタグを2回使わず一行で表記する必要がある。
  #### index.html
  - ```<p>Crafted with</p> <i class="fas fa-heart"></i> <p>by BlackTie.co.</p>``` を ```<p>Crafted with <i class="fas fa-heart"></i>by BlackTie.co.</p>```へ変更しました。
  #### style.css
  - class: ```.footer-text``` のプロパティ ```display: flex;  float: right;``` を削除し、```text-align: right``` を追加しました。
