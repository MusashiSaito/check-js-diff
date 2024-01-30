# 差分確認

```
$ acorn before.js > after-format.json
$ acorn after.js > before-format.json

```

## 差分確認

```
$ batdiff before-format.json after-format.json
```

## 詳細差分確認

```
$ batdiff before-format.json after-format.json | grep -v "start" | grep -v "end" | grep "^[+-]" | less >> output.txt
```

# 前提

```
npm install -g acorn
```
