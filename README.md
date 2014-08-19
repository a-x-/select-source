select-soutce
=============

Implement parsing declaration source data resource for select html element syntax

## The Idea

html:
```html
<select src="<url>" name="car-type" ></select>
...
<script src="/select-source.js">
```

`GET <url>`:
```json
{
  "audi": { "content":"Audi" },
  "vw": { "content":"Volkswagen" },
  "mercedes": { "content":"Mercedes" },
  "delorian": { "content": "DeLorean DMC-12" }
}
```

rendered html:
```html
<select src="<url>" name="car-type" >
 <option value="audi">Audi</option>
 <option value="vw">Volkswagen</option>
 <option value="mercedes">Mercedes</option>
 <option value="delorian">DeLorean DMC-12</option>
</select>
...
<script src="/select-source.js">
```
