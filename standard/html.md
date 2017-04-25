# HTML代码规范

与代码格式化相关不做强制要求，建议使用Atom（Beautify Editor contents）webStorm（refomat code）统一美化代码。

## 语言规范

  1. `doctype`声明使用`html5`。

    ```html
    <!doctype html>
    ```

  2. 统一页面编码格式为`utf-8` , `meta`标签`charset`设置为`utf-8`;

    ```html
    <meta charset="utf-8" />
    ```

  3. 标签、标签属性全部小写。

    ```html
    <a href="/" data-attr="attr">Home</a>

    ```

  4. 所有html标签必须有结束符，`<img />`, `<col />`, `<base />`, `<link />`, `<meta />`, `<input />` 除外。

  5. 标签自定义属性使用`data-name="value"`的形式来写, 如果自定义属性特别多, 可以考虑使用标准 json 的方式去写: `data-json='{"a":"a", "b":"b"}'`。

    ```html
    <div data-json='{"a":1, "b":true, "c":[1, 2]}' ></div>
    ```

  6. 对于 JS 钩子, 以 `js-CamelCase` 的驼峰形式来命名。

  7. 对于普通`class`或者`id`命名（此处id仅在特殊情况下做样式，不做js钩子）, 统一使用小写字母, 第一个字符必须为字母, 连接符用中划线 `-`。

    ```html
    <div class="sns-box"></div>
    <div class="box"></div>
    ```

  8. css 引用置于头部`<head>`标签内。

  9. js 引用置于底部`</body>`标签前。

## 注释规范

  1. 主要的`html`模块需加注释

  2. 修改别人代码时, 加入修改信息。至少加入修改者大名和修改时间。

    ```html
    <!--主要修改IE8浏览器兼容性问题 XX 2013-09-26 13:21 -->
    ```

## 其他注意

  1. 开发时页面原则上不内嵌`style`、`script`代码，如特殊情况请标明并注释。
