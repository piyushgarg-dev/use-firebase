# use-firebase-v2

### Simple hook for react-firebase

## Install

```npm i use-firebase-v2```

## DOCS
```js
import useFirebase from 'use-firebase-v2';

const myComponent = () => {

  const docRef = firebase.firestore().collection('myCollection').doc('myDoc');

  const value = useFirebase(docRef);

  return(
    <p>Hello, {value && value.name}</p>
  )
}
```