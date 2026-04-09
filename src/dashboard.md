# RAP EU Dashboard
# Digital Bauhaus Funding Dashboard (EU Focus)

## 🎯 Project Overview
This dashboard presents research on funding opportunities for Digital Bauhaus-type initiatives focused on:
- Digital innovation
- Sustainability / green transition
- Creative industries
- Skills development & youth engagement

---

## 💰 Funding Opportunities

### 1. Horizon Europe
- What it funds: Innovation, sustainability, research projects
- Who can apply: Universities, startups, organisations (often in partnerships)
- Key requirements: Cross-country collaboration, strong impact

---

### 2. Erasmus+
- What it funds: Education, youth, skills development, mobility
- Who can apply: Universities, NGOs, youth organisations
- Key requirements: Learning outcomes, collaboration across countries

---

### 3. European Social Fund Plus (ESF+)
- What it funds: Employment, skills, social inclusion
- Who can apply: Governments, NGOs, training organisations
- Key requirements: Focus on skills, inclusion, job creation

---

### 4. Creative Europe
- What it funds: Cultural & creative industries
- Who can apply: Creative organisations, cultural institutions
- Key requirements: Innovation + cultural impact

---

## 📊 Insights (What gets funded)
- Projects combining **digital + sustainability**
- Cross-border collaboration (EU partnerships)
- Youth-focused skills development
- Innovation with real-world impact

---

## ❌ What does NOT get funded
- Pure business ideas without social impact
- Single-person projects (usually need teams)
- Projects without EU collaboration

---

## 📈 Next Steps
- Add charts to compare funding programmes
- Visualise types of projects supported
## 📊 Funding Focus Comparison
```js
import * as Plot from "@observablehq/plot";

const data = [
  { programme: "Horizon Europe", level: 5 },
  { programme: "Erasmus+", level: 4 },
  { programme: "ESF+", level: 4 },
  { programme: "Creative Europe", level: 3 }
];

display(
  Plot.plot({
    title: "Funding Program Comparison",
    marks: [
      Plot.barY(data, { x: "programme", y: "level" })
    ]
  })
);
```
