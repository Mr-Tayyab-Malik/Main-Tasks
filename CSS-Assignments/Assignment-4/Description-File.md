# Box Model Task
---
## What I did
---
I made a div and changed its content width, padding and border to see how the total size changes. Then I did the same with height.
---
## Code Used
---
div{
    width: 300px;
    height: 300px;
    border-radius: 10px;
    border: 15px dotted black;
    margin-top: 50px;
    margin-left: 200px;
    padding: 50px;
}
---
## Observation
- Padding and border are added on top of width and height, so the box gets bigger
- Width uses left + right values. Height uses top + bottom values.
- With box-sizing: border-box the box stays 300px x 300px and the content area shrinks instead.
