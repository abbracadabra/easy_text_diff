# easy_text_diff
- 支持自定义渲染行
- 相同行收起展开
- 支持两侧对比

# todo
- 单侧展示diff
- 支持展示行内的modify

# 比对步骤
- 用diff-match-patch生成文本diff（行转uniq char token、uniq char token字符级diff、diff char片段还原line）
- diff结果加工，生成适合前端渲染的结构
- 相同行collapse
