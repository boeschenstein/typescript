# TypeScript

## 5 Differences between regular and arrow functions

<https://dmitripavlutin.com/differences-between-arrow-and-regular-functions/#:~:text=The%20arrow%20function%20doesn't,arrow%20function%20resolves%20this%20lexically.>

### Scope of CallBack

```ts
private myLocalVariable: string = 'can you read this?';

private myCallBack(value: MyObject) {
  // callback runs in the context of execution
  console.warn('myLocalVariable is NOT available', this.myLocalVariable);
};

private myCallBack = (value: MyObject) => {
  // callback runs in the context of declaration
  console.warn('myLocalVariable is available now', this.myLocalVariable);
};
```
