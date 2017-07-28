# IMP

类的方法列表会把选择子的名称映射到相关的方法实现上，是的“动态消息派发系统”能够根据此找到应该调用的方法。这些方法均以函数指针的形式来表示，这种指针叫做IMP

        id(*IMP)(id, SEL...)

# method swizzling

- 交换方法的实现

        void method_exchangeImplementations(Method m1, Method m2)

- 获取方法的实现

       Method class_getInstanceMethod(Class cls, SEL name)