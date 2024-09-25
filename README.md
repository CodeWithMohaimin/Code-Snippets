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

## 4. Automatic Send Friend Request

```javascript


document.querySelectorAll('[aria-label="Add friend"]').forEach((item) => {
  item.click();
});



```

## 5. Change Existing Git Repo To New

```javascript


git remote set-url origin https://github.com/CodeWithMohaimin/Wordpress.git

git remote remove origin
git remote add origin https://github.com/CodeWithMohaimin/Wordpress.git

git push -u origin master




```

## 6. Automatic Unfollow

```javascript

document.querySelectorAll('[aria-label="Manage"]').forEach((item, i) => {
    setTimeout(() => {
        item.click();
        console.log(`Clicked Manage button for item ${i}`);

        setTimeout(() => {
            const unfriendButton = document.querySelector('img[src="https://static.xx.fbcdn.net/rsrc.php/v3/yw/r/Kluyv0pwyPt.png"]');
            if (unfriendButton) {
                unfriendButton.click();
                console.log(`Clicked Unfriend for item ${i}`);

                setTimeout(() => {
                    const confirmButton = document.querySelector('[aria-label="Confirm"]');
                    if (confirmButton) {
                        confirmButton.click();
                        console.log(`Confirmed Unfriend for item ${i}`);
                    } else {
                        console.log(`No confirm button found for item ${i}`);
                    }
                }, 1000);

            } else {
                console.log(`Unfriend button not found for item ${i}`);
            }
        }, 1000);

    }, i * 3000);
});




```
