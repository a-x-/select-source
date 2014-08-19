select-source
=============

Implement parsing declaration source data resource for select html element syntax

# The Idea

HTML:
```html
<select src="/car-types.json" name="car-type" ></select>
...
<script src="/select-source.js">
```

`GET /car-types.json`:
```json
{
  "audi": { "content":"Audi" },
  "vw": { "content":"Volkswagen" },
  "mercedes": { "content":"Mercedes" },
  "delorian": { "content": "DeLorean DMC-12" }
}
```

Rendered HTML:
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

# Usage


# Status

This is under active development stage **(not production ready)**.

| **Idea** | Alpha | Beta | RC | Production |
|:--------:|:-----:|:----:|:--:|:----------:|
|  **Ok**  |   —   |  —   |  — |      —     |


# Demo

# License

All under MIT license.

# Contribution

You're welcome!
I watch github issues and mailbox (me@invntrm.ru).

English typo-fixes are welcome too.
