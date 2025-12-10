### @explicitHints 1

# Lesson 1: Code a Road Network

## Step 1
Rename the **run** element of the ``||Player:on chat command||`` block to **road_1**. Select the ``||Blocks:fill with||`` code block and drag it into your ``||Player:on chat command||`` block.

### ~ tutorialhint
``` blocks
player.onChat("road_1", function () {
    blocks.fill(
    GRASS,

    pos(0, 0, 0),
    pos(0, 0, 0),
    FillOperation.Replace
    )
})
```

## Step 2
Use the drop-down menu to change the type of block from **Grass** to **Gray Concrete**.
### ~ tutorialhint

``` blocks
player.onChat("road_1", function () {
    blocks.fill(
    GRAY_CONCRETE,
    pos(0, 0, 0),
    pos(0, 0, 0),
    FillOperation.Replace
    )
})
```

## Step 3
Now open ``||Positions:POSITIONS||`` toolbox drawer and drag the world ``||Positions:[0] [0] [0]||`` code block onto your coding Workspace.
Drag the world ``||Positions:[0] [0] [0]||`` block and replace the ``||Positions:relative||`` positions block inside the ``||Blocks:fill||`` block.

### ~ tutorialhint
``` blocks
player.onChat("road_1", function () {
    blocks.fill(
    GRAY_CONCRETE,
    world(0, 0, 0),
    pos(0, 0, 0),
    FillOperation.Replace
    )
})
```

## Step 4
Drag another ``||Positions:world [0] [0] [0]||`` positions code block from the ``||Positions:POSITIONS||`` drawer and replace the second ``||Positions:relative||`` positions block inside the ``||Blocks:fill with||`` block.

### ~ tutorialhint
``` blocks
player.onChat("road_1", function () {
    blocks.fill(
    GRAY_CONCRETE,
    world(0, 0, 0),
    world(0, 0, 0),
    FillOperation.Replace
    )
})
```

## Step 5
We are almost ready to test our code, however there is one more important thing we have to do to make this code work properly. Change the center, or **Y** coordinate, to one number lower. In this example, this will be **68**. Now test your code. If you have coded correctly, you should see a road appear in place of the Grass.

### ~ tutorialhint
``` blocks
player.onChat("road_1", function () {
    blocks.fill(
    GRAY_CONCRETE,
    world(-21, 68, -565),
    world(61, 68, -569),
    FillOperation.Replace
    )
})

```

## Step 6
Repeat the steps for the second road.

### ~ tutorialhint
``` blocks
player.onChat("road_2", function () {
    blocks.fill(
    GRAY_CONCRETE,
    world(-21, 68, -532),
    world(61, 68, -536),
    FillOperation.Replace
    )
})
```

## Step 7
(Extension) With two roads done, build more using the code you have just created. When you are finished, go to the Unit 2 Lesson 1 NPC and ask for some carpet to make road markings with using your agent to place them.
``` blocks
agent.place()
```


> 在 [https://junming0106.github.io/test-01/](https://junming0106.github.io/test-01/) 打開此頁面

## 作為擴充功能使用

可以在 MakeCode 中將此儲存庫新增為**擴充功能**。

* 開啟 [https://minecraft.makecode.com/](https://minecraft.makecode.com/)
* 按一下**新專案**
* 按一下工具齒輪選單下的**擴充功能**
* 搜索 **https://github.com/junming0106/test-01** 並匯出

## 編輯此專案

編輯 MakeCode 中的儲存庫。

* 開啟 [https://minecraft.makecode.com/](https://minecraft.makecode.com/)
* 按一下**匯入**，然後按一下**匯入 URL**
* 貼上 **https://github.com/junming0106/test-01** 並按一下匯入

#### 中繼資料 (用於搜索、渲染)

* for PXT/minecraft
<script src="https://makecode.com/gh-pages-embed.js"></script><script>makeCodeRender("{{ site.makecode.home_url }}", "{{ site.github.owner_name }}/{{ site.github.repository_name }}");</script>
