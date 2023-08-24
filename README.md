# TypeScript

## Scope of CallBack

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
