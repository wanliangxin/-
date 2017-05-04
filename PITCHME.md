#  progress bar（进度条）
适用进度条，用户可以跟进相关的任务执行进度，带有百分比的0进度条表示一个确定的进度，没有带百分比的进度条表示不确定的进度
用户研究表明，用户意识到响应的时长超过一秒，所以当操作获得反馈的时间超过两秒时，应该考虑某种进度的反馈


![图片标题](https://i-msdn.sec.s-msft.com/dynimg/IC725875.png)

## 使用进度条的场景

 - 操作是否在约五秒钟内完成？如果是这样，使用活动指标，因为在这么短的时间内显示进度条将会分散注意力。如果操作通常需要五秒钟或更短时间，但有时需要更多，请从繁忙的指针开始，并在五秒钟后转换为进度条。
 - 用于等待用户完成任务的不确定进度条？如果是这样，不要使用进度条。
 - 进度栏用于计算机进度，而不是用户进度。
 - 一个不确定的进度条与动画结合在一起吗？如果是，请改用动画。不确定的进度条实际上是一个通用的动画，并且不为动画添加任何值。
 - 操作是否非常漫长（超过两分钟）后台任务，用户对完成比对进度更感兴趣？如果是，请改用通知。在这种情况下，用户在此期间执行其他任务，并不监视进度。使用通知允许用户执行其他任务而不中断。这种冗长操作的示例包括打印，备份，系统扫描和批量数据传输或转换。
 - 操作完成后，用户能否重播结果？如果是，请改用滑块。这种操作的示例包括视频和音频记录和回放。
 
## 设计理念
在一个长操作中，用户需要明确的问题有以下几个方面：
 - 长操作已经开始
 - 长操作正在取得进展，并且将最终完成（没有被锁死）
 - 已经完成的操作的大致百分比
 - 如果不值得等待，用户可以取消该操作
 - 在等待完成的同时，是否应该继续等待，或者做点别的


对于需要有限时间量的操作，即使无法准确预测该时间量，请使用确定的进度条。不确定的进度条显示正在取得进展，但不提供其他信息。不要仅仅根据可能的精度不足来选择一个不确定的进度条。


总之一句话：确保您为长时间的操作提供进度反馈，并且上述信息被明确传达。尽可能使用确定的进度条。

## 使用模式

### Determinate progress bars

 - Modal determinate progress bars
 
   因为这种反馈是模态的，所以用户无法在窗口中执行其他任务（或者如果在模态对话框中显示，则为其父任务），直到操作完成。
 
![图片标题](https://i-msdn.sec.s-msft.com/dynimg/IC725877.png)

 - Modal determinate progress bars with a Cancel or Stop button
 
   Allow users to halt the operation, perhaps because the operation is taking too long or isn't worth the wait.

![图片标题](https://i-msdn.sec.s-msft.com/dynimg/IC725878.png)

 - Modal determinate progress bars with a Cancel or Stop button and animation
 
   Allow users to halt the operation, and include an animation to help users visualize the effect of an operation.

![图片标题](https://i-msdn.sec.s-msft.com/dynimg/IC725879.png)
  

 - Modal determinate double progress bars

![图片标题](https://i-msdn.sec.s-msft.com/dynimg/IC725880.png)

  In this example, the first progress bar shows the progress of the current step and the second progress bar shows the overall progress.

 - Modeless determinate progress bars
 
  Unlike with modal progress bars, users can perform other tasks while the operation is in progress. These progress bars can be displayed in context or on a status bar.

![图片标题](https://i-msdn.sec.s-msft.com/dynimg/IC725881.png)

  In this example, Windows Internet ExplorerWindows Internet Explorer displays its progress for loading a Web page on the status bar. Users can perform other tasks while the page is loading.

### Indeterminate progress bars

 - Modal indeterminate progress bars

  Used only for operations whose overall progress cannot be determined, so there is no notion of completeness. Determinate progress bars are preferable because they indicate the approximate percentage of the operation that has been completed, and help users determine if the operation is worth continuing to wait. They are also less visually distracting.

![](https://i-msdn.sec.s-msft.com/dynimg/IC725882.png)

 - Modeless indeterminate progress bars
 
  Unlike modal progress bars, users can perform other tasks while the processing is in progress. These progress bars can be displayed in context or on a status bar.
 
![图片标题](https://i-msdn.sec.s-msft.com/dynimg/IC725883.png)

## meters

表示一个百分比，而不是一个相对进度

This pattern isn't a progress bar, but it is implemented using the progress bar control. Meters have a distinct look to differentiate them from true progress bars.

![](https://i-msdn.sec.s-msft.com/dynimg/IC725884.png)















