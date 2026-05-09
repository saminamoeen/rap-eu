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
## 📌 Analysis

The chart shows a comparison of different EU funding programmes based on budget, accessibility, and innovation.

Horizon Europe has the highest score in innovation and budget, which shows that it strongly supports research and advanced projects. However, its accessibility is lower compared to other programmes, which means it may be more competitive or difficult to access.

Erasmus+ has the highest accessibility score, making it the most accessible programme for students and organisations. However, its innovation score is lower, indicating that it focuses more on education and mobility rather than research.

ESF+ shows balanced scores across all categories, especially in accessibility and budget, which indicates that it supports employment and social inclusion effectively.

Creative Europe has lower scores in innovation but moderate accessibility, which reflects its focus on cultural and creative sectors rather than technical innovation.

Overall, the comparison shows that each programme has different strengths, and the choice depends on the needs of the applicant.
## 📚 Programme Overview

- **Horizon Europe**: Supports research and innovation projects across Europe.
- **Erasmus+**: Focuses on education, student mobility, and international collaboration.
- **ESF+**: Aims to improve employment opportunities and social inclusion.
- **Creative Europe**: Supports cultural and creative industries.
## 🎯 Recommendations

Based on the analysis, users should select funding programmes according to their needs. 
Horizon Europe is suitable for research and innovation-focused projects, while Erasmus+ is more appropriate for education and mobility purposes. ESF+ is beneficial for social and employment-related initiatives, whereas Creative Europe is ideal for cultural and creative sectors.

This comparison can support decision-making by helping applicants choose the most relevant funding programme.
## 🔗 Project Relevance

This dashboard was developed as part of the RAP EU internship project to analyse and compare European funding programmes using data visualisation tools.
## 📚 Programme Overview

- **Horizon Europe** supports research and innovation projects across Europe.
- **Erasmus+** focuses on education, mobility, and international collaboration.
- **ESF+** supports employment, social inclusion, and skills development.
- **Creative Europe** supports cultural and creative sectors.
## 🎯 Recommendations

Different funding programmes support different goals. Horizon Europe is suitable for research and innovation projects, while Erasmus+ is more accessible for education and mobility activities. ESF+ is useful for employment and social inclusion initiatives, and Creative Europe is beneficial for cultural and creative projects.
## 🔗 Project Relevance

This dashboard was developed during the RAP EU internship project to compare European funding programmes through data visualisation and comparative analysis.
