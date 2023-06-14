# Tag Filter プラグイン

![test reearth dev_published html_alias=idchebgbdb(1440 desktop) (1)](https://user-images.githubusercontent.com/21994748/183280643-7f183826-d48a-4faa-a5f6-93089ca91867.png)

## このプラグインについて
- Tag Filter プラグインは各レイヤーのタグを複数指定することで、条件に一致するレイヤーを絞り込んで表示することができる、フィルターの機能を果たすプラグインです。<br>
- このプラグインは[reearth-plugin-toolbox](https://github.com/airslice/reearth-plugin-toolbox)を利用して作成されています。

　
## 使用方法

### 準備
タグクラウドで制御したいレイヤーにタグを設定します。
![](https://github.com/airslice/reearth-plugin-tag-filter/assets/13118515/d3e64733-61cf-4c3c-84a1-46493e23a00c)

### 右パネルの設定項目
- Tag Filter リスト<br>
   検索対象のタググループのリストです。必要に応じて追加してください。ここで作成したリストが、Tag Filter上に検索対象のグループとして表示されます。<br>
    ![](https://github.com/airslice/reearth-plugin-tag-filter/assets/13118515/0b20711e-6051-423c-a513-f82f396ae76a)
- Tag Group Name <br>
    検索対象のタググループ名を指定します。Tag Filter リストの各項目に一つづつ設定します。<br>
    ![](https://github.com/airslice/reearth-plugin-tag-filter/assets/13118515/3d40e6e0-b495-4d94-85e8-10e3683f7f2c)
- Customize <br>
    ウイジェットUIの表示色をカスタマイズします。<br>
    ![](https://github.com/airslice/reearth-plugin-tag-filter/assets/13118515/072c6eb2-a54e-4b18-a94a-50e842698427)
    
    - Theme：ウィジェットのテーマカラーをDarkかLightから選択することができます。
    - Backgroung Color：ウィジェットの背景色を変更することができます。これを設定している場合、Themeの設定内容は無視されます。
    - Primary Color：Exportボタンの色を変更することができます。これを設定している場合、Themeの設定内容は無視されます。


(左：ThemeをDark、中央：ThemeをLight、右：BackgroundColorとPrimary Colorを指定)
![](https://github.com/airslice/reearth-plugin-tag-filter/assets/13118515/49871b34-ac57-43c2-aaa1-346cc8615a4c)
    
### 操作方法
- Tag Filter に表示されたタググループ名のスライドスイッチをオンにするとの検索対象のタグのリストが表示されます。リストをクリックすることで検索対象に追加されます。<br>
![](https://github.com/airslice/reearth-plugin-tag-filter/assets/13118515/30b681e5-a9a8-4bd6-a714-0bb65371857b)
- Search ボタンを押すと、検索条件にマッチしたレイヤーのみ表示され、それ以外は非表示になります。<br>
![](https://github.com/airslice/reearth-plugin-tag-filter/assets/13118515/6adc854b-caf8-40d9-b77e-8ab3f06c35de)

### 留意点
- 同一タググループ内で複数の条件を設定した場合、その条件は”または”（論理和）として検索されます。
- 複数のタググループ間での検索条件は"かつ”（論理積）として検索されます。
- 指定タググループ内のタグを持たないレイヤーは ... に分類されます。この場合 ... を検索条件として指定可能です。

## 備考
- テストブラウザ環境
  - OS:Mac OS Montery 12.6.5
  - ブラウザ：Google Chrome 112.0.5615.121

## 開発者欄

このプラグインは、Re:Earth公式プラグインです。

 ![](https://eukarya-inc.github.io/reearth-plugin-shinsuiNavi/src/logo-3.png)

ソースコードはこちら(https://github.com/airslice/reearth-plugin-tag-filter)

- コミュニティ

  - このプラグインを利用したプロジェクトをユーザーコミュニティでシェアしましょう。

  - このプラグインについての不明点がある場合にもここからRe:Earthチームや他の開発者に質問することができます。

  - Discordへのリンクはこちら(https://discord.gg/BXcQhvwqqM)
<br>
<br>

# Tag Filter

This is a Re:earth plugin made with [reearth-plugin-toolbox](https://github.com/airslice/reearth-plugin-toolbox).

Tag filter can be useful when show layers with tags in different dimensions. 

![test reearth dev_published html_alias=idchebgbdb(1440 desktop) (1)](https://user-images.githubusercontent.com/21994748/183280643-7f183826-d48a-4faa-a5f6-93089ca91867.png)

- Features:
  - Show several tag filter base on selected tag groups.
  - Each filter can be enable/disabled independently.
  - Filter layers (show/hide).

- Setup:
  - Add/remove/reorder tag group from Re:earth Earth Editor.
  - Type in the tag group name.

- Tips:
  - Layer will be visible when it has enabled tag in each enabled filter.
  - If a layer does not have any tags of selected tag group it will be list in a special tag `...`
