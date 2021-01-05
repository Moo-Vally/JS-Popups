## JS-Popups
Alternative to Alert() and Prompt()

### How to use info popup

```
openInfoModal('Hello World');
```

### How to use input modal

```
openInputModal('Enter you name', 'unnamed', (modal, input) => {
  if (input.value != null && input.value != '') {
      openInfoModal('Welcome ' + input.value);
  }
  else {
      openInfoModal('Name cannot be empty');
  }
  modal.parentNode.removeChild(modal);
});
```
