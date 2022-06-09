# subject-220609

### Visual Studio Code 周りのノウハウ
![image](https://user-images.githubusercontent.com/1501327/172763639-9c3c7b66-9eda-4164-a275-affd436c17ed.png)

### reg-menu のメンテナンス
- ### レジストリのフォルダの右クリックの定義 => HKEY_CLASSES_ROOT\Directory

### 掲示板 4 - 5 の比較

### [jQuery の構築テスト](https://toolbox.winofsql.jp/html-page.php)
```html
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/5.0.1/css/bootstrap.min.css">
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.6.0/jquery.min.js"></script>

<script>

$(function(){

	$("form").on( "submit", function(){

		var name = $("#name").val();

		name = name.trim();

		console.log(name);

		if( name == "" ) {
			alert("お名前を入力してください");
			event.preventDefault();
		}

	});

});

</script>

<div id="title" class="alert alert-primary">てすと</div>
        <form action="https://winofsql.jp/"
            target="_self"
            method="POST">
            <div>
                <span class="title_entry">
                    タイトル
                </span>
                <input
                    type="text"
                    name="subject"
                    >
            </div>
            <div>
                <span class="title_entry">
                    お名前
                </span>
                <input
                    type="text"
                    name="name"
                    id="name"
                    >
            </div>
            <div>
                <textarea name="text" id="text"></textarea>
            </div>
            <div>
                <input type="submit" name="send" value="送信">
            </div>
            <input name="datetime" id="datetime">
        </form>
```
