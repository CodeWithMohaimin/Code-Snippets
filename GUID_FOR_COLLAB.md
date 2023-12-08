# You have to write all the Code-Snippet in the README.md file.

Like this way

````
## List_Number. code_use_case

```Language_Name

const btns = document.querySelectorAll(".ctrl-btn");
btns.forEach((btn) => {
  btn.addEventListener("click", () => {
    btns.forEach((tab) => {
      tab.classList.remove("active");
    });
    btn.classList.add("active");
  });
});

````

```

```

Just Write the code snippet and send a pull request.
