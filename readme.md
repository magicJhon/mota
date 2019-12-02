# 魔塔

    这是一个用H5重置的经典50层魔塔。
    该游戏适用于移动端，打包后可自选任意方式直接制作成手机app进行游戏。
    

## 关于游戏资源：
游戏中物品、怪物等数据来源：[百度百科：魔塔50层](https://baike.baidu.com/item/50%E5%B1%82%E9%AD%94%E5%A1%94/4446423?fr=aladdin)  
游戏素材来源：[百度贴吧：魔塔吧](https://tieba.baidu.com/f?kw=%C4%A7%CB%FE&fr=ala0&tpl=5)  

## 关于游戏编辑器：
为了方便制作地图，我使用Vue.js + Iview写了一个很简易的地图编辑器。
编辑器中包含了所有游戏元素。  
游戏元素主要分为：建筑、物品、NPC、事件、怪物。  
游戏元素，均可通过选择对应图标直接添加在地图中。  
添加怪物、NPC、事件需要选择或输入对应附加内容。  

#### 怪物元素在添加前可选择事件及开门选项  
- 事件选项：开启后，需要输入对应事件名称  
- 开门选项：开启后，需要选择门的类型，及门的坐标集。多个坐标之间用空格分隔  

#### NPC及事件在添加时需要输入对应事件名称  

#### 其他编辑内容：
当前楼层、从楼下上来后角色的位置、从楼上下来后角色的位置。

地图编辑完成后，只需要点击生成地图，会自动将地图信息复制到粘贴板。  
讲生成的地图信息直接粘贴在Maps文件中即可。改文件会导出所有已添加的地图。  

## 更新
- 2019/11/15：第一次上传。已完成了游戏大部分逻辑及地图编辑器功能。并制作了1、2层地图用于测试。
- 2019/11/19：增加广度优先搜索（BFS）算法，用于后期自动寻路 
- 2019/11/26：增加A*算法，提高寻路算法效率。（但实际测试小地图中，性能提升非常有限，甚至由于算法中循环更多，性能会下降。）
- 2019/11/27：增加怪物、NPC等自动寻路功能及缓动动画。对应剧情中可展现NPC移动过程。
- 2019/11/28：
  - 测试自动寻路
  - 修复自动寻路中玩家仍可移动的BUG
  - 修复游戏事件完成后，角色自动移动的BUG
- 2019/12/02：制作动画库。
  - 根据图片自动计算播放路径
  - 动画播放完成回调
  - 可设置播放速度
  - 播放及暂停功能 


## 免责声明
制作这个游戏基于两个出发点：  
1、这是我第一次开发游戏，完全出于学习的目的。  
2、这是我学生时代在电子词典上玩过的游戏，我很怀念那个时光，所以选择了它。  

游戏非原创，游戏中的资源也来自网络。也就是说除了代码，都不是我的。  
如果有人看到了这个游戏，并认为我在某些方面涉及侵权，请与我联系。





