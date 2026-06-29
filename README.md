# HHU Design System

Visual design token extraction from Hohai University PPT templates (6 themed + icon library).
用途: Open Design reference, AI prompt injection, brand consistency auditing.

---

## 1. Color Tokens

### Text Colors (Top 5 by frequency)

| Rank | HEX | Role | Count |
|------|-----|------|-------|
| 1 | `#00489D` | blue primary | 8 |
| 2 | `#004098` | blue primary | 8 |
| 3 | `#E7E6E6` | light gray bg | 8 |
| 4 | `#13489D` | blue primary | 7 |
| 5 | `#D00A09` | red accent | 6 |

### Shape/Fill Colors (Top 5)

| Rank | HEX | Role | Count |
|------|-----|------|-------|
| 1 | `#004098` | blue primary | 20 |
| 2 | `#00489D` | blue primary | 10 |
| 3 | `#9CACCE` | mixed | 10 |
| 4 | `#D00A09` | red accent | 7 |
| 5 | `#123D89` | mixed | 4 |

### Palette Classification

- **Warm/Accent**: #D00A09, #C00000, #D22624, #DD1615, #D00A09
- **Cool/Primary**: #00489D, #004098, #13489D, #074D9F, #123E89
- **Neutral**: #E7E6E6, #FFF6E9, #778495, #E7E6E6

---

## 2. Typography Tokens

### Font Families

| Font | Normal | Bold | Total |
|------|--------|------|-------|
| 微软雅黑 | 263 | 122 | 385 |
| None | 0 | 45 | 45 |
| +mn-ea | 5 | 0 | 5 |
| 思源黑体 CN Medium | 4 | 0 | 4 |
| 思源黑体 CN Normal | 1 | 1 | 2 |

### Font Sizes

| Size (pt) | Count | Role |
|-----------|-------|------|
| 20 | 97 | Heading 3 |
| 14 | 88 | Body |
| 28 | 14 | Heading 2 |
| 24 | 12 | Heading 2 |
| 19 | 12 | Heading 3 |
| 16 | 12 | Body |
| 23 | 10 | Heading 3 |
| 60 | 9 | Heading 1 |

---

## 3. Layout Tokens

- **Slide Size**: 16:9 (33.87cm x 19.05cm)
- **Average Margins**: L 0.47cm / T -0.14cm / R 2.0cm / B 1.64cm
- **Total Slides Analyzed**: 70

---

## 4. Assets

252 deduplicated images extracted to `assets/`.

---

## 5. Structured Data

Full extraction in `design-tokens.json`:
- `colors` - all extracted colors with frequency
- `typography` - font, size, weight statistics
- `layout` - per-slide margin and alignment data
- `placeholders` - placeholder usage stats
- `images` - embedded image inventory
- `shape_usage` - shape type statistics

---

## 6. Open Design Prompt

See `open-design-prompt.md` for copy-paste ready prompts.
