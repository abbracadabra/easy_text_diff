# easy_text_diff
- 支持自定义渲染行（例如假如比对文本是json，有需求要求能在每行后显示忽略、取消忽略json path按钮，忽略的json path路径覆盖行置灰，这需要比对组件能自定义渲染行）
- 相同行收起展开
- 支持两侧对比

# todo
- 单侧展示diff
- 支持展示行内的modify（在加工diff结果时，对remove add顺序的前后两个diff片段判断行数是否一致，若一致则对其一行一行字符级比对）

# 比对步骤
- 用diff-match-patch生成文本diff（行转uniq char token、uniq char token字符级diff、diff char片段还原line）
- diff结果加工，生成适合前端渲染的结构
- 相同行collapse
