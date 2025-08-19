- 虚拟DOM本质：轻量JS对象描述UI
    
- Fiber节点结构：`tag`/`stateNode`/`child`/`lanes`
    
- 双缓存机制：current树与workInProgress树
    
- 源码定位：`ReactFiber.js`关键字段解析


- **Fiber节点设计**
    
    - 链表结构：`child`/`sibling`/`return`遍历路径
        
    - 双缓存树：`current`与`workInProgress`切换策略
        
- **协调算法**
    
    - Diff优化：单节点/多节点比对策略（`reconcileChildFibers`）
        
    - 副作用收集：`subtreeFlags`冒泡标记
        
- **提交阶段**
    
    - 三阶段划分：BeforeMutation→Mutation→Layout
        
    - DOM原子操作：`commitPlacement`节点插入
        
- **源码精读**：`ReactFiberWorkLoop.js`构建流程
