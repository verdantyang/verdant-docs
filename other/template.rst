.. _template:

RST模板
========

二级标题
--------

.. note:: 注解
  - 标题级别和下划线无对应，文档中保持一致就好。
  - reST标题可用下列符号标记： # * = - ^ ~ ` : . _ + ” 等。

三级标题
~~~~~~~~

四级标题
^^^^^^^^

五级标题
++++++++

六级标题
````````

字体
--------

两个连续反引号嵌入代码，如: ``git status`` 。

`Got GitHub` by Jiang Xin.

这是 **粗体** ，这是 *斜体* 。

不留白的\ **粗体**\ 和\ *斜体*\ 效果

.. role:: strike
   :class: strike

:strike:`删除线` 效果

不留白的\ :strike:`删除线`\ 效果

.. role:: ul
   :class: underline

:ul:`下划线` 效果

不留白的\ :ul:`下划线`\ 效果

- Water: H\ :sub:`2`\ O
- E = mc\ :sup:`2`

标记符号前后空白\
用\ **反斜线**\ 消除

段落
--------

第一段内容。

第二段和第一段间有一空行。

一个回车不分段，
本行续上行。

| 保持换行符，
| 本行不续行。

.. role:: raw-html(raw)
   :format: html

用新定义的role插入换行，
:raw-html:`<br />`
本行不再续行。

段落缩进
~~~~~~~~

邮件体段落缩进：

> 第一级段落缩进。
>
> > 第二级段落缩进。
>
> 返回一级段落缩进。

代码块
~~~~~~~~

双冒号后缩进为代码块。

::

  $ printf "Hello, world.\n"

还可声明语言类型实现语法加亮。

.. code-block:: sh

   $ printf "Hello, world.\n"

注释
~~~~~~~~

git
  Simple and beautiful.

hg
  Another DVCS.

subversion
  VCS with many constrains.

  Why not Git?

分割线
~~~~~~~~

四条短线或以上显示为分隔线。

----

列表
--------

无序列表
~~~~~~~~

* 星号、减号、加号开始列表。

  - 列表层级和缩进有关。

    + 和具体符号无关。

* 返回一级列表。

有序列表
~~~~~~~~

1. 数字和点是一种编号方式。

   A. 大写字母编号。

      a. 小写字母编号。

2. 继续一级列表。

   (I) 大写罗马编号。

       i) 小写罗马编号。

列表续行、段落和代码块
~~~~~~~~~~~~~~~~~~~~~~

1. 列表项可以折行，
   对齐则自动续行。

2. 列表项可包含多个段落。

   空行开始的新段落，
   新段落要和列表项内容对齐。

3. 列表下的代码段注意对齐即可。

   ::

     $ printf "Hello, world.\n"


链接
--------

超链接
~~~~~~~~

- 网址 http://github.com/
- 邮件 me@foo.bar

- 访问 `Google <http://google.com/>`_ 。
- 上面已定义，直接引用 google_ 链接。
- 链接地址在后面定义，如： GitHub_ 。
- 反引号括起多个单词的链接。如 `my blog`_ 。

.. _GitHub: http://github.com
.. _my blog: http://www.worldhello.net

内部跳转
~~~~~~~~

.. _fig1:

.. figure:: /images/test_github.png

   内部跳转图例

上面定义的位置，可以：

- 通过 fig1_ 跳转。
- 或者 `点击这里 <#fig1>`__ 跳转。
- 或者参见 :ref:`fig1`\ 。


表格
--------

.. table:: 示例表格
   :class: classic

   +---------+--------+--------+
   | head1   | head2  | head3  |
   +=========+========+========+
   |         | cell   | cell   |
   | rowspan +--------+--------+
   |         | * colspan       |
   |         | * another line  |
   +---------+-----------------+

图片
--------

.. figure:: /images/test_github.png
   :width: 32

   图：GitHub Octocat

- GitHub Logo: |octocat|
- 带链接的图片：
  |imglink|_
- 下图向右浮动。
   .. image:: /images/test_github.png
      :align: right

.. |octocat| image:: /images/test_github.png
.. |imglink| image:: /images/test_github.png
.. _imglink: https://github.com/


其他
--------

转义
~~~~~~~~

反斜线作为转义字符，\
禁止对后面 \*字符* 做语法解析。

脚注
~~~~~~~~

reST脚注的多种表示法：

- 脚注即可以手动分配数字 [1]_ ，
  也可以使用井号自动分配 [#]_ 。

- 自动分配脚注 [#label]_ 也可以用
  添加标签形式 [#label]_ 多次引用。

- 还支持用星号嵌入符号式脚注，
  如这个 [*]_ 和 这个 [*]_ 。

- 使用单词做标识亦可 [CIT2012]_ 。


.. [1] 数字编号脚注。
.. [#] 井号自动编号。
.. [#label] 井号添加标签以便多次引用。
.. [*] 星号自动用符号做脚注标记。
.. [*] 星号自动用符号做脚注标记。
.. [CIT2012] 单词或其他规定格式。


