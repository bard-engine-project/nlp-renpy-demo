# NLP, Interpreter and Game Engine

### Interpreter and Parser

选型：ANTLR4 / PLY

### NLP

（第二阶段再考虑）

### Game and Game Engine
之前的架构设计：
![Design](res/Design.png)

- Input/Medium Connector部分，简单而言就是设计meta primitive，使得input device和input flow通过mapping方式松耦合（类似于手柄映射设置），使得output flow根据output device的capability自由拆分并实现同步
- RenPy已经实现了上图的五层结构中四部分（除了connector这一概念），是一个完整的游戏引擎了；这个项目要实现的，是在最下面一层追加**翻译层**：从**自然语言**翻译到**RenPy脚本语言**

> 以下部分为第三阶段内容
- 根据体验到的游戏，以下内容的自动生成是可行的：
    - 对话框：
    - 人物动作描述：
    - p
- 根据体验到的而言，以下内容的自动生成是不可行的：
    > “Rewrite”，“Finding Paradise”，“仙剑奇侠传六”，“Nier：Automata”，etc.
    - 互动形式：
    - 场景资源自动堆叠：


### TODO
- [ ] Integrated with Waifu Generator