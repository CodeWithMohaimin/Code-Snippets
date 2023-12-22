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

## 2. When Scroll down & When scroll up

```javascript

function handleScroll(event) {
  if (event.deltaY > 0) {
    homeUpperContainer.classList.add("active");
  } else if (event.deltaY < 0) {
    homeUpperContainer.classList.remove("active");
  }
}

homeContainer.addEventListener("wheel", handleScroll);

```

## 3. Automatic Send Connect from console

```javascript



document.querySelectorAll('[data-testid="connect-button"]').forEach((item) => {
  item.click();

document.querySelectorAll('[data-testid="connect-without-message-button"]').forEach((popupSendButton) => {
  popupSendButton.click();

  });
});




```
