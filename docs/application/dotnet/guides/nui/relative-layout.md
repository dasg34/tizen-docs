# Relative Layout

`RelativeLayout` calculates the size and position of all the children based on their relationship to each other.

Here are the attached properties of `RelativeLayout`:

| Property               | Type            | Description  |
| -----------------------| --------------- | ------------ |
| `LeftTarget`           | View            | Gets or sets the left side edge of the child view relative to the given target view.|
| `RightTarget`          | View            | Gets or sets the right side edge of the child view relative to the given target view.|
| `TopTarget`            | View            | Gets or sets the top side edge of the child view relative to the given target view.|
| `BottomTarget`         | View            | Gets or sets the bottom side edge of the child view relative to the given target view.|
| `LeftRelativeOffset`   | float           | Gets or sets the relative offset for left target. <br /> When value is 0 the left edges of the left target and child view are aligned.<br/> When value is 1 the left edge of the child view is aligned to the right edge of the left target. |
| `RightRelativeOffset`  | float           | Gets or sets the relative offset for right target. <br /> When value is 0 the right edge of the child view is aligned to the left edge of the right target.<br/> When value is 1 the right edges of the right target and child view are aligned.
| `TopRelativeOffset`    | float           | Gets or sets the relative offset for top target. <br /> When value is 0 the top edges of the top target and child view are aligned.<br/> When value is 1 the top edge of the child view is aligned to the bottom edge of the top target.
| `BottomRelativeOffset` | float           | Gets or sets the relative offset for bottom target. <br /> When value is 0 the bottom edge of the child view is aligned to the top edge of the right target.<br/>When value is 1 the bottom edges of the bottom target and child view are aligned.
| `BottomRelativeOffset` | float           | Gets or sets the relative offset for bottom target. <br /> When value is 0 the bottom edge of the child view is aligned to the top edge of the right target.<br/>When value is 1 the bottom edges of the bottom target and child view are aligned.
| `HorizontalAlignment`  | RelativeLayout.Alignment| Gets or sets the horizontal alignment of this child view.|
| `VerticalAlignment`  | RelativeLayout.Alignment| Gets or sets the vertical alignment of this child view.|
| `FillHorizontal`  | bool | Gets or sets the boolean value whether child fills its horizontal space.|
| `Fillvertical`  | bool | Gets or sets the boolean value whether child fills its vertical space.|

<a name="targetandrelativeoffset"></a>
## Target And RelativeOffset
`Target` and `RelativeOffset` determine a size for layout space.

`Target` indicates the target view that each edge of layout space is aligned with. default value is `null` that means parent relative layout.

`RelativeOffset` moves a each edge of layout space in proportion to target view size.<br/>
When the value is `0.0f`, edge of layout space is aligned with left/top edge of target view.<br/>
When the value is `1.0f`,  edge of layout space is aligned with right/bottom edge of target view.

