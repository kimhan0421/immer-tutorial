- 설치

```
yarn add immer
```

- immer로 바꾸기

```javascript
//array에 새로운 등록
setData({
  ...data,
  array: data.array.concat(info),
});
```

```javascript
//array에 새로운 등록
setData(
  produce(data, (draft) => {
    draft.array.push(info);
  })
);
```
