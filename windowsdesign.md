# 产品的力量和简约
> 一个伟大的应用应该是简单并且具有力量的，具体包含以下几点：
* 可用性. 产品用来满足目标用户的需求, 使他们能够执行他们无法做到的任务，有效的实现目标；
* 有效性. 从规模和效率两个层面提高用户的生产效率；
* 多兼容，多层面. 能够使用户在多种情况下，多种环境中有效的执行任务；
* 直接性. 直接帮助用户实现目标，不绕不偏. 快捷键、键盘访问，诸如此类；
* 灵活性. 允许用户在使用过程中完整、细粒度的控制；
* 集成并整体统一. 产品能够无缝衔接于所承载应用的介质，产品与介质融为一体；
* 先进性.产品拥有非凡的、积极地、先进的竞争对手没有的特性.
> An application is powerful when it has the right combination of these characteristics:
* Enabling. The application satisfies the needs of its target users, enabling them to perform tasks that they couldn't otherwise do and achieve their goals effectively.
* Efficient. The application enables users to perform tasks with a level of productivity and scale that wasn't possible before.
* Versatile. The application enables users to perform a wide range of tasks effectively in a variety of circumstances.
* Direct. The application feels like it is directly helping users achieve their goals, instead of getting in the way or requiring unnecessary steps. Features like shortcuts, keyboard access, and macros improve the sense of directness.
* Flexible. The application allows users complete, fine-grained control over their work.
* Integrated. The application is well integrated with Microsoft Windows, allowing it to share data with other applications.
* Advanced. The application has extraordinary, innovative, state-of-the-art features that are not found in competing solutions
# 设计技巧
> To obtain simplicity while maintaining power, choose the right set of features, locate the features in the right places, and reduce the effort to use them. This section gives some common techniques to achieve these goals.
## 选择恰当的功能设置
> "Perfection is achieved, not when there is nothing more to add,
> but when there is nothing left to take away." —Antoine de Saint-Exupery
* Determine the features your users need. Understand your users' needs through goal, scenario, and task analysis. Determine a set of features that realizes these objectives.
* Remove unnecessary elements. Remove elements that aren't likely to be used or have preferable alternatives.
* ==Remove unnecessary redundancy.== There might be several effective ways to perform a task. To achieve simplicity, make the hard decision and choose the best one for your target users instead of providing all of them and making the choice an option.
*　Make it "just work" automatically. The element is necessary, but any user interaction to get it to work is not because there is an acceptable default behavior or configuration. To achieve simplicity, make it work automatically and either hide it from the user completely or reduce its exposure significantly.
## 通过以下的手段去呈现力量，保持简单
>"The ability to simplify means to eliminate the unnecessary
> so that the necessary may speak." —Hans Hofmann

