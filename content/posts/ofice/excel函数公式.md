---
title: "Excel函数公式" #标题
date: 2024-10-09T18:39:38+08:00 #创建时间
lastmod: 2024-10-09T18:39:38+08:00 #更新时间
author: ["yfc01"] #作者
categories: 
- ofice
tags: 
- excel函数公式
- ofice
description: "excel中的函数运算功能是数据处理的重要工具" #描述
weight: # 输入1可以顶置文章，用来给文章展示排序，不填就默认按时间排序
slug: ""
draft: false # 是否为草稿
comments: true #是否展示评论
showToc: true # 显示目录
TocOpen: false # 自动展开目录
hidemeta: false # 是否隐藏文章的元信息，如发布日期、作者等
disableShare: true # 底部不显示分享栏
showbreadcrumbs: false #顶部显示当前路径
cover:
    image: "" #图片路径：posts/tech/文章1/picture.png
    caption: "" #图片底部描述
    alt: ""
    relative: falsew
---

excel中的函数运算功能是数据处理的重要工具，熟练运用该工具能大大提高使用excel进行数据处理的速度。

## 运算符

在 Excel 中，运算符用于执行各种数学、逻辑和文本操作。不同类型的运算符允许用户在单元格中进行计算、比较值或连接文本。以下是 Excel 中常用的运算符分类及其详细介绍：

<table border="1" cellspacing="0" cellpadding="5">
  <tr>
    <th>运算符类型</th>
    <th>运算符符号</th>
    <th>描述</th>
    <th>示例</th>
  </tr>
  <tr>
    <td rowspan="6">算术运算符</td>
    <td>+</td>
    <td>加法，两个数相加</td>
    <td>=5 + 3 结果是 8</td>
  </tr>
  <tr>
    <td>-</td>
    <td>减法，从一个数中减去另一个数</td>
    <td>=10 - 4 结果是 6</td>
  </tr>
  <tr>
    <td>*</td>
    <td>乘法，两个数相乘</td>
    <td>=7 * 2 结果是 14</td>
  </tr>
  <tr>
    <td>/</td>
    <td>除法，一个数除以另一个数</td>
    <td>=8 / 2 结果是 4</td>
  </tr>
  <tr>
    <td>^</td>
    <td>幂运算，计算一个数的幂次</td>
    <td>=3 ^ 2 结果是 9</td>
  </tr>
  <tr>
    <td>%</td>
    <td>百分比运算</td>
    <td>=50% 结果是 0.5</td>
  </tr>
  <tr>
    <td rowspan="6">比较运算符</td>
    <td>=</td>
    <td>等于，比较两个值是否相等</td>
    <td>=A1 = B1</td>
  </tr>
  <tr>
    <td>&lt;&gt;</td>
    <td>不等于，比较两个值是否不相等</td>
    <td>=A1 &lt;&gt; B1</td>
  </tr>
  <tr>
    <td>&gt;</td>
    <td>大于，比较左边的值是否大于右边</td>
    <td>=A1 &gt; B1</td>
  </tr>
  <tr>
    <td>&lt;</td>
    <td>小于，比较左边的值是否小于右边</td>
    <td>=A1 &lt; B1</td>
  </tr>
  <tr>
    <td>&gt;=</td>
    <td>大于或等于，比较左边的值是否大于或等于右边</td>
    <td>=A1 &gt;= B1</td>
  </tr>
  <tr>
    <td>&lt;=</td>
    <td>小于或等于，比较左边的值是否小于或等于右边</td>
    <td>=A1 &lt;= B1</td>
  </tr>
  <tr>
    <td>文本运算符</td>
    <td>&</td>
    <td>连接符，将两个文本连接在一起</td>
    <td>="Hello" &amp; " World"</td>
  </tr>
  <tr>
    <td rowspan="3">引用运算符</td>
    <td>:</td>
    <td>范围运算符，表示从一个单元格到另一个单元格的区域</td>
    <td>=SUM(A1:A10)</td>
  </tr>
  <tr>
    <td>,</td>
    <td>将多个不连续的单元格或区域结合</td>
    <td>=SUM(A1, A3, A5)</td>
  </tr>
  <tr>
    <td>空格</td>
    <td>交集运算符，返回两个区域中共同的单元格</td>
    <td>=SUM(A1:A5 B2:B6)</td>
  </tr>
  <tr>
    <td rowspan="3">逻辑运算符</td>
    <td>AND</td>
    <td>逻辑与，所有条件满足时返回 TRUE</td>
    <td>=AND(A1&gt;1, B1&lt;10)</td>
  </tr>
  <tr>
    <td>OR</td>
    <td>逻辑或，任一条件满足时返回 TRUE</td>
    <td>=OR(A1&gt;1, B1&lt;10)</td>
  </tr>
  <tr>
    <td>NOT</td>
    <td>逻辑非，条件为 TRUE 时返回 FALSE</td>
    <td>=NOT(A1&gt;1)</td>
  </tr>
  <tr>
    <td rowspan="2">范围运算符</td>
    <td>-</td>
    <td>范围减法，用于排除某些单元格</td>
    <td>=SUM(A1:A10 - A5:A8)</td>
  </tr>
  <tr>
    <td>!</td>
    <td>引用其他工作表的单元格</td>
    <td>=Sheet1!A1</td>
  </tr>
  <tr>
    <td>条件运算符</td>
    <td>IF</td>
    <td>条件判断运算符，根据条件返回不同的值</td>
    <td>=IF(A1&gt;10, "大于", "小于")</td>
  </tr>
