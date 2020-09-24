# NLP, Interpreter and Game Engine


之前的架构设计：
![Design](res/Design.png)

- Input/Medium Connector部分，简单而言就是设计meta primitive，使得input device和input flow通过mapping方式松耦合（类似于手柄映射设置），使得output flow根据output device的capability自由拆分并实现同步
- RenPy已经实现了上图的五层结构中四部分（除了connector这一概念），是一个完整的游戏引擎了；这个项目要实现的，是在最下面一层追加**翻译层**：从**自然语言**翻译到**RenPy脚本语言**