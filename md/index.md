# 正規表現 チュートリアル

## 正規表現ってこうゆうの

=== "Python"

    ``` python linenums="1"
    import re

    target = "001-111-1234"
    pattern = r"\d{3}\D\d{3}\D\d{4}"

    prog = re.compile(pattern=pattern)

    result = prog.findall(target)

    print(result)
    # >>> ['001-111-1234']

    ```

## 解説

### 正規表現
|001|-|111|-|1234|
|----|----|----|----|----|
|\d{3}|\D|\d{3}|\D|\d{4}|
|数字３桁|数字以外の文字（空白含む）|数字３桁|数字以外の文字（空白含む）|数字４桁|




[Next](1_1.md){ .md-button }