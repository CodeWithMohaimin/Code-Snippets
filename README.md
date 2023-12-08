# Here are some of the most uses code snippet that developer use daily.

## 1. For adding an active class & Remove an active class

```javascript

const btns = document.querySelectorAll(".ctrl-btn");
btns.forEach((btn) => {
  btn.addEventListener("click", () => {
    btns.forEach((tab) => {
      tab.classList.remove("active");
    });
    btn.classList.add("active");
  });
});

```
