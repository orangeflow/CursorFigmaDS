# WeChat Pay HK Design System
## 微信支付香港设计系统 CSS 规范

这是一个基于 Figma 设计系统生成的 CSS 设计系统规范文件，包含了完整的组件样式、设计令牌和工具类。

## 📁 文件结构

```
CursorFigmaDS/
├── design-system.css              # 设计系统 CSS 主文件
├── design-system-examples.html     # 组件使用示例
├── components-documentation.html    # 组件文档（带左侧导航树）
└── README.md                      # 本文档
```

## 🚀 快速开始

### 1. 引入 CSS 文件

在 HTML 文件中引入设计系统 CSS：

```html
<link rel="stylesheet" href="design-system.css">
```

### 2. 使用组件

- 查看组件文档：打开 `components-documentation.html` 查看完整的组件文档（带左侧导航树）
- 查看使用示例：打开 `design-system-examples.html` 查看组件的实际效果

## 🎨 设计令牌 (Design Tokens)

### 颜色系统

#### 品牌色
- `--color-brand-primary`: `#07c160` - 主要品牌色（绿色）
- `--color-brand-primary-disabled`: `rgba(7, 193, 96, 0.5)` - 禁用状态

#### 危险色
- `--color-danger`: `#fa5151` - 危险操作颜色（红色）
- `--color-danger-disabled`: `rgba(250, 81, 81, 0.5)` - 禁用状态

#### 中性色
- `--color-white`: `#ffffff`
- `--color-black`: `#000000`
- `--color-black-05`: `rgba(0, 0, 0, 0.05)`
- `--color-black-10`: `rgba(0, 0, 0, 0.1)`
- `--color-black-50`: `rgba(0, 0, 0, 0.5)`

### 字体系统

#### 字体族
- `--font-family-chinese`: `'PingFang_HK', 'PingFang_SC', ...`

#### 字体大小
- `--font-size-text-01`: `44px`
- `--font-size-text-02`: `34px`
- `--font-size-text-03`: `32px`
- `--font-size-text-04`: `28px`
- `--font-size-text-05`: `24px`
- `--font-size-text-06`: `22px`
- `--font-size-text-07`: `20px`

#### 行高
- `--line-height-text-01`: `64px`
- `--line-height-text-02`: `48px`
- `--line-height-text-03`: `48px`
- `--line-height-text-04`: `40px`
- `--line-height-text-05`: `32px`
- `--line-height-text-06`: `32px`
- `--line-height-text-07`: `28px`

#### 字重
- `--font-weight-regular`: `400`
- `--font-weight-medium`: `500`
- `--font-weight-semibold`: `600`

### 间距系统

- `--space-010`: `4px` - 组件场景使用，例如选项卡、标签等小型元素之间的间隔
- `--space-020`: `8px` - 组件场景使用，例如按钮、徽标、单元格、页脚、小标题之间的间隔
- `--space-030`: `16px` - 组件场景使用，例如选项卡、表单、协议、多选框、单选框
- `--space-040`: `24px` - 组件场景使用，例如步骤器、侧边栏
- `--space-050`: `32px` - 组件场景使用，例如步骤器、输入框
- `--space-060`: `40px` - 组件场景使用，例如半屏弹层顶部
- `--space-070`: `48px` - 组件场景使用，例如结果页
- `--space-080`: `64px` - 组件场景使用，例如对话框、半屏弹层
- `--space-090`: `80px` - 组件场景使用，例如半屏弹层、结果页操作区
- `--space-100`: `96px` - 组件场景使用，例如结果页
- `--space-110`: `120px` - 半屏弹层顶部与导航栏底部需保持120px及以上间距

### 圆角系统

- `--radius-010`: `4px` - 极小场景使用，例如标签
- `--radius-020`: `8px` - 组件场景使用，例如按钮
- `--radius-030`: `12px` - 组件场景使用
- `--radius-040`: `16px` - 组件场景使用，例如向导提示、公告栏
- `--radius-050`: `24px` - 组件场景使用，例如半屏弹层、轻提示
- `--radius-060`: `32px` - 组件场景使用
- `--radius-full`: `9999px` - 胶囊型组件使用，例如选项卡、胶囊徽标、开关、分页导航器

### 动效系统 (Motion System)

#### 动效时间

**移动设备时间：**
- `--motion-duration-mobile-small`: `100ms`
- `--motion-duration-mobile-base`: `200ms`
- `--motion-duration-mobile-medium`: `250ms`
- `--motion-duration-mobile-large`: `300ms`
- `--motion-duration-mobile-xlarge`: `500ms`

