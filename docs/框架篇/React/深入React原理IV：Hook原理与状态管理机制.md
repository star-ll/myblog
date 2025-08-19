- **Hooks架构**
    
    - 链表结构：`fiber.memoizedState`串联Hooks
        
    - 全局调度器：`ReactCurrentDispatcher`切换
        
- **核心Hook原理**
    
    - `useState`：状态更新批处理与`lane`绑定
        
    - `useEffect`：异步调度与依赖比对（`areHookInputsEqual`）
        
    - `useRef`：跨生命周期引用实现
        
- **自定义Hook**
    
    - 逻辑复用：闭包陷阱与依赖处理规范
        
- **源码解密**：`ReactFiberHooks.js`调度逻辑