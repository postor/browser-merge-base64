# canvas-merge-images

## install

```
yarn add canvas-merge-images
```

## usage

```
import { mergeFile } from 'canvas-merge-images'

let fileInput = document.getElementById('fileinput')
let preview = document.getElementById('preview')

fileInput.onchange = async () => {
  if (!fileInput.files) return
  let base64 = await mergeFile(fileInput.files)
  preview.src = base64
  console.log(base64)
}
```

## try on your own

```
git clone this_repo
cd repo
yarn
yarn dev
```

![screenshot](./screenshot.gif)