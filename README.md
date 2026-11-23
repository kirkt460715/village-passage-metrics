# 古村出行与布置资料

该项目为村民议事使用的出行观察、分时道路和节日布置信息提供基础读取能力。`data/passages.json` 是匿名合成资料，包含出行需求时段、道路能力、步行条件、便桥变更和已确认通行承诺。

`data/access-windows.json` 带抽样概率的匿名历史行程与一次布置协商使用同一张路网。`observed=false` 表示该行程虽被抽中但实际未观测，时间字段只在观察成立时用于估计。道路按双向记录，步行能力决定可用坡度和台阶，公共服务记录列出开放窗口。

要求 Python 3.11 或更新版本。运行基线检查可使用 `python3 -m unittest discover -s tests`。`src/records.py` 提供基础 JSON 资料读取能力。