**平板设备时间（比移动设备长30%）：**
- `--motion-duration-tablet-small`: `130ms`
- `--motion-duration-tablet-base`: `260ms`
- `--motion-duration-tablet-medium`: `325ms`
- `--motion-duration-tablet-large`: `390ms`
- `--motion-duration-tablet-xlarge`: `650ms`

**UI组件尺寸时间：**
- `--motion-duration-small-ui`: `100ms` - 小尺寸UI组件（开关、勾选）
- `--motion-duration-small-ui-close`: `200ms`
- `--motion-duration-medium-ui-open`: `250ms` - 中尺寸UI组件（菜单弹层）展开
- `--motion-duration-medium-ui-close`: `200ms` - 中尺寸UI组件收起
- `--motion-duration-large-ui-open`: `300ms` - 大尺寸UI组件（全局弹层）展开
- `--motion-duration-large-ui-close`: `250ms` - 大尺寸UI组件收起

#### 缓动曲线

- `--easing-linear`: `linear` - 线性动效（无缓动）
- `--easing-ease-out`: `cubic-bezier(0.33, 1, 0.68, 1)` - 缓出（快速响应，自然结束）
- `--easing-ease-in`: `cubic-bezier(0.11, 0, 0.5, 0)` - 缓入（慢速开始，加速离开）
- `--easing-ease-in-out`: `cubic-bezier(0.65, 0, 0.35, 1)` - 缓入缓出（持续在视线内的元素）

## 🧩 组件

### 按钮 (Button)

#### 基础用法

```html
<!-- Primary 按钮 -->
<button class="btn btn--primary btn--large">完成</button>

<!-- Auxillary 按钮 -->
<button class="btn btn--auxillary btn--middle">取消</button>
```

#### 尺寸

- `btn--large`: 大尺寸 (80px 高)
- `btn--middle`: 中等尺寸 (64px 高)
- `btn--small`: 小尺寸 (56px 高)

#### 类型

- `btn--primary`: 主要按钮（绿色背景，白色文字）
- `btn--auxillary`: 辅助按钮（浅灰背景，品牌色文字）

#### 主题

- `btn--danger`: 危险主题（红色背景，白色文字）

#### 状态

- `btn--disabled` 或 `disabled` 属性：禁用状态

#### 带图标的按钮

```html
<button class="btn btn--primary btn--middle">
  <span class="btn__icon btn__icon--prefix">
    <!-- 图标内容 -->
  </span>
  <span class="btn__text">完成</span>
</button>
```

#### 按钮组

```html
<div class="btn-group">
  <button class="btn btn--auxillary btn--middle">取消</button>
  <button class="btn btn--primary btn--middle">确认</button>
</div>
```

### 运营按钮 (Operational Button)

```html
<!-- 大尺寸 -->
<button class="operational-btn operational-btn--large">
  <span class="operational-btn__text">按钮文案</span>
</button>

<!-- 中等尺寸 -->
<button class="operational-btn operational-btn--medium">
  <span class="operational-btn__text">按钮文案</button>
</button>

<!-- 小尺寸（仅图标） -->
<button class="operational-btn operational-btn--small">
  <span class="operational-btn__icon">→</span>
</button>
```

### Banner 组件

```html
<div class="banner">
  <div class="banner__content">
    <h3 class="banner__title">主文案</h3>
    <p class="banner__subtitle">副文案副文案副文案</p>
  </div>
  <div class="banner__action">
    <button class="operational-btn operational-btn--medium">
      <span class="operational-btn__text">按钮文案</span>
    </button>
  </div>
</div>
```

### Picker 选择器组件

用于选择一个时间点或者一个时间段。

#### 基础用法

```html
<!-- 单列选择器 -->
<div class="picker picker--single-column">
  <div class="picker__header">
    <button class="picker__close">
      <svg class="picker__close-icon">...</svg>
    </button>
    <p class="picker__title">单列选择器</p>
    <div class="picker__placeholder"></div>
  </div>
  <div class="picker__content">
    <div class="picker__columns picker__columns--single">
      <div class="picker__column">
        <div class="picker__option">
          <span class="picker__option-text">选项一</span>
        </div>
        <div class="picker__option picker__option--selected">
          <span class="picker__option-text">选项二</span>
        </div>
      </div>
    </div>
    <div class="picker__mask-top"></div>
    <div class="picker__mask-bottom"></div>
  </div>
  <div class="picker__footer">
    <button class="picker__confirm-btn">
      <span class="picker__confirm-btn-text">确定</span>
    </button>
  </div>
</div>
```

#### 类型