</table>


在 Excel 中，运算符的优先级决定了表达式中各个运算符执行的顺序。默认情况下，运算从高优先级到低优先级依次进行。如果运算符具有相同的优先级，则按照从左到右的顺序计算。

以下是运算符的优先级顺序，从高到低：

1. **括号** `( )`：括号内的运算最先执行，用于强制改变默认的运算顺序。
2. **引用运算符** `:`、`空格`、`,`：这些运算符用于单元格范围的引用操作。
3. **负号** `-`：用于表示负数。
4. **百分比** `%`：将数值转换为百分比。
5. **幂运算** `^`：用于计算幂次。
6. **乘法和除法** `*`、`/`：这两个运算符的优先级相同。
7. **加法和减法** `+`、`-`：这两个运算符的优先级相同。
8. **连接符** `&`：用于连接文本字符串。
9. **比较运算符** `=`、`<>`、`>`、`<`、`>=`、`<=`：用于比较数值或文本。

如果表达式中有多个运算符，可以使用括号明确控制优先级。例如，在 `=(2 + 3) * 4` 中，括号内的加法先执行，结果为 `5`，然后再进行乘法，最终结果为 `20`。



## 相对引用和绝对引用

在 Excel 中，**绝对引用**和**相对引用**是两种常见的引用方式，它们决定了当复制或拖动单元格公式时，引用的单元格是否会发生变化。

### 相对引用

相对引用是 Excel 默认的引用方式。当你复制或拖动公式到其他单元格时，公式中引用的单元格会根据新位置自动调整。这种引用方式对引用的位置进行相对的计算。

- 形式：`A1`，`B2`，`C3` 等。
- 特点：行和列都会根据公式的位置变化自动调整。
- 适用场景：当你希望公式在不同位置使用不同的单元格时，使用相对引用。

**示例：**
假设在单元格 `B1` 中有一个公式 `=A1 + 1`，如果你将该公式复制到 `B2`，公式会自动变为 `=A2 + 1`，引用的单元格从 `A1` 变为了 `A2`。

### 绝对引用

绝对引用使用美元符号 (`$`) 来锁定行或列，使引用的单元格在公式复制或拖动时保持不变。无论公式移到哪里，引用的单元格始终指向相同的位置。

- 形式：`$A$1`，`$B$2`，`$C$3` 等。
- 特点：行和列都不会发生变化，始终指向固定的单元格。
- 适用场景：当你希望公式无论复制到哪里，始终引用同一个单元格时，使用绝对引用。

**示例：**
在单元格 `B1` 中有公式 `=$A$1 + 1`，如果将该公式复制到其他位置（如 `B2`），公式仍然是 `=$A$1 + 1`，始终引用单元格 `A1`。

### 混合引用

混合引用是绝对引用和相对引用的组合，允许你锁定行或列中的一个，而另一个随公式位置改变。

- 形式：`$A1`（锁定列，行随位置变化），或 `A$1`（锁定行，列随位置变化）。
- 特点：只锁定行或列中的一个，灵活度更高。
- 适用场景：当你只需要锁定行或列中的某一个时，可以使用混合引用。

**示例：**

- `=$A1`：锁定列 `A`，行号随着公式复制到不同位置而改变。
- `=A$1`：锁定行 `1`，列号随着公式复制到不同位置而改变。

在使用 Excel 公式时，根据需求选择相对引用或绝对引用，能更灵活地管理公式行为。



## 函数

### 逻辑函数

