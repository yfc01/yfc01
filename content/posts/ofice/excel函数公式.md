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

| **函数**                                                     | **说明**                                                     |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| [IF 函数](https://support.microsoft.com/zh-cn/office/if-函数-69aed7c9-4e8a-4755-a9bc-aa8bbff73be2) | 指定要执行的逻辑检测                                         |
| [IFERROR 函数](https://support.microsoft.com/zh-cn/office/iferror-函数-c526fd07-caeb-47b8-8bb6-63f3e417f611) | 如果公式的计算结果错误，则返回您指定的值；否则返回公式的结果 |
| [AND 函数](https://support.microsoft.com/zh-cn/office/and-函数-5f19b2e8-e1df-4408-897a-ce285a19e9d9) | 如果其所有参数均为 TRUE，则返回 TRUE                         |
| [OR 函数](https://support.microsoft.com/zh-cn/office/or-函数-7d17ad14-8700-4281-b308-00b131e22af0) | 如果任一参数为 TRUE，则返回 TRUE                             |
| [NOT 函数](https://support.microsoft.com/zh-cn/office/not-函数-9cfc6011-a054-40c7-a140-cd4ba2d87d77) | 对其参数的逻辑求反                                           |

### 文本函数

| **函数**                                                     | **说明**                                       |
| :----------------------------------------------------------- | :--------------------------------------------- |
| [LEFT、LEFTB 函数](https://support.microsoft.com/zh-cn/office/left-leftb-函数-9203d2d2-7960-479b-84c6-1ea52b99640c) | 返回文本值中最左边的字符                       |
| [RIGHT、RIGHTB 函数](https://support.microsoft.com/zh-cn/office/right-rightb-函数-240267ee-9afa-4639-a02b-f19e1786cf2f) | 返回文本值中最右边的字符                       |
| [MID、MIDB 函数](https://support.microsoft.com/zh-cn/office/mid-midb-函数-d5f9e25c-d7d6-472e-b568-4ecb12433028) | 从文本字符串中的指定位置起返回特定个数的字符   |
| [LEN、LENB 函数](https://support.microsoft.com/zh-cn/office/len-lenb-函数-29236f94-cedc-429d-affd-b5e33d2c67cb) | 返回文本字符串中的字符个数                     |
| [LOWER 函数](https://support.microsoft.com/zh-cn/office/lower-函数-3f21df02-a80c-44b2-afaf-81358f9fdeb4) | 将文本转换为小写                               |
| [UPPER 函数](https://support.microsoft.com/zh-cn/office/upper-函数-c11f29b3-d1a3-4537-8df6-04d0049963d6) | 将文本转换为大写形式                           |
| [SUBSTITUTE 函数](https://support.microsoft.com/zh-cn/office/substitute-函数-6434944e-a904-4336-a9b0-1e58df3bc332) | 在文本字符串中用新文本替换旧文本               |
| [REPLACE、REPLACEB 函数](https://support.microsoft.com/zh-cn/office/replace-replaceb-函数-8d799074-2425-4a8a-84bc-82472868878a) | 替换文本中的字符                               |
| [FIND、FINDB 函数](https://support.microsoft.com/zh-cn/office/find-findb-函数-c7912941-af2a-4bdf-a553-d0d89b0a0628) | 在一个文本值中查找另一个文本值（区分大小写）   |
| [SEARCH、SEARCHB 函数](https://support.microsoft.com/zh-cn/office/search-searchb-函数-9ab04538-0e55-4719-a72e-b6f54513b495) | 在一个文本值中查找另一个文本值（不区分大小写） |
| [TRIM 函数](https://support.microsoft.com/zh-cn/office/trim-函数-410388fa-c5df-49c6-b16c-9e5630b479f9) | 删除文本中的空格                               |
| [TEXT 函数](https://support.microsoft.com/zh-cn/office/text-函数-20d5ac4d-7b94-49fd-bb38-93d29371225c) | 设置数字格式并将其转换为文本                   |
| [VALUE 函数](https://support.microsoft.com/zh-cn/office/value-函数-257d0108-07dc-437d-ae1c-bc2d3953d8c2) | 将文本参数转换为数字                           |

### 查找和引用函数

| **函数**                                                     | **说明**                                             |
| :----------------------------------------------------------- | :--------------------------------------------------- |
| [LOOKUP 函数](https://support.microsoft.com/zh-cn/office/lookup-函数-446d94af-663b-451d-8251-369d5e3864cb) | 在向量或数组中查找值                                 |
| [VLOOKUP 函数](https://support.microsoft.com/zh-cn/office/vlookup-函数-0bbc8083-26fe-4963-8ab8-93a18ad188a1) | 在数组第一列中查找，然后在行之间移动以返回单元格的值 |
| [HLOOKUP 函数](https://support.microsoft.com/zh-cn/office/hlookup-函数-a3034eec-b719-4ba3-bb65-e1ad662ed95f) | 查找数组的首行，并返回指定单元格的值                 |
| [COLUMN 函数](https://support.microsoft.com/zh-cn/office/column-函数-44e8c754-711c-4df3-9da4-47a55042554b) | 返回引用的列号                                       |
| [ROWS 函数](https://support.microsoft.com/zh-cn/office/rows-函数-b592593e-3fc2-47f2-bec1-bda493811597) | 返回引用中的行数                                     |
| [ADDRESS 函数](https://support.microsoft.com/zh-cn/office/address-函数-d0c26c0d-3991-446b-8de4-ab46431d4f89) | 以文本形式将引用值返回到工作表的单个单元格           |
| [INDIRECT 函数](https://support.microsoft.com/zh-cn/office/indirect-函数-474b3a3a-8a26-4f44-b491-92b6306fa261) | 返回由文本值指定的引用                               |
| [INDEX 函数](https://support.microsoft.com/zh-cn/office/index-函数-a5dcf0dd-996d-40a4-a822-b56b061328bd) | 使用索引从引用或数组中选择值                         |

