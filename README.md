# ng-ts-snippets
Angular + TypeScript code abbreviations snippets for Atom

![](https://github.com/ProjectsZ/ng-ts-snippets/blob/master/drawable-xxhdpi-icon.png)

### TypeScript Snippets

|Snippet o Abbrev                |    Information           |
| ------------------------------ | ------------------------ |
|[imp_ts](#imp_ts)               |import basic init         |
|[exp_ts](#exp_ts)               |export basic init         |
|[ng-c](#ng-c)                   |Angular generate Component|
|[ng-rt](#ng-rt)                 |Angular generate Routes   |
|[ng-s](#ng-s)                   |Angular generate Service  |
|[ng-pipe](#ng-pipe)             |Angular generate Pipe     |
|[ng-d](#ng-d)                   |Angular generate Directive|

### TypeScript personalized

|Snippet o Abbrev                                  |    Information                       |
| ------------------------------------------------ | ------------------------------------ |
|[ng-new-FormGroup](#ng-new-FormGroup)             |Angular Class FormGroup (STABLE)      |
|[ng-ng-meth_extractData](#ng-ng-meth_extractData) |Angular response object (to .map())   |
|[ng-meth_handleError](#ng-meth_handleError)       |Angular response object (to .catch()) |

### Import personalized

|Snippet o Abbrev                        |    Information                             |
| -------------------------------------- | ------------------------------------------ |
|[imp_ts](#imp_ts)                       |import basic init                           |
|[imp_ts_m](#imp_ts_m)                   |import all modules in the index.module      |
|[imp_ts_components](#imp_ts_components) |import folder-structure for components      |
|[imp_ts_c](#imp_ts_c)                   |import all components in the index.component|
|[imp_ts_services](#imp_ts_services)     |import folder-structure for services        |
|[imp_ts_s](#imp_ts_s)                   |import all services in the index.service    |
|[imp_ts_interfaces](#imp_ts_interfaces) |import folder-structure for interfaces      |
|[imp_ts_pipes](#imp_ts_pipes)           |import folder-structure for pipes           |
|[imp_ts-all](#imp_ts-all)               |import folder-structure for pipes           |

### Import JS library

|Snippet o Abbrev                                  |    Information       |
| ------------------------------------------------ | -------------------- |
|[imp_ts-RxJS_map](#imp_ts-RxJS_map)               |import map observable |
|[imp_ts-RxJS_Observable](#imp_ts-RxJS_Observable) |import observable     |

### Import all Core Angular

|Snippet o Abbrev                         |    Information                                     |
| --------------------------------------- | -------------------------------------------------- |
|[imp_ts-router](#imp_ts-router)          |import router all                                   |
|[imp_ts-forms_tml](#imp_ts-forms_tml)    |import Forms (all x Template)                       |
|[imp_ts-forms_data](#imp_ts-forms_data)  |import Forms (all x Data)                           |
|[imp_ts-http](#imp_ts-http)              |import (http, headers, options and res)             |
|[imp_ts-animations](#imp_ts-animations)  |import (trigger, state, style, animate, transition) |
|[imp_ts-ngfire2](#imp_ts-ngfire2)        |import (AngularFire and FirebaseListObservable)     |

### Export personalized

|Snippet o Abbrev                          |    Information           |
| ---------------------------------------- | ------------------------ |
|[exp_ts](#exp_ts)                         |export (basic, default)   |
|[exp_ts-class](#exp_ts-class)             |export class              |
|[exp_ts-const](#exp_ts-const)             |export const              |
|[exp_ts-class_impl](#exp_ts-class_impl)   |export class + Implements |
|[exp_ts-intf](#exp_ts-intf)               |export interface          |

### HTML Snippets

|Snippet o Abbrev                             |    Information                    |
| ------------------------------------------- | --------------------------------- |
|[ngIf](#ngIf)                                |Directive NgIf                     |
|[ngFor](#ngFor)                              |Directive NgFor (NgForOf)          |
|[ngModel](#ngModel)                          |Directive NgModel                  |
|[ngRouterOutlet](#ngRouterOutlet)            |Directive RouterOutlet (STABLE)    |
|[ng-rtLink](#ng-rtLink)                      |Directive RouterLink               |
|[ng-rtLinkActive](#ng-rtLinkActive)          |Directive RouterLinkActive         |
|[ngStyle](#ngStyle)                          |Directive NgFor                    |
|[ngClass](#ngClass)                          |Directive NgClass                  |
|[ngSwitch](#ngSwitch)                        |Directive NgSwitch                 |
|[ng_propty-formGroup_event-submit](#ng_pfes) | formGroup event submit            |
|[ng-FormControlName](#ng-FormControlName)    |Directive FormControlName (STABLE) |
|[ng-FormGroupName](#ng-FormGroupName)        |Directive FormGroupName (STABLE)   |
|[ng-FormArrayName](#ng-FormArrayName)        |Directive FormArrayName (STABLE)   |

### NOTE:

> Use key TAB of the keyboard or Modify text ^^^^^^^^^^ in code generated !!...

### imp_ts

`imp_ts` generating a import basic init.

```ts
import { ^^^^^^^^^^ } from '^^^^^^^^^^';

```

### exp_ts

`exp_ts` Angular export (basic, default)

```ts
export { ^^^^^^^^^^ } from '^^^^^^^^^^';

```

### exp_ts-class

`exp_ts-class` export a class.

```ts
export class ^^^^^^^^^^ {

}

```

### exp_ts-class_impl

`exp_ts-class_impl` export class + implements (methods).

```ts
export class ^^^^^^^^^^ implements ^^^^^^^^^^ {

}

```

### exp_ts-const

`exp_ts-const` export a const.

```ts
export const ^^^^^^^^^^ = [
  {

  }
];
```

### ng-c

`ng-c` generating a Component basic, **Note:** *import + declarations in file module (app.module.ts) or ignore this message.*

```ts
import { Component } from '@angular/core';

@Component({
  selector: '^^^^^^^^^^',
  templateUrl: './^^^^^^^^^^.component.html',
  styleUrls: ['./^^^^^^^^^^.component.css'],
  animations: [  ]
})
export class ^^^^^^^^^^Component {
  /* Note: import + declarations in file module (~.module.ts) or ignore this message. */
  constructor(  ){  }

}
```

### ng-c_lite

`ng-c_lite` generating a Component basic, **Note:** *import + declarations in file module (app.module.ts) or ignore this message.*

```ts
import { Component } from '@angular/core';

@Component({
  selector: '^^^^^^^^^^',
  template: `

  `,
  styles: [ '  ' ],
  animations: [  ]
})
export class ^^^^^^^^^^Component {
  /* Note: import + declarations in file module (~.module.ts) or ignore this message. */
  constructor(  ){  }

}
```

### ng-rt

`ng-rt` generating a Routing Component basic, **Note:** *add tag <router-outlet> in component, import + imports in file module (app.module.ts) he const (app_routing); or ignore this message.*

```ts
import { RouterModule, Routes } from '@angular/router';

import { ^^^^^^^^^^ } from '^^^^^^^^^^';

const NAV_ROUTES: Routes = [
  { path: '^^^^^^^^^^', component: ^^^^^^^^^^ },
  { path: '**', pathMatch:'full', redirectTo: '^^^^^^^^^^' }

];

export const app_routing = RouterModule.forRoot( NAV_ROUTES );
/* Note:
  * add tag <router-outlet></router-outlet> in file component (~.component.html)
  * Need import and imports `app_routing`  in file module (~.module.ts) or ignore this message. */

];

export const app_routing = RouterModule.forRoot( NAV_ROUTES );
/* Note:
  * add tag <router-outlet></router-outlet> in file component (~.component.html)
  * Need import and imports `app_routing`  in file module (~.module.ts) or ignore this message. */

```

### ng-rtRouterOutlet

`ng-rtRouterOutlet` generating a Directive [RouterOutlet (STABLE)](https://angular.io/api/router/RouterOutlet "RouterOutlet (STABLE)")

```html
<router-outlet
  (activate)='onActivate($event)'
  (deactivate)='onDeactivate($event)'></router-outlet>
```

### ng-rtLink

`ng-rtLink` generating a Directive [RouterLink](https://angular.io/api/router/RouterLink "RouterLink") in HTML

```html
[routerLink]="['^^^^^^^^^^']"
```

### ng-rtLinkActive

`ng-rtLinkActive` generating a Directive [RouterLinkActive (STABLE)](https://angular.io/api/router/RouterLinkActive "RouterLinkActive (STABLE)"), in HTML. Lets you add a CSS class to an element when the link's route becomes active.

```html
routerLinkActive="^^^^^^^^^^"
```

### ng-s

`ng-s` Angular generate service

```ts
import { Injectable } from '@angular/core';

@Injectable()
export class ^^^^^^^^^^Service {
  /* Note: import + providers in file module (~.module.ts) or ignore this message. */
  constructor(  ){  }

}
```

### ng-pipe

`ng-pipe` Angular generate pipe

```ts
import { Pipe, PipeTransform } from '@angular/core';

@Pipe({
  name: '^^^^^^^^^^'
})
export class ^^^^^^^^^^Pipe implements PipeTransform {
  /* Note: import + declarations in file module (~.module.ts) or ignore this message. */
  constructor(  ){  }

  transform( ^^^^^^^^^^: ^^^^^^^^^^, args: any[] ): ^^^^^^^^^^ {
    return ;
  }

}

```

### ng-d

`ng-d` Angular generate directive

```ts
import { Directive, Input } from '@angular/core';

@Directive({ selector: '[^^^^^^^^^^]' })
export class ^^^^^^^^^^Directive {



  constructor(  ){  }

  @Input(  ) set ^^^^^^^^^^ ( ^^^^^^^^^^: boolean ) {

  }

  /* Note: import + declarations in file module (~.module.ts) or ignore this message. */
}

```

### ng-new-FormGroup

`ng-new-FormGroup` Angular Class FormGroup (STABLE)

```ts
const ^^^^^^^^^^ = new FormGroup({
  ^^^^^^^^^^: new FormControl( '^^^^^^^^^^' ),
  ^^^^^^^^^^: new FormControl( '', Validators.^^^^^^^^^^ ),
  ^^^^^^^^^^: new FormArray([
                    new FormControl ( '', Validators.^^^^^^^^^^)
                   ])
});
/* Note: add he FormControlName (the values ${2:^^^^^^^^^^}" and "${4:^^^^^^^^^^}", etc ... ) in tag input (~.component.html)
         add he FormArrayName ( ${6:^^^^^^^^^^}", etc ... ) in a tag what container he tag input (~.component.html) */

```

### ng-meth_extractData

`ng-meth_extractData` Angular - response object

```ts
private extractData(res: Response) {
  let body = res.json();
  return body.data ||  { };
  /* In the above snippet we are transforming response to the json format by doing res.json().
   *? Make no assumptions about the server API. Not all servers return an object with a data property.*/
}
```

### ng-meth_handleError

`ng-meth_handleError` Angular - error handling

```ts
private handleError(error: any) {
  /* In a real world app, we might use a remote logging infrastructure.
   * We'd also dig deeper into the error to get a better message */
  let errMsg = (error.message) ? error.message :
      error.status ? `${error.status} - ${error.statusText}` : 'Server error';
  console.error(errMsg); /*log to console instead*/
  return Promise.reject(errMsg);
  // return Observable.throw(errMsg);
}
```

### imp_ts-router

`imp_ts-router` Angular import (routes all)

```ts
/* routes, Know where the page you are and where you want to move, see the state in which it is, going to say that you can activate that route or not (implements in class)... */
import { Router, ActivatedRouteSnapshot, RouterStateSnapshot, CanActivate } from '@angular/router';

```

### imp_ts-forms_tml

`imp_ts-forms_tml` Angular import Forms (all x Template)

```ts
/* Note: Need import and imports FormsModule in file module (~.module.ts) or ignore this message. */
import { NgForm } from '@angular/forms';

```

### imp_ts-forms_data

`imp_ts-forms_data` Angular import Forms (all x data)

```ts
/* Note: Need import and imports FormsModule and ReactiveFormsModule in file module (~.module.ts) or ignore this message. */
import { FormGroup, FormControl, FormArray, Validators } from '@angular/forms';

```

### imp_ts-http

`imp_ts-http` Angular import (http, headers, options and res)

```ts
import { Http, Headers, RequestOptions, Response } from '@angular/http'; /* Note: http, headers, options and res work in a service (~.service.ts) or ignore this message. */

```

### imp_ts-animations

`imp_ts-animations` Angular import (trigger, state, style, animate, transition)

```ts
/* Note: Need import and imports BrowserAnimationsModule in file module (~.module.ts) or ignore this message. */
import { trigger, state, style, animate, transition } from '@angular/animations';

```

### imp_ts-ngfire2

`imp_ts-ngfire2` Angular import (AngularFire and FirebaseListObservable)

```ts
import { AngularFire, FirebaseListObservable } from 'angularfire2';

```


### imp_ts_components

`imp_ts_components` Angular import (components).

```ts
import { ^^^^^^^^^^ } from './components/^^^^^^^^^^.component';

```

### imp_ts_services

`imp_ts_services` Angular import (services)

```ts
import { ^^^^^^^^^^ } from './services/^^^^^^^^^^.service';

```

### exp_ts-intf

`imp_ts_interfaces` export interface.

```ts
export interface ^^^^^^^^^^ {

}

```

### imp_ts_interfaces

`imp_ts_interfaces` Angular import (interfaces)

```ts
import { ^^^^^^^^^^ } from './interfaces/^^^^^^^^^^.interface';

```

### imp_ts_pipes

`imp_ts_pipes` Angular import (pipes)

```ts
import { ^^^^^^^^^^ } from './pipes/^^^^^^^^^^.pipe';

```

### imp_ts_m

`imp_ts_m` Angular import that exports all of these modules

```ts
import { ^^^^^^^^^^ } from '../index.module';

```

### imp_ts_c

`imp_ts_c` Angular import that exports all of these components

```ts
import { ^^^^^^^^^^ } from '../index.component';

```

### imp_ts_s

`imp_ts_s` Angular import that exports all of these services

```ts
import { ^^^^^^^^^^ } from '../index.service';

```

### imp_ts-all

`imp_ts-all` Angular import (Import an entire module is contents.)

```ts
import * as ^^^^^^^^^^ from '^^^^^^^^^^';

```

### imp_ts-RxJS_map

`imp_ts-RxJS_map` import the map (operator) method is used to extract the JSON content from the response and use it then in the observable processing.

```ts
import 'rxjs/add/operator/map'; /*or ( ... rxjs/Rx ); map it to a JSON (_res.json()) */

```

### imp_ts-RxJS_Observable

`imp_ts-RxJS_Observable` import Observables.

```ts
import { Observable } from 'rxjs/Rx'; /* or ( ... rxjs/Observable ) */

```

### ngFor

`ngFor` Directive NgFor ([NgForOf](https://angular.io/api/common/NgForOf "NgForOf")): index (current loop) and first, last, even, odd (boolean value indicating whether the item)

```html
*ngFor="let ^^^^^^^^^^ of ^^^^^^^^^^; let i = index"

```

### ngIf

`ngIf` Directive [NgIf (STABLE)](https://angular.io/api/common/NgIf "NgIf (STABLE)")

```html
*ngIf="^^^^^^^^^^"

```

### ngModel

`ngModel` Directive [NgModel (STABLE)](https://angular.io/api/forms/NgModel "NgModel (STABLE)")

```html
[(ngModel)]="^^^^^^^^^^"

```

### ngStyle

`ngStyle` Directive [NgStyle](https://angular.io/api/common/NgStyle "NgStyle (STABLE)")

```html
[ngStyle]="{ \'^^^^^^^^^^\' :^^^^^^^^^^ }"

```

### ngClass

`ngClass` Directive [NgClass (STABLE)](https://angular.io/api/common/NgClass "NgClass (STABLE)")

```html
[ngClass]="{ \'^^^^^^^^^^\' :^^^^^^^^^^ }"

```

### ngSwitch

`ngSwitch` Directive [NgSwitch (STABLE)](https://angular.io/api/common/NgSwitch "NgSwitch (STABLE)")

```html
<div [ngSwitch]="^^^^^^^^^^" >
  <div *ngSwitchCase="\'^^^^^^^^^^\'" > ^^^^^^^^^^ </div>
  <div *ngSwitchCase="\'^^^^^^^^^^\'" > ^^^^^^^^^^ </div>
  <div *ngSwitchDefault > ^^^^^^^^^^ </div>
</div>

```

### ng_pfes

`ng_propty-formGroup_event-submit` [formGroup]="name of the object FormGroup" ang (ngSubmit)="var or function/method"

```html
   [formGroup]="^^^^^^^^^^" (ngSubmit)="^^^^^^^^^^"
```

### ng-FormControlName

`ng-FormControlName` [Directive FormControlName (STABLE)](https://angular.io/api/forms/FormControlName "Directive FormControlName (STABLE)")

```html
  formControlName="^^^^^^^^^^"
```

### ng-FormGroupName

`ng-FormGroupName` [FormGroupName (STABLE)](https://angular.io/api/forms/FormGroupName "FormGroupName (STABLE)")

```html
  formGroupName="^^^^^^^^^^"
```

### ng-FormArrayName

`ng-FormArrayName` [FormArrayName (STABLE)](https://angular.io/api/forms/FormArrayName "FormArrayName (STABLE)")

```html
  formArrayName="^^^^^^^^^^"
```

# Contact
More contributions and suggestions in the theme to:

* E-mail:  Freddy_ps_3@hotmail.com
* Twitter: https://twitter.com/Fred_Pizarro

Copyright © 2017-2018 [MIT License](https://github.com/ProjectsZ/ng-ts-snippets/) by Fred Pizarro.

**Enjoy!**
