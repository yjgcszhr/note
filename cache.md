### 硬件预取（Hardware Prefetching）
是一种在计算机系统中用于提高缓存性能的技术。它通过预先将可能被访问的数据块加载到缓存中，以减少缓存未命中的情况，从而提高数据访问的效率。硬件预取通常由处理器或缓存控制器等硬件组件实现，并且在现代计算机系统中得到广泛应用。

硬件预取通常有两种类型：

1. **流式硬件预取（Stream Prefetching）**：
   - 流式硬件预取是指根据已知的数据访问模式，在预定的流程中预先加载数据块到缓存中。例如，当处理器访问一个数组中的连续元素时，硬件可以预先加载下一个数据块到缓存中，以提高连续访问的效率。

2. **跳跃硬件预取（Stride Prefetching）**：
   - 跳跃硬件预取是指根据已知的数据访问间隔，预先加载可能被访问的数据块到缓存中。例如，当处理器以固定的步长访问一个数组时，硬件可以预先加载固定步长之后的数据块到缓存中，以减少跳跃访问引起的缓存未命中。

硬件预取的实现通常依赖于硬件的预取引擎或预取缓冲器，它们可以监视和分析数据访问模式，并根据预先定义的预取策略来预取数据块到缓存中。预取策略可能包括预取深度、预取宽度、预取距离等参数，用于控制预取的行为。

总的来说，硬件预取是一种在计算机系统中提高缓存性能的重要技术，通过预先加载可能被访问的数据块到缓存中，减少缓存未命中，从而提高数据访问的效率。