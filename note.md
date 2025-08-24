---
theme: gaia
_class: lead
paginate: true
backgroundColor: #fff
backgroundImage: url('https://marp.app/assets/hero-background.svg')
marp: true
---

# 智能助教本地开发
清华大学计算机系科协 张馨元

---

## Outline
1. 背景
2. Dify 本地开发
3. 优秀案例介绍

---

## 背景
- “挑战杯”一直是清华大学的重要科创竞赛。近年来，大模型技术迅猛发展，越来越多的智能应用涌现。因此，今年的第四十三届挑战杯特别增加"AI助教智能体设计专项赛"，由计算机系科协提供技术支持。
- 本次比赛采用的主要技术栈是开源项目 [Dify](https://dify.ai/)。其门槛较低，即使零基础也能很快轻松上手，也非常方便进行本地部署。
- RyZen AI PC 的特别架构允许以相对较低的成本进行本地大模型部署，并提供 API 接入到 Dify 的 Workflow 中。

--- 
## 本地开发
- 以上的开发流程完全可以借助Ryzen AI PC 实现本地开发，方便快速地构建你自己的智能体。
- 在本地构建Dify应用，并部署Ollama大模型接入到Dify节点。

---

### [Dify 部署](https://github.com/langgenius/dify/?tab=readme-ov-file#quick-start)
1. `git clone git@github.com:langgenius/dify.git`
2. 运行
```bash
cd dify/docker
cp .env.example .env
docker compose up -d
```
3. 在`http://localhost/install`就可以愉快访问 Dify 应用了

---
### Ollama 部署
1. `winget install --id=Ollama.Ollama -e`
2. `ollama pull hf-mirror.com/unsloth/got-oss-20b-GGUF`
3. `ollama serve`
ollama 默认将在`http://localhost:11434`运行

---
### Ollama 接入Dify
现场演示

---

## 优秀案例介绍
- "AEI4U -- 基于 Dify 平台的《模拟电子技术基础》课程助手" 在本次挑战杯中获得特等奖，项目成员是清华大学自动化系的本科生**张博和贾明远**。

---
## Appendix
1. 讲义：https://github.com/Daucloud/amd_summer25
2. `AEI4U` 主页：https://truth-kitchen-37f.notion.site/AEI4U-1c87097e35a88136b686fb1088683809

---
<!--_class: lead-->>
# 谢谢
2025.8.25