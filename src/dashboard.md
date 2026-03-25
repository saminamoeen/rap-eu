# RAP EU Dashboard

## Revenue Growth Trends
This section will show how revenue is changing over time.

## Sample Data Chart
This chart is a simple example of how business data can be shown in the dashboard.

```js
const salesData = [
  { month: "Jan", sales: 120 },
  { month: "Feb", sales: 150 },
  { month: "Mar", sales: 180 },
  { month: "Apr", sales: 170 },
  { month: "May", sales: 210 }
]

display(
  Plot.plot({
    y: { grid: true, label: "Sales" },
    x: { label: "Month" },
    marks: [
      Plot.barY(salesData, { x: "month", y: "sales" })
    ]
  })
)
```
