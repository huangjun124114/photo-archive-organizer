# 已迁移 · MOVED

> ⚠️ **本仓库已归档，不再更新。**

`photo-archive-organizer` 已迁入统一的 skills 仓库：

**新地址 → https://github.com/huangjun124114/skills/tree/main/skills/photo-archive-organizer**

```bash
git clone https://github.com/huangjun124114/skills.git
# skill 位于 skills/photo-archive-organizer/
```

---

## 迁移记录

| 项 | 值 |
|---|---|
| 迁移时间 | 2026-09-16 |
| 迁出 commit | [`4993d2e`](https://github.com/huangjun124114/photo-archive-organizer/commit/4993d2ee6ef9fd5f0382640418dc9edd762676cb) |
| 迁入位置 | [`skills/photo-archive-organizer`](https://github.com/huangjun124114/skills/tree/main/skills/photo-archive-organizer) |
| 内容变更 | 无，逐文件原样搬迁 |

本仓库保留为历史归档，代码与文档内容已完整迁至新仓库。后续所有更新请前往新地址。

---

## 原 README 内容（归档快照）

<details>
<summary>点击展开</summary>

# 家庭相册整理专家 · photo-archive-organizer

家庭相册整理技能 —— 多源合并 / 筛选归档 / 六闸校验 / Windows 沙箱适配。

把散乱照片整理成「YYYYMM-事件名」结构化相册，支持两种模式：

- **模式 A：迁移合并** —— 多来源目录 → 共享相册，迁移，一张不丢
- **模式 B：筛选归档** —— 散乱照片 → 精选主题相册，筛选，大量剔除

含六道检验闸门与 Windows 沙箱适配，基于 6,763 张家庭照片实战沉淀。

## 结构

```
├── SKILL.md                     # skill 主文档
├── README.md
├── references/                  # 按需加载的参考文档（11 篇）
│   ├── terminology.md
│   ├── date-inference.md
│   ├── naming-rules.md
│   ├── classifier-recipes.md
│   ├── quality-scoring.md
│   ├── verification-gates.md
│   ├── pitfalls.md
│   ├── report-template.md
│   ├── worked-example.md
│   └── scripts-guide.md
└── scripts/                     # 模式 B 7 个 + 模式 A 9 个
    ├── _common.py
    ├── date_infer.py
    ├── extract_features.py
    ├── cluster_events.py
    ├── train_classifier.py
    ├── make_contact_sheet.py
    ├── verify_gates.py
    ├── safe_delete.py
    ├── migrate.py
    ├── fix_ext.py
    ├── normalize_names.py
    ├── organize_loose.py
    ├── analyze_pending.py
    ├── apply_pending.py
    ├── backup.py
    ├── scan.py
    └── verify.py
```

## 依赖

Python 3.10+、`Pillow`、`pillow-heif`、`numpy`、`scikit-learn`。

## License

MIT

</details>
