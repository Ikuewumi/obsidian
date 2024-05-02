## Scroll Snap
```css
.container {
	scroll-snap-type: y mandatory;
}

.child {
	scroll-snap-align: start;
}
```


---

## Encoding Strings
```js
function base64ToBytes(base64) {
  const binString = atob(base64);
  return Uint8Array.from(binString, (m) => m.codePointAt(0));
}

function bytesToBase64(bytes) {
  const binString = String.fromCodePoint(...bytes);
  return btoa(binString);
}

// Usage
bytesToBase64(new TextEncoder().encode("a Ā 𐀀 文 🦄")); // "YSDEgCDwkICAIOaWhyDwn6aE"
new TextDecoder().decode(base64ToBytes("YSDEgCDwkICAIOaWhyDwn6aE")); // "a Ā 𐀀 文 🦄"

```

---

## A Nice Gradient

```css
html {
  --s: 84px; /* control the size*/
  --c1: #f2f2f2;
  --c2: #cdcbcc;
  --c3: #999999;
  
  --_g: 0 120deg,#0000 0;
  background:
    conic-gradient(from    0deg at calc(500%/6) calc(100%/3),var(--c3) var(--_g)),
    conic-gradient(from -120deg at calc(100%/6) calc(100%/3),var(--c2) var(--_g)),
    conic-gradient(from  120deg at calc(100%/3) calc(500%/6),var(--c1) var(--_g)),
    conic-gradient(from  120deg at calc(200%/3) calc(500%/6),var(--c1) var(--_g)),
    conic-gradient(from -180deg at calc(100%/3) 50%,var(--c2)  60deg,var(--c1) var(--_g)),
    conic-gradient(from   60deg at calc(200%/3) 50%,var(--c1)  60deg,var(--c3) var(--_g)),
    conic-gradient(from  -60deg at 50% calc(100%/3),var(--c1) 120deg,var(--c2) 0 240deg,var(--c3) 0);
  background-size: calc(var(--s)*1.732) var(--s);
}
```

Find more at [CSS Patterns](https://css-pattern.com/)


---

## CSS Organization

To not have a headache when dealing with CSS properties, I have decided to follow Kevin Powell's format for organizing my properties and this is a reference to that


```css
selector {
	
	display: flex; /*display stuff*/
	position: relative; /*positioning stuff*/
	padding: 2rem; /*box-model stuff*/
	font-family: 'IBM Plex Sans', system-ui; /*typography*/
	
	/*manipulation*/
	transform: translateX(30px);
	filter: opacity(0.4);
	
	/*misc properties*/
}
```
