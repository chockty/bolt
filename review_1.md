
# Bolt PC
## 修正内容
### 1. 各sectionタグにある見出しの文字の大きさを統一する。
 #### index.html
 - 以下の箇所に class: title-font を追加しました。  
   44行目： ```<h1 class="white-text-format usability-text-title"> ```  
   55行目: ```<h1 class="works-title">```  
   94行目: ```<h1 class="title-format white-text-format skills-title">```
 - 44行目: class: ```usability-text-title``` を削除しました。
 #### style.css
 - ```.title-font``` を新規作成し、```font-size: 24px``` を適用しました。（21行目〜24行目）
 - 116行目 〜 119行目 class: ```usability-text-title``` を削除しました。
----------
### 2. Font Latoを使用する。
 #### style.css
 - 11行目: ```font-family: 'Raleway'``` を　```font-family: 'Lato';``` へ変更しました。
 - 23行目: ```.font-title``` へ ```font-family: 'Raleway';```　を追加しました。
 - 119行目: ```.usability-text-content``` へ ```font-family: 'Raleway';```　を追加しました。
----------
### 3. innerと同じ階層に別クラスを指定して、それぞれのセクションで同じ構造にする。
同じ構造 = innerと同じ階層のクラスで padding / margin を使用して余白を取る。
 #### index.html
 - 21行目: class: ```contact-btn``` を削除しました。
 - 54行目: ```<div class="inner">``` へ class: ```works-box``` を追加しました。
 - 93行目: ```<div class="inner">``` へ class: ```skills-box``` を追加しました。
 #### style.css
 - 60行目: ```.header-box``` へプロパティ ```align-items: center;``` ```padding: 15px 0;``` を追加しました。
 - 72行目: class: ```.contact-btn``` を削除しました。
 - 99行目: ```.usability``` のプロパティ ```padding-top: 50px;``` を削除しました。
 - 105行目: ```.usability-box``` へプロパティ ```padding-top: 50px;``` を追加しました。
 - ```.works-box``` を新規作成し、 ```padding: 60px 0 70px 0;``` を適用しました。（127行目〜129行目）
 - 132行目: ```.works-title``` のプロパティ ```padding: 60px 0 40px 0;``` を削除しました。
 - 140行目: ```.works-imgs``` へプロパティ ```margin-top: 60px;``` を追加しました。
 - 165行目: ```.works-email-box``` のプロパティ ```padding: 90px 190px 70px 120px;``` を ```padding: 90px 190px 0 120px;``` へ修正しました。
 - ```.skills-box```を新規作成し、 ```padding: 70px 0 100px 0;``` を適用しました。（187行目〜189行目）
 - 193行目: ```.skills-title``` へのプロパティ ```padding: 70px 0 70px 0;``` を削除しました。
 - 198行目: ```.skills-items``` へのプロパティ ```padding-bottom: 100px;``` を削除し、 ```margin-top: 70px;``` を追加しました。
---------- 
### 4. contactボタンの外側でもリンクにクリックできる状態なので修正する。
 #### style.css
 - 69行目: ```.fa-bolt``` のプロパティ ```padding: 15px 0;``` を削除しました。
