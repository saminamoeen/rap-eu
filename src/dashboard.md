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