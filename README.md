# obsidian-code-block-snippet



## How to install

1. Download the files (Code -> Download ZIP)
2. Open your Obsidian.md vault in explorer
3. Copy and paste the .obsidian folder in it
4. Go to: Obsidian app -> Settings -> Appearance -> CSS Snippets



- `CodeBlock.css`

![CodeBlock](./CodeBlock.png)



- `VuepressFix.css`

![base](./base.png)



# Test Code

- `Test Code`



# H1
## H2

### H3
#### H4
##### H5
###### H6

> Hello World

 - 1
	- 2
		- 3


`Hellow World`


```html
<template>
  <div class="app-container home">
    <button @click="testRequest">testRequest</button>
  </div>
</template>

<script setup name="Index" lang="ts">
  import request from "@/utils/request";

  const testRequest = () => {
    request({
      url: "/",
      method: "get",
    }).then((result: any) => {
      console.log(result);
    });
  };
</script>
```

```ts
const sessionCache = {
  get(key: string) {
    if (!sessionStorage) {
      return null
    }
    if (key == null) {
      return null
    }
    return sessionStorage.getItem(key)
  },
  getJSON(key: string) {
    const value = this.get(key)
    if (value != null) {
      return JSON.parse(value)
    }
  },
  remove(key: string) {
    sessionStorage.removeItem(key)
  },
}
```

```java
public class main {
    public static void main(String[] args){
        String s = new String("Hello World");
        System.out.println(s);
    }
}
```