- `picker--single-column`: 单列选择器
- `picker--double-column`: 双列选择器
- `picker--triple-column`: 三列选择器

#### 状态

- `picker__option--selected`: 选中状态

### Step 步骤器组件

用于任务步骤展示或任务进度展示。支持水平（Horizontal）和垂直（Vertical）两种布局方式。

#### 基础用法

```html
<!-- 水平步骤器 -->
<div class="step step--horizontal step--process">
  <div class="step__item step__item--completed">
    <div class="step__icon">
      <div class="step__icon-number step__icon-number--green">
        <span class="step__icon-number-text">1</span>
      </div>
    </div>
    <div class="step__line step__line--brand"></div>
  </div>
  <div class="step__item step__item--in-progress">
    <div class="step__icon">
      <div class="step__icon-number step__icon-number--green">
        <span class="step__icon-number-text">2</span>
      </div>
    </div>
    <div class="step__line"></div>
  </div>
</div>

<!-- 垂直步骤器 -->
<div class="step step--vertical step--process">
  <div class="step__item step__item--completed">
    <div class="step__icon">
      <div class="step__icon-done">
        <svg>...</svg>
      </div>
      <div class="step__line step__line--brand"></div>
    </div>
    <div class="step__content">
      <div class="step__header">
        <p class="step__title">标题</p>
        <p class="step__time">2020-4-15 17:23</p>
      </div>
      <p class="step__summary">摘要信息</p>
    </div>
  </div>
</div>
```

#### 类型

- `step--process`: 流程步骤器（有先后顺序）
- `step--indicator`: 状态指示器（无逻辑先后关系）

#### 布局方向

- `step--horizontal`: 水平布局
- `step--vertical`: 垂直布局

#### 状态

- `step__item--completed`: 已完成状态
- `step__item--in-progress`: 进行中状态
- `step__item--pending`: 未开始状态

#### 图标类型

- `step__icon-number--green`: 绿色数字图标（已完成/进行中）
- `step__icon-number--gray`: 灰色数字图标（未开始）
- `step__icon-done`: 完成图标
- `step__icon-other--time`: 时间图标
- `step__icon-other--error`: 报错图标
- `step__icon-other--info`: 信息图标
- `step__icon-other--more`: 更多图标

#### 连接线

- `step__line--brand`: 绿色连接线
- `step__line`: 灰色连接线（默认）
- `step__line--hidden`: 隐藏连接线

## 📝 文本样式

### 文本大小

#### 中文字体
```html
<p class="text-01">Text-01 (44px)</p>
<p class="text-02">Text-02 (34px)</p>
<p class="text-03">Text-03 (32px)</p>
<p class="text-04">Text-04 (28px)</p>
<p class="text-05">Text-05 (24px)</p>
<p class="text-06">Text-06 (22px)</p>
<p class="text-07">Text-07 (20px)</p>
```

#### 英文字体
```html
<p class="text-english-01">English Text-01 (42px)</p>
<p class="text-english-02">English Text-02 (32px)</p>
<p class="text-english-03">English Text-03 (30px)</p>
<p class="text-english-04">English Text-04 (26px)</p>
<p class="text-english-05">English Text-05 (22px)</p>
<p class="text-english-06">English Text-06 (20px)</p>
<p class="text-english-07">English Text-07 (18px)</p>
```

#### 数值字体
```html
<p class="text-number-01">HK$1,234.56</p>
<p class="text-number-02">HK$1,234.56</p>
<p class="text-number-03">HK$1,234.56</p>
<p class="text-number-04">HK$1,234.56</p>
<p class="text-number-05">HK$1,234.56</p>
<p class="text-number-06">HK$1,234.56</p>
<p class="text-number-07">HK$1,234.56</p>
```

### 字重

```html
<p class="text-regular">Regular (400)</p>
<p class="text-medium">Medium (500)</p>
<p class="text-semibold">Semibold (600)</p>
```

### 文本颜色

```html
<p class="text-brand">品牌色文本</p>
<p class="text-danger">危险色文本</p>
<p class="text-disabled">禁用文本</p>
<p class="text-white">白色文本</p>
```

## 🛠️ 工具类

### 间距工具类

#### Margin
- `m-010`, `m-020`, `m-030`, `m-040`, `m-050`, `m-060`, `m-070`, `m-080`, `m-090`, `m-100`, `m-110`
- `mt-010` 到 `mt-110` (top)
- `mr-010` 到 `mr-110` (right)
- `mb-010` 到 `mb-110` (bottom)
- `ml-010` 到 `ml-110` (left)

