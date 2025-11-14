**"How can I perfectly center an element (`.child`) both horizontally and vertically inside its container (`.parent`) using Flexbox?"**

---

## 🎯 Answer: Perfect Centering with Flexbox

You can perfectly center a child element inside its flex container using the CSS property **`margin: auto;`** on the **child element**.

### CSS Code

```css
.parent {
  display: flex; /* 1. Turn the container into a flex container */
  height: 300px; /* Define container size */
}

.child {
  width: 100px;
  height: 100px;
  margin: auto; /* 2. The magic: absorbs all extra space on all sides */
}
```

### Explanation

When a child item is inside a **flex container** (an element with `display: flex`), setting its **`margin`** to **`auto`** causes the margins to automatically absorb all the available extra space in both the main axis (horizontal by default) and the cross-axis (vertical by default). By absorbing the space equally on all four sides, the item is centered perfectly in the middle of the container.