- [IF 函数](https://support.microsoft.com/zh-cn/office/if-函数-69aed7c9-4e8a-4755-a9bc-aa8bbff73be2)：`IF` 函数是 Excel 中的一种逻辑函数，允许用户根据特定条件返回不同的结果。其基本语法为 `IF(条件, 值_if_true, 值_if_false)`，其中“条件”是需要判断的逻辑表达式，“值_if_true”是在条件为真时返回的值，“值_if_false”是在条件为假时返回的值。通过使用 `IF` 函数，用户可以轻松处理不同情况，并根据条件动态生成结果。
- [IFERROR 函数](https://support.microsoft.com/zh-cn/office/iferror-函数-c526fd07-caeb-47b8-8bb6-63f3e417f611)：`IFERROR` 函数是 Excel 中用于处理错误的函数，它能够检测公式或表达式是否产生错误，并根据情况返回用户指定的值。其基本语法为 `IFERROR(值, 错误值)`，其中“值”是要检查的表达式或公式，“错误值”是在检测到错误时要返回的替代结果。通过使用 `IFERROR` 函数，用户可以避免在工作表中显示错误信息（如 `#DIV/0!` 或 `#N/A`），而是提供更友好的提示或替代值，从而提高数据的可读性和可靠性。
- [AND 函数](https://support.microsoft.com/zh-cn/office/and-函数-5f19b2e8-e1df-4408-897a-ce285a19e9d9)：`AND` 函数是 Excel 中的逻辑函数，用于检查多个条件是否都为真。它接受多个条件作为参数，如果所有条件都为真，则返回 `TRUE`，否则返回 `FALSE`。该函数常用于复杂的条件判断中，特别是当你希望确保多个条件同时满足时。它可以与 `IF` 函数等其他函数结合使用，以实现更复杂的逻辑判断。
- [OR 函数](https://support.microsoft.com/zh-cn/office/or-函数-7d17ad14-8700-4281-b308-00b131e22af0)：`OR` 函数是 Excel 中的逻辑函数，用于检查多个条件中是否至少有一个为真。它接受多个条件作为参数，只要有一个条件为真，函数就返回 `TRUE`，如果所有条件都为假，才会返回 `FALSE`。`OR` 函数常用于需要判断多个可能性是否成立的情况，特别是在需要满足任意一个条件时。它也可以与 `IF` 等函数结合使用，构建更复杂的逻辑判断。
- [NOT 函数](https://support.microsoft.com/zh-cn/office/not-函数-9cfc6011-a054-40c7-a140-cd4ba2d87d77)：`NOT` 函数是 Excel 中的逻辑函数，用于反转条件的逻辑值。它接受一个条件作为参数，如果该条件为 `TRUE`，`NOT` 函数会返回 `FALSE`；如果条件为 `FALSE`，它会返回 `TRUE`。`NOT` 常用于需要颠倒某个逻辑判断的场景，或者与其他逻辑函数如 `AND` 和 `OR` 结合使用，创建更复杂的判断逻辑。例如，可以用 `NOT` 来检查某个条件不成立的情况。

### 文本函数

- [LEFT、LEFTB 函数](https://support.microsoft.com/zh-cn/office/left-leftb-函数-9203d2d2-7960-479b-84c6-1ea52b99640c)：`LEFT` 函数是 Excel 中的文本函数，用于从文本字符串的左侧提取指定数量的字符。它接受两个参数，第一个参数是要提取字符的文本，第二个参数是需要提取的字符数。`LEFT` 常用于从文本中提取固定长度的前缀，比如提取电话号码的区号或产品编号的前几位。如果第二个参数省略，默认提取第一个字符。通过使用 `LEFT`，你可以灵活地处理和分割文本数据。
- [RIGHT、RIGHTB 函数](https://support.microsoft.com/zh-cn/office/right-rightb-函数-240267ee-9afa-4639-a02b-f19e1786cf2f)：`RIGHT` 和 `RIGHTB` 函数用于从文本字符串的右侧提取指定数量的字符。`RIGHT` 函数根据字符数来提取，例如，如果从单词 "Excel" 提取 2 个字符，结果是 "el"。而 `RIGHTB` 函数根据字节数提取字符，主要用于双字节字符集 (DBCS) 语言，如中文、日文等，因此每个汉字占两个字节，而英文字符只占一个字节。这个区别在处理双字节字符集时尤为重要。
- [MID、MIDB 函数](https://support.microsoft.com/zh-cn/office/mid-midb-函数-d5f9e25c-d7d6-472e-b568-4ecb12433028)：`MID` 函数用于从文本字符串的指定位置开始，提取一定数量的字符。你可以通过提供起始位置和要提取的字符数量来获取子字符串。例如，对于文本 "Excel Functions"，使用 `MID` 提取从第 7 个字符开始的 9 个字符，结果将是 "Functions"。它非常适合在较长的文本中提取特定部分，常用于数据清理和文本操作。
- [LEN、LENB 函数](https://support.microsoft.com/zh-cn/office/len-lenb-函数-29236f94-cedc-429d-affd-b5e33d2c67cb)：`LEN` 函数用于计算文本字符串中的字符总数，包括字母、数字、符号和空格。它能够快速返回字符串的长度，对于检查输入数据的字符数量或清理数据非常有用。例如，`LEN("Excel 123")` 的结果是 9，因为空格和数字也被计算在内。这个函数在处理文本数据时非常常用。
- [LOWER 函数](https://support.microsoft.com/zh-cn/office/lower-函数-3f21df02-a80c-44b2-afaf-81358f9fdeb4)：`LOWER` 函数是 Excel 中用于将文本字符串中的所有字母转换为小写字母的函数。其语法为 `LOWER(text)`，其中 `text` 是你想要转换为小写的文本。无论输入的字母是大写还是混合大小写，`LOWER` 函数都会将其全部转换为小写。这个函数常用于文本规范化，尤其是在需要对大小写不敏感的数据进行比较或处理时。例如：`=LOWER("Hello World")` 的结果是 `hello world`。
- [UPPER 函数](https://support.microsoft.com/zh-cn/office/upper-函数-c11f29b3-d1a3-4537-8df6-04d0049963d6)：`UPPER` 函数是 Excel 中用于将文本字符串中的所有字母转换为大写字母的函数，语法为 `UPPER(text)`，其中 `text` 是要转换为大写的文本。无论输入的字母是小写还是混合大小写，`UPPER` 函数都会将其全部转换为大写，常用于文本格式化和标准化数据。例如，`=UPPER("Hello World")` 的结果为 `HELLO WORLD`。
- [SUBSTITUTE 函数](https://support.microsoft.com/zh-cn/office/substitute-函数-6434944e-a904-4336-a9b0-1e58df3bc332)：`SUBSTITUTE` 函数是 Excel 中用于替换文本字符串中指定字符或子字符串的函数，语法为 `SUBSTITUTE(text, old_text, new_text, [instance_num])`。其中，`text` 是要进行替换的原始文本，`old_text` 是要被替换的字符或子字符串，`new_text` 是用于替换的新字符或子字符串，而可选参数 `instance_num` 指定要替换的实例编号（如果省略则替换所有实例）。此函数常用于文本处理和数据清理，例如将字符串中的特定词汇替换为其他内容。示例：`=SUBSTITUTE("I love apples", "apples", "oranges")` 的结果为 `I love oranges`。
- [REPLACE、REPLACEB 函数](https://support.microsoft.com/zh-cn/office/replace-replaceb-函数-8d799074-2425-4a8a-84bc-82472868878a)：`REPLACE` 和 `REPLACEB` 函数是 Excel 中用于替换文本字符串中特定位置的字符的函数。`REPLACE` 的语法为 `REPLACE(old_text, start_num, num_chars, new_text)`，其中 `old_text` 是要进行替换的原始文本，`start_num` 是开始替换的位置，`num_chars` 是要替换的字符数，`new_text` 是用于替换的新字符。`REPLACEB` 函数则是专为使用双字节字符集（如中文或日文）设计的，其语法相似，`REPLACEB(old_text, start_num, num_bytes, new_text)`，这里的 `num_bytes` 指定要替换的字节数。两个函数常用于文本处理，尤其在需要替换特定位置字符时。示例：`=REPLACE("Hello World", 7, 5, "Excel")` 的结果为 `Hello Excel`。
- [FIND、FINDB 函数](https://support.microsoft.com/zh-cn/office/find-findb-函数-c7912941-af2a-4bdf-a553-d0d89b0a0628)：`FIND` 和 `FINDB` 函数是 Excel 中用于查找文本字符串中特定字符或子字符串的位置的函数。`FIND` 的语法为 `FIND(find_text, within_text, [start_num])`，其中 `find_text` 是要查找的字符或子字符串，`within_text` 是要搜索的原始文本，`start_num` 是可选参数，表示从哪个位置开始查找，默认从第一个字符开始。`FINDB` 函数则是专为使用双字节字符集（如中文或日文）设计，其语法为 `FINDB(find_text, within_text, [start_num])`，其中 `find_text` 和 `within_text` 的含义相同，但在计数上以字节为单位。两个函数常用于文本处理，特别是在需要定位特定字符或子字符串的位置时。示例：`=FIND("W", "Hello World")` 的结果为 `7`，表示字母 `W` 在字符串中的位置。
- [SEARCH、SEARCHB 函数](https://support.microsoft.com/zh-cn/office/search-searchb-函数-9ab04538-0e55-4719-a72e-b6f54513b495)：`SEARCH` 和 `SEARCHB` 函数是 Excel 中用于查找文本字符串中特定字符或子字符串的位置的函数。`SEARCH` 的语法为 `SEARCH(find_text, within_text, [start_num])`，其中 `find_text` 是要查找的字符或子字符串，`within_text` 是要搜索的原始文本，`start_num` 是可选参数，表示从哪个位置开始查找，默认从第一个字符开始。与 `FIND` 函数不同，`SEARCH` 函数不区分大小写，并且支持使用通配符。`SEARCHB` 函数则是专为使用双字节字符集（如中文或日文）设计，其语法类似，`SEARCHB(find_text, within_text, [start_num])`，同样以字节为单位进行计数。两个函数常用于文本处理，特别是在需要查找字符或子字符串位置时，示例：`=SEARCH("W", "Hello World")` 的结果为 `7`，表示字母 `W` 在字符串中的位置。
- [TRIM 函数](https://support.microsoft.com/zh-cn/office/trim-函数-410388fa-c5df-49c6-b16c-9e5630b479f9)：`TRIM` 函数是 Excel 中用于去除文本字符串开头和结尾处多余空格的函数，同时也会将多个空格压缩为一个空格。其语法为 `TRIM(text)`，其中 `text` 是要处理的文本字符串。该函数常用于数据清理，尤其是在从外部源导入数据时，可以有效去除不必要的空格，从而提高数据的整洁性和准确性。需要注意的是，`TRIM` 函数只会删除 ASCII 空格字符（32），而不会去除其他非打印字符。示例：`=TRIM("   Hello   World   ")` 的结果为 `"Hello World"`。
- [TEXT 函数](https://support.microsoft.com/zh-cn/office/text-函数-20d5ac4d-7b94-49fd-bb38-93d29371225c)：`TEXT` 函数是 Excel 中用于将数字转换为文本格式的函数，同时可以指定数字的显示格式。其语法为 `TEXT(value, format_text)`，其中 `value` 是要转换的数字，`format_text` 是指定的格式代码。此函数非常实用，可以用于将日期、货币和其他数字格式化为易于阅读的文本形式，例如，将数字转换为特定的货币格式或日期格式。示例：`=TEXT(1234.56, "$#,##0.00")` 的结果为 `"$1,234.56"`，将数字格式化为带有美元符号和千位分隔符的文本。
- [VALUE 函数](https://support.microsoft.com/zh-cn/office/value-函数-257d0108-07dc-437d-ae1c-bc2d3953d8c2)：`VALUE` 函数是 Excel 中用于将文本字符串转换为数字的函数。其语法为 `VALUE(text)`，其中 `text` 是要转换的文本字符串。此函数特别适用于将以文本格式存储的数字转换为可以进行数学计算的实际数字，确保在执行数学运算时不会出现错误。例如，如果单元格中存储的值为 `"123.45"`（文本格式），使用 `VALUE` 函数可以将其转换为数字 `123.45`。示例：`=VALUE("123.45")` 的结果为 `123.45`，使得该值可以用于进一步的计算。

### 查找和引用函数

- [LOOKUP 函数](https://support.microsoft.com/zh-cn/office/lookup-函数-446d94af-663b-451d-8251-369d5e3864cb)：`LOOKUP` 函数是 Excel 中用于查找某个值并返回对应结果的函数，能够在一维或二维数组中进行查找。其基本语法为 `LOOKUP(lookup_value, lookup_vector, [result_vector])`，其中 `lookup_value` 是要查找的值，`lookup_vector` 是包含要查找值的范围，而可选的 `result_vector` 是要返回结果的对应范围。如果未提供 `result_vector`，则返回 `lookup_vector` 中与 `lookup_value` 相同位置的值。`LOOKUP` 函数可用于查找和提取信息，尤其适合处理排好序的数据。需要注意的是，该函数在查找时不支持模糊匹配，只会返回匹配项或最后一个小于该值的项。例如，`=LOOKUP(5, A1:A5, B1:B5)` 会查找范围 A1:A5 中的值 5，并返回 B1:B5 中对应的值。