#### Padding
- `p-010`, `p-020`, `p-030`, `p-040`, `p-050`, `p-060`, `p-070`, `p-080`, `p-090`, `p-100`, `p-110`
- `pt-010` 到 `pt-110` (top)
- `pr-010` 到 `pr-110` (right)
- `pb-010` 到 `pb-110` (bottom)
- `pl-010` 到 `pl-110` (left)

### 圆角工具类

- `rounded-010`: 4px
- `rounded-020`: 8px
- `rounded-030`: 12px
- `rounded-040`: 16px
- `rounded-050`: 24px
- `rounded-060`: 32px
- `rounded-full`: 完全圆形

### 布局工具类

- `flex`: 弹性布局
- `flex-col`: 纵向排列
- `items-center`: 垂直居中
- `justify-center`: 水平居中
- `justify-between`: 两端对齐
- `gap-010`, `gap-020`, `gap-030`, `gap-040`, `gap-050`, `gap-060`, `gap-070`, `gap-080`, `gap-090`, `gap-100`, `gap-110`: 间距

### 文本工具类

- `text-left`: 左对齐
- `text-center`: 居中对齐
- `text-right`: 右对齐
- `text-ellipsis`: 单行省略
- `text-clamp-2`: 两行省略
- `text-clamp-3`: 三行省略

## 📱 响应式设计

设计系统包含响应式断点，在移动设备上（宽度 ≤ 768px）：
- 按钮会自动调整为全宽
- 按钮组会变为纵向排列

## 🎯 使用规范

### 按钮使用规则

1. **Large 尺寸按钮**：
   - 单独使用时，默认最小宽度为 304px
   - 左右 padding 为 32px
   - 当文字宽度超出 304px 时，按钮会自动拉伸

2. **Middle 尺寸按钮**：
   - 单独使用时，默认最小宽度为 84px
   - 左右 padding 为 16px
   - 当文字宽度超出 84px 时，按钮会自动拉伸

3. **Disable 状态**：
   - Disable 状态下保留点击功能
   - 点击后的交互效果依业务需求而定

4. **运营按钮**：
   - 应用于 Banner 之上
   - 无需开发介入（设计层面处理）

## 🔗 相关链接

