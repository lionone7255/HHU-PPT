# Open Design Prompt - HHU Design System

Copy the prompt below into any AI design tool (Midjourney / DALL-E / Figma AI / 即时设计 AI)
to generate designs matching Hohai University's visual style.

---

## Prompt

### Chinese

```
设计一个河海大学官方风格的视觉设计稿。

【色彩约束】
主色（按使用频率排序）：
  - #00489D
  - #004098
  - #E7E6E6

填充/强调色：
  - #004098
  - #00489D
  - #9CACCE

【字体约束】
推荐字体（按使用频率排序）：
  - 微软雅黑
  - None
  - +mn-ea

【版式约束】
- 比例: 16:9
- 边距: 左 2.5cm / 上 1.5cm / 右 2.5cm / 下 1.5cm
- 对齐: 左对齐为主，标题居中
- 留白充足，学术简洁风格

【风格关键词】
学术 · 简洁 · 专业 · 河海蓝 · 留白 · 几何线条装饰 · 机构感

【禁止】
- 不使用花哨渐变
- 不使用卡通元素
- 不使用非官方配色
```

### English

```
Design an official visual in Hohai University (HHU) institutional style.

[Color Constraints]
Primary colors (by frequency):
  - #00489D
  - #004098
  - #E7E6E6

Fill/accent colors:
  - #004098
  - #00489D
  - #9CACCE

[Typography]
Preferred fonts (by frequency):
  - 微软雅黑
  - None
  - +mn-ea

[Layout]
- Aspect ratio: 16:9
- Margins: ~2.5cm left/right, ~1.5cm top/bottom
- Alignment: left-aligned body, centered headings
- Generous whitespace, academic minimalism

[Style Keywords]
academic, clean, professional, HHU blue, whitespace, geometric line accents, institutional

[Avoid]
- No flashy gradients
- No cartoon elements
- No off-brand colors
```

---

## Usage Examples

1. **Figma / 即时设计 AI**: Paste prompt, set canvas to 1920x1080
2. **Midjourney**: Append `--ar 16:9 --style raw`
3. **DALL-E / ChatGPT**: Use as system prompt or first user message
4. **Python**: Load `design-tokens.json` and inject hex values dynamically

---

## Auto-injection Example (Python)

```python
import json

with open("design-tokens.json") as f:
    tokens = json.load(f)

primary = [c["hex"] for c in tokens["colors"]["text_colors_by_frequency"][:3]]
fonts = list(tokens["typography"]["fonts"].keys())[:2]

prompt = f"Use colors {primary} and fonts {fonts} for HHU style design."
print(prompt)
```
