# Dashboard

This chart compares key EU funding programmes based on their focus on innovation, collaboration, and societal impact.

## 📊 Funding Comparison
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

## 📊 Project Types
```js
display(
  Plot.plot({
    title: "Project Types",
    marks: [
      Plot.barY(
        [
          { type: "Research & Innovation", value: 5 },
          { type: "Education & Mobility", value: 4 },
          { type: "Employment & Social", value: 4 },
          { type: "Creative & Culture", value: 3 }
        ],
        { x: "type", y: "value" }
      )
    ]
  })
)
```
## 📊 Detailed Comparison

```js
const detailedData = [
  { programme: "Horizon Europe", category: "Budget", value: 5 },
  { programme: "Horizon Europe", category: "Accessibility", value: 3 },
  { programme: "Horizon Europe", category: "Innovation", value: 5 },

  { programme: "Erasmus+", category: "Budget", value: 4 },
  { programme: "Erasmus+", category: "Accessibility", value: 5 },
  { programme: "Erasmus+", category: "Innovation", value: 3 },

  { programme: "ESF+", category: "Budget", value: 4 },
  { programme: "ESF+", category: "Accessibility", value: 4 },
  { programme: "ESF+", category: "Innovation", value: 3 },

  { programme: "Creative Europe", category: "Budget", value: 3 },
  { programme: "Creative Europe", category: "Accessibility", value: 4 },
  { programme: "Creative Europe", category: "Innovation", value: 2 }
];

display(
  Plot.plot({
    title: "Detailed Comparison of Funding Programmes",
    x: { label: "Programme" },
    y: { label: "Score" },
    color: { legend: true },
    marks: [
      Plot.barY(detailedData, {
        x: "programme",
        y: "value",
        fill: "category",
        fx: "category"
      })
    ]
  })
);
```

## 📌 Key Insights

- Horizon Europe strongly supports research and innovation  
- Erasmus+ focuses on education and mobility  
- ESF+ supports employment and social inclusion  
- Creative Europe promotes cultural and creative sectors  

## 🌍 Who Can Apply?

- Universities  
- Startups  
- NGOs  
- Public sector organisations
## 📊 Detailed Comparison

```js
const detailedData = [
  { programme: "Horizon Europe", category: "Budget", value: 5 },
  { programme: "Horizon Europe", category: "Accessibility", value: 3 },
  { programme: "Horizon Europe", category: "Innovation", value: 5 },

  { programme: "Erasmus+", category: "Budget", value: 4 },
  { programme: "Erasmus+", category: "Accessibility", value: 5 },
  { programme: "Erasmus+", category: "Innovation", value: 3 },

  { programme: "ESF+", category: "Budget", value: 4 },
  { programme: "ESF+", category: "Accessibility", value: 4 },
  { programme: "ESF+", category: "Innovation", value: 3 },

  { programme: "Creative Europe", category: "Budget", value: 3 },
  { programme: "Creative Europe", category: "Accessibility", value: 4 },
  { programme: "Creative Europe", category: "Innovation", value: 2 }
];

display(
  Plot.plot({
    title: "Detailed Comparison of Funding Programmes",
    x: { label: "Programme" },
    y: { label: "Score" },
    color: { legend: true },
    marks: [
      Plot.barY(detailedData, {
        x: "programme",
        y: "value",
        fill: "category",
        fx: "category"
      })
    ]
  })
);
```