- [Figma 设计系统](https://www.figma.com/design/U0JmLhPEuRjqMVfD1CuPsH/WeChat-Pay-HK-Design-System)

## 📄 许可证

本设计系统由 WeChat Pay HK 团队创建和维护。

## 🎬 动效系统 (Motion System)

### 动效原则

1. **贴合产品**：根据业务属性划分，贴合产品业务，在心智尺寸符合用户心理认知
2. **自然流畅**：在动效运动过程中遵循自然规律，在视觉上是连贯且一致的
3. **清晰准确**：清晰准确地传达信息，有效且有目的的运动，避免不必要的装饰和过分夸张

### 动效时间规范

研究表明，在界面中小于100ms的动效难以被用户识别，超过一秒的动效会让用户有迟滞感。界面中的动效时长一般与元素的大小及运动距离有关。

- **移动设备**：微动效的最佳持续时间为200-500ms
- **平板设备**：动效持续时间比移动设备长30%左右

### 缓动曲线使用指南

#### 线性动效 (Linear)
没有任何缓动的动效称为线性运动，线性运动不受任何物理力量的影响，采用线性运动的动效往往显得很僵硬，不自然。线性动效通常只会用在色彩、hover、按钮点击的状态变化，动效时长较短。

#### 缓出 (Ease-Out)
缓出动效会在开始阶段加速进入屏幕，给用户一种快速响应，操作流畅的心理感受；在动效结束时有自然的减慢速度，给动效一些缓冲时间，可减少快速运动下来带急躁的心理感受。

**参数**：`cubic-bezier(0.33, 1, 0.68, 1)`

#### 缓入 (Ease-In)
缓入动效是指物体以慢速开始并逐渐积累速度加速离开，通常适用于元素离开画面、退场时，重要性降低的场景，保持合理运动的同时可让使元素逐渐快速离开用户视线，不影响用户后续的操作。

**参数**：`cubic-bezier(0.11, 0, 0.5, 0)`

#### 缓入缓出 (Ease-In-Out)
常见的运动曲线，适用于表达持续在用户视线内中的元素动效，例如卡片移动，图片缩放，选项卡切换等转场效果。

**参数**：`cubic-bezier(0.65, 0, 0.35, 1)`

### 动效类型

#### 转场类 (Transition)
UI元素之间的跳转或场景切换，加强页面前后衔接的关联度，让元素之间的过渡更自然连贯，且帮助用户理解界面间的变化和层级关系。

#### 展示类 (Display)
吸引用户的第一视觉，引导用户视觉流向，突出产品功能特点，增强点击率。

#### 引导类 (Guidance)
通过元素的微变化，聚焦用户的视线，引导用户进行相关操作，常用于产品功能提醒，活动通知，新手引导等。

#### 反馈类 (Feedback)
在用户进行操作之后第一时间给与用户相应的视觉反馈，让用户有一定的心理预期，如下拉刷新等。

### 使用示例

```css
/* 基础过渡 */
.element {
  transition: all var(--motion-duration-mobile-medium) var(--easing-ease-out);
}

/* 模态弹层动画 */
.modal {
  animation: slideUp var(--motion-duration-large-ui-open) var(--easing-ease-out);
}

/* 展示类动画 */
.card {
  animation: fadeIn var(--motion-duration-mobile-medium) var(--easing-ease-out);
}

/* 引导类动画 */
.notification {
  animation: pulse 2s var(--easing-ease-in-out) infinite;
}
```

## 📝 更新日志

### v2.3.0 (2024)
- **新增**：Step 步骤器组件
  - 支持水平（Horizontal）和垂直（Vertical）两种布局方式
  - 支持流程步骤器（Process Step）和状态指示器（Status Indicator）两种类型
  - 支持三种状态：已完成（Completed）、进行中（In Progress）、未开始（Pending）
  - 支持多种图标类型：数字图标（绿色/灰色）、完成图标、时间图标、报错图标、信息图标、更多图标
  - 支持连接线样式：绿色线、灰色线、无线
  - 垂直布局支持显示标题、时间、摘要等内容

### v2.2.0 (2024)
- **新增**：Picker 选择器组件
  - 支持单列、双列、三列三种布局类型
  - 包含头部（关闭按钮和标题）、内容区域（可滚动选项列表）、底部操作区（确定按钮）
  - 支持选中状态样式
  - 包含顶部和底部渐变遮罩效果
  - 提供动画参数说明（停止动画时间、惯性滚动参数、滑动阈值等）

### v2.1.0 (2024)
- **修复**：全量检查并补充所有缺失的样式和组件
  - **问题原因**：在初始生成示例和文档文件时，只包含了最常用的样式，遗漏了大量完整的样式定义
  - **修复内容**：
    
    **文本样式系统：**
    - 补充缺失的 Text-05 (24px) 和 Text-07 (20px) 样式示例和文档
    - 补充完整的英文文本样式（text-english-01 到 text-english-07）示例和文档
    - 补充完整的数值文本样式（text-number-01 到 text-number-07）示例和文档
    
    **圆角系统：**
    - 补充缺失的 Radius-010 (4px)、Radius-030 (12px)、Radius-050 (24px) 示例和文档
    - 更新所有圆角值的完整文档和 CSS 变量列表
    
    **间距工具类：**
    - 补充缺失的间距值示例：Space-040 (24px), 060 (40px), 070 (48px), 080 (64px), 090 (80px), 100 (96px), 110 (120px)
    - 补充完整的 Padding 工具类示例（p-010 到 p-110）
    - 补充完整的 Gap 工具类示例（gap-010 到 gap-110）
    - 在 CSS 中添加缺失的 Gap 工具类（gap-040, 060, 070, 080, 090, 100, 110）
    
    **组件：**
    - 补充 Divider 分割线组件的完整示例和文档
    - 补充 Tabs 选项卡组件的完整示例和文档
    - 补充 Icon 图标库的完整示例和文档
    
    **文档完善：**
    - 更新所有 CSS 变量列表，包含完整的定义
    - 更新 README.md 中的设计令牌说明
    - 在导航树中添加所有组件的链接
- **新增**：图标库 (Icon Library) 组件
  - 基础图标样式类 (`.icon`)
  - 图标尺寸变体 (small, medium, large)
  - 图标颜色变体 (primary, brand, danger, disabled)
  - 图标样式变体 (fill, outline)
  - 图标按钮 (`.icon-btn`)
  - 图标与文本组合 (`.icon-with-text`)
- **新增**：Divider 分割线组件
- **新增**：Tabs 选项卡组件

### v2.0.0 (2024)
- 新增完整的动效系统（Motion System）
- 包含时间系统、缓动曲线、动效类型
- 支持转场类、展示类、引导类、反馈类动效
- 响应式动效时间（移动设备/平板设备）

### v1.0.0 (2024)
- 初始版本
- 包含按钮、文本、Banner 等核心组件
- 完整的设计令牌系统
- 响应式支持

