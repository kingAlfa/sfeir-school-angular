<!-- .slide: class="sfeir-basic-slide with-code" -->
# Communication parent - enfant: @Input
<ul>
    <li>Enfant</li>
</ul>
<br>
```typescript
import { Component, Input} from '@angular/core';
@Component({
   selector: "app-child"
})
export class ChildComponent {
   @Input() name: string;
}
```
<!-- .element: class="big-code" -->
<br>
<ul>
    <li>Parent - template</li>
</ul>
<br>
```html
<section>
    <app-child [name]="person.name"></app-child>
</section>
```
<!-- .element: class="big-code" -->