### 实现产品相对于用户简单使用，可以通过以下手段：
* 集合应该集合的信息； 将支撑同一个任务的功能结合在一起，使用户能够流畅线性的操作，拆解复杂的逻辑，将复杂的逻辑拆成一个个的小流程和小逻辑，一个地方可能会有多种页面呈现形式，例如：引导性内容 
* 拆分应该拆分的信息；不是所有的东西都要展示在同一个区域，区域与区域之间应该有清晰，明显的边界，区域中应该凸显出对应的核心功能，适当的隐藏和折叠无关重要的功能，互相存在关联的信息在两个信息之间留有胡同的入口
* 去除能被去除的信息；信息中突出呈现核心信息，若一块信息移除之后不会对整体产生影响，那就移除该模块，可做可不做，选择不做；
* 一致性、可配置性、通用性有时候会带来不必要的麻烦
* 将元素放在最合适的位置；无关主流程的介绍信息等，与当前操作无关的详细信息，可以用一个新的窗口或者新的页面去呈现；一个元素的呈现要考虑其对应的模块、上下文关系，界面元素布局等。
* 使用有意义的高级组合；页面中呈现的东西考虑更加适合的方案，高对比度黑色配色背后的意图比黑色的背景更加明显。 
* 选择合适的控件。
### Use the following design techniques to preserve power, while achieving simplicity through the perception of reduction or removal:
* Combine what should be combined. Put the essential features that support a task together so that a task can be performed in one place. The task's steps should have a unified, streamlined flow. Break down complex tasks into a set of easy, clear steps, so that "one" place might consist of several UI surfaces, such as a wizard.
* Separate what should be separated. Not everything can be presented in one place, so always have clear, well-chosen boundaries. Make features that support core scenarios central and obvious, and hide optional functionality or make it peripheral. Separate individual tasks and provide links to related tasks. For example, tasks related to manipulating photos should be clearly separated from tasks related to managing collections of photos, but they should be readily accessible from each other.
* Eliminate what can be eliminated. Take a printout of your design and highlight the elements used to perform the most important tasks. Even highlight the individual words in the UI text that communicate useful information. Now review what isn't highlighted and consider removing it from the design. If you remove the item, would anything bad happen? If not, remove it!
* Consistency, configurability, and generalization are often desirable qualities, but they can lead to unnecessary complexity. Review your design for misguided efforts in consistency (such as having redundant text), generalization (such as having any number of time zones when two is sufficient), and configurability (such as options that users aren't likely to change), and eliminate what can be eliminated.
* Put the elements in the right place. Within a window, an element's location should follow its utility. Essential controls, instructions, and explanations should all be in context in logical order. If more options are needed, expose them in context by clicking a chevron or similar mechanism; if more information is needed, display an infotip on mouse hover. Place less important tasks, options, and Help information outside the main flow in a separate window or page. The technique of displaying additional detail as needed is called progressive disclosure.
* Use meaningful high-level combinations. It is often simpler and more scalable to select and manipulate groups of related elements than individual elements. Examples of high-level combinations include folders, themes, styles, and user groups. Such combinations often map to a user goal or intention that isn't apparent from the individual elements. For example, the intention behind the High Contrast Black color scheme is far more apparent than that of a black window background.
* Select the right controls. Design elements are embodied by the controls you use to represent them, so selecting the right control is crucial to efficient presentation. For example, the font selection box used by Microsoft Word shows both a preview of the font as well as the most recently used fonts. Similarly, the way Word shows potential spelling and grammar errors in place is much simpler than the dialog box alternative, as shown in the beginning of this article.

### 减少用户的努力
> "Simple things should be simple.
> Complex things should be possible."—Alan Kay
* Make tasks discoverable and visible. All tasks, but especially frequent tasks, should be readily discoverable within the user interface. The steps required to perform tasks should be visible and should not rely on memorization.
* Present tasks in the user's domain. Complex software requires users to map their problems to the technology. Simple software does that mapping for them by presenting what is natural. For example, a red-eye reduction feature maps directly to the problem space and doesn't require users to think in terms of details like hues and gradients.
* Put domain knowledge into the program. Users shouldn't be required to access external information to use your application successfully. Domain knowledge can range from complex data and algorithms to simply making it clear what type of input is valid.
* Use text that users understand. Well-crafted text is crucial to effective communication with users. Use concepts and terms familiar to your users. Fully explain what is being asked in plain language so that users can make intelligent, informed decisions.
* Use safe, secure, probable defaults. If a setting has a value that applies to most users in most circumstances, and that setting is both safe and secure, use it as the default value. Make users specify values only when necessary.
* Use constraints. If there are many ways to perform a task, but only some are correct, constrain the task to those correct ways. Users should not be allowed to make readily preventable mistakes.

# Powerful and simple

Power is all about enabling your users and making them productive. Simplicity is all about removing the unessential and presenting features the right way. By understanding your target users and achieving the right balance of features and presentation, you can design Windows-based applications that do both.
# 箴言

* 简约而不简陋。"Everything should be made as simple as possible,but not simpler."—Albert Einstein
* 用户呈现的越简约，意味着我们付出的努力越多。"I have only made this letter longer because I have not the time to make it shorter."—Blaise Pascal
