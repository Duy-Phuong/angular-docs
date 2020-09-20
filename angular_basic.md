[TOC]

---

- [Angular – Giới thiệu](#angular--giới-thiệu)
  - [Cau truc thu muc](#cau-truc-thu-muc)
  - [Mục đích của từng thư mục, tập tin trong thư mục src này mình có thể liệt kê như sau:](#mục-đích-của-từng-thư-mục-tập-tin-trong-thư-mục-src-này-mình-có-thể-liệt-kê-như-sau)
  - [Setting](#setting)
  - [Cài TypeScript](#cài-typescript)
  - [Cài Angular CLI](#cài-angular-cli)
- [Typescript](#typescript)
  - [Các kiểu dữ liệu cơ bản](#các-kiểu-dữ-liệu-cơ-bản)
  - [Class](#class)
  - [Phương thức](#phương-thức)
  - [Phương thức khởi tạo](#phương-thức-khởi-tạo)
  - [Kế thừa](#kế-thừa)
  - [Fat Arrow Function](#fat-arrow-function)
- [Angular – Kiến trúc](#angular--kiến-trúc)
  - [Module](#module)
  - [Component](#component)
  - [Template](#template)
  - [Metadata](#metadata)
  - [Data Binding](#data-binding)
  - [Directive](#directive)
  - [Service](#service)
  - [Dependency injection](#dependency-injection)
- [Angular – Cấu trúc của một ứng dụng Angular](#angular--cấu-trúc-của-một-ứng-dụng-angular)
- [Angular – Root Module](#angular--root-module)
  - [Imports](#imports)
  - [Declarations](#declarations)
  - [Bootstrap](#bootstrap)
  - [Khởi động ứng dụng](#khởi-động-ứng-dụng)
- [Angular – Hiển thị dữ liệu](#angular--hiển-thị-dữ-liệu)
  - [Tạo project Angular](#tạo-project-angular)
  - [Trích xuất dữ liệu và hiển thị](#trích-xuất-dữ-liệu-và-hiển-thị)
  - [Duyệt dữ liệu với \*ngFor](#duyệt-dữ-liệu-với-ngfor)
  - [Biểu thức điều kiện](#biểu-thức-điều-kiện)
- [Angular – Tạo Component](#angular--tạo-component)
  - [Tạo component](#tạo-component)
  - [Cấu trúc của component](#cấu-trúc-của-component)
- [Angular – Xử lý sự kiện](#angular--xử-lý-sự-kiện)
  - [Bắt sự kiện](#bắt-sự-kiện)
  - [Lấy dữ liệu từ sự kiện từ đối tượng \$event](#lấy-dữ-liệu-từ-sự-kiện-từ-đối-tượng-event)
  - [Lấy dữ liệu trong template](#lấy-dữ-liệu-trong-template)
  - [Lọc sự kiện](#lọc-sự-kiện)
- [Angular – Liên kết dữ liệu với Form](#angular--liên-kết-dữ-liệu-với-form)
  - [Tạo form](#tạo-form)
  - [Liên kết dữ liệu với form](#liên-kết-dữ-liệu-với-form)
- [Angular – Theo dõi trạng thái form với ngModel](#angular--theo-dõi-trạng-thái-form-với-ngmodel)
  - [Trạng thái](#trạng-thái)
  - [Submit form](#submit-form)
- [Angular – Template – Phần 1](#angular--template--phần-1)
  - [HTML](#html)
  - [Biểu thức](#biểu-thức)
  - [Ngữ cảnh của biểu thức](#ngữ-cảnh-của-biểu-thức)
  - [Câu lệnh](#câu-lệnh)
  - [Ngữ cảnh của câu lệnh](#ngữ-cảnh-của-câu-lệnh)
  - [Cú pháp kết nối dữ liệu](#cú-pháp-kết-nối-dữ-liệu)
- [Angular – Template – Phần 2](#angular--template--phần-2)
  - [Bắt thuộc tính […]](#bắt-thuộc-tính-)
  - [Bắt sự kiện (…)](#bắt-sự-kiện-)
  - [Bắt dữ liệu 2 chiều [(…)]](#bắt-dữ-liệu-2-chiều-)
- [Angular – Template – Phần 3](#angular--template--phần-3)
  - [Biến template (#var)](#biến-template-var)
  - [Thuộc tính @Input và @Output](#thuộc-tính-input-và-output)
- [Angular – Directive – Phần 1](#angular--directive--phần-1)
  - [Attribute directive](#attribute-directive)
  - [NgClass](#ngclass)
  - [NgStyle](#ngstyle)
  - [NgModel](#ngmodel)
- [Angular – Directive – Phần 2](#angular--directive--phần-2)
  - [Structural directive](#structural-directive)
  - [ngIf](#ngif)
  - [Sử dụng template trong if else](#sử-dụng-template-trong-if-else)
  - [ngFor](#ngfor)
  - [ngSwitch](#ngswitch)
- [Angular – Service và Dependency Injection](#angular--service-và-dependency-injection)
- [Angular – Routing](#angular--routing)
  - [Tham số URL](#tham-số-url)
- [Angular – HTTP](#angular--http)
  - [Tạo web server API](#tạo-web-server-api)
  - [Truy vấn API](#truy-vấn-api)
- [Angular 4 nghiep UIT](#angular-4-nghiep-uit)
  - [Các câu lệnh thường sử dụng trong Angular CLI](#các-câu-lệnh-thường-sử-dụng-trong-angular-cli)
  - [Component](#component-1)
  - [Component to view](#component-to-view)
  - [View to Component](#view-to-component)
  - [Two way binding](#two-way-binding)
  - [Structural Directive : \*ngIf](#structural-directive--ngif)

## Angular – Giới thiệu

### Cau truc thu muc

| Tập tin / Thư mục  | Mục đích                                                                                                                      |
| ------------------ | ----------------------------------------------------------------------------------------------------------------------------- |
| e2e                | Thư mục này dùng để chứa các tập tin dành cho mục đích testing                                                                |
| node_modules       | Chứa các Node.js module cần thiết cho ứng dụng Angular của chúng ta                                                           |
| src                | Đây là thư mục sẽ chứa toàn bộ source code của ứng dụng Angular các bạn nhé                                                   |
| .editorconfig      | Chứa các cấu hình liên quan đến phần Editor để chỉnh sửa source code như: indent_size, max_line_length,…                      |
| .gitignore         | Đây là tập tin metadata của Git, chứa thông tin những tập tin hoặc thư mục sẽ bị ignore không được commit lên Git Repository. |
| angular-cli.json   | Đây là tập tin chứa cấu hình cho Angular CLI, giúp chúng ta có thể build ứng dụng Angular.                                    |
| karma.conf.js      | Tập tin cấu hình cho Karma, liên quan nhiều đến phần testing                                                                  |
| package-lock.json  | Dùng để lock version cho các Node.js module dependencies                                                                      |
| package.json       | Tập tin cấu hình cho Node.js module dependencies                                                                              |
| protractor.conf.js | Tập tin cấu hình cho Protractor, liên quan nhiều đến phần testing                                                             |
| README.md          | Tập tin này thường được sử dụng để cho các hệ thống Git hiển thị thông tin về Git Repository của chúng ta.                    |
| tslint.json        | Tập tin cấu hình để kiểm tra lỗi cho các tập tin .ts (TypeScript) trong Angular project                                       |

---

### Mục đích của từng thư mục, tập tin trong thư mục src này mình có thể liệt kê như sau:

| Tập tin / Thư mục | Mục đích                                                                                                                                                                     |
| ----------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| app               | Đây là thư mục sẽ chứa toàn bộ code của ứng dụng Angular                                                                                                                     |
| assets            | Thư mục này sẽ chứa các file ảnh, CSS, custom JavaScript của ứng dụng Angular                                                                                                |
| environments      | Chúng ta có thể viết ứng dụng chạy trên nhiều môi trường khác nhau, đây chính là thư mục giúp chúng ta làm định nghĩa các tập tin cấu hình cho những môi trường khác nhau đó |
| favicon.ico       | Icon của ứng dụng Angular                                                                                                                                                    |
| index.html        | Trang chủ của ứng dụng Angular                                                                                                                                               |
| main.ts           | Chứa code bootstrapping cho ứng dụng Angular                                                                                                                                 |
| polyfill.ts       | Dùng để định nghĩa các chuẩn để ứng dụng của chúng ta có thể chạy được trên mọi trình duyệt                                                                                  |
| style.css         | Định nghĩa style CSS cho ứng dụng Angular                                                                                                                                    |
| test.ts           | Code để chạy test                                                                                                                                                            |
| tsconfig.json     | Tập tin định nghĩa việc compile cho TypeScript                                                                                                                               |

---

https://phocode.com/javascript/lap-trinh-web-voi-angularjs-2/angular-vi-du/

### Setting

### Cài TypeScript

Sau đó bạn mở Command Prompt (cmd) trên Windows ra và gõ lệnh npm install -g typescript để node cài đặt gói typescript.

```js
C:\>npm install -g typescript

```

Ở đây phiên bản typescript của mình là phiên bản 2.1.4

### Cài Angular CLI

Bản thân Angular chỉ là một thư viện Javascript mở rộng dành cho Node.js chứ không phải một ứng dụng hoàn toàn, tuy nhiên nhóm phát triển Angular đã viết thêm gói Angular CLI là một chương trình dòng lệnh để hỗ trợ chúng ta tạo project, thêm file, xóa file, khởi động project… một cách dễ dàng.

Bạn mở Command Prompt (cmd) lên và gõ lệnh sau để cài gói Angular CLI vào npm:

```js
npm install -g @angular/cli

```

npm sẽ tải và cài bộ thư viện này về máy của bạn, bộ Angular CLI này khá lớn nên quá trình này sẽ mất một lúc.

Sau khi hoàn tất thì bạn có thể tạo một project Angular bằng cách chạy lệnh

```js
ng new my-app

```

Trong đó my-app là tên project, Angular sẽ tạo một thư mục có tên my-app và tạo một số file cần thiết, chúng ta sẽ tìm hiểu về chúng sau.

Để chạy project này thì chúng ta dùng lệnh cd để chuyển thư mục hiện hành trong CMD vào thư mục project rồi chạy lệnh sau:

```js
ng serve --open

```

Angular sẽ khởi động server tại địa chỉ http://localhost:4200

## Typescript

**TypeScript** là một ngôn ngữ có “họ hàng” với Javascript. Đây là một bản mở rộng của **ECMAScript6** (viết tắt là ES6), ES6 lại là một bản mở rộng của ECMAScript5 (viết tắt là ES5), ES5 chính là Javascript mà chúng ta thường dùng.

Ở đây chúng ta sẽ tìm hiểu nhanh qua TypeScript chứ không đi sâu.

Tuy nhiên hiện tại các trình duyệt web hiện cũng chưa hỗ trợ đầy đủ cho TypeScript nên chúng ta có thể dịch code TypeScript thành code ES5 bình thường.

Bạn có thể dùng lệnh tsc -v để xem phiên bản TypeScript của Node.

```ts
C:\>tsc -v
Version 2.1.4

```

Ở đây mình dùng phiên bản 2.1.4

Các file code TypeScript sẽ có phần mở rộng là .ts, để dịch code TypeScript thành ES5 thì chúng ta dùng lệnh tsc <tên_file>.

Ví dụ dưới đây là một đoạn code TypeScript trong file example.ts:

example.ts

```ts
class Person {
  first_name: string;
  last_name: string;
  age: number;

  constructor(first_name: string, last_name: string, age: number) {
    this.first_name = first_name;
    this.last_name = last_name;
    this.age = age;
  }

  greet() {
    console.log('Hello', this.first_name);
  }
}

var p: Person = new Person('Pho', 'Code', 23);
p.greet();
```

Dùng lệnh tsc example.ts chúng ta sẽ được một file example.js như sau:

example.js

```js
var Person = (function () {
  function Person(first_name, last_name, age) {
    this.first_name = first_name;
    this.last_name = last_name;
    this.age = age;
  }
  Person.prototype.greet = function () {
    console.log('Hello', this.first_name);
  };
  return Person;
})();
var p = new Person('Pho', 'Code', 23);
p.greet();
```

Chạy bằng node:

```js
C:\>node example.js
Hello Pho

```

### Các kiểu dữ liệu cơ bản

Các kiểu dữ liệu thường dùng là string, number, boolean, array, enum, any, void.

**String**
Đây là kiểu chuỗi kí tự.

```ts
var name: string = 'Pho Code';
```

**Number**
Đây là kiểu số, trong TypeScript thì tất cả đều là số chấm động (số thực).

```ts
var age: number = 36;
```

**Boolean**
Kiểu luận lý, hay chúng ta hay gọi là kiểu true/false.

```ts
var married: boolean = true;
```

**Array**
Kiểu mảng, khi khai báo các phần tử trong mảng thì chúng ta phải chỉ ra cả kiểu dữ liệu nữa. Để tạo array thì chúng ta có thể dùng cú pháp Array<kiểu> hoặc <kiểu>[].

```ts
var jobs: Array<string> = ['Coder', 'Tester', 'Manager'];
var primes: int[] = [2, 3, 5, 7];
```

**Enum**
Đây là kiểu danh sách, phần tử trong danh sách được đánh số theo thứ tự từ 0.

```ts
enum Role {
  Employee,
  Manager,
  Administrator,
}
var role: Role = Role.Employee;
```

**Any**
Biến kiểu Any có thể nhận bất kiểu giá trị kiểu nào.

```ts
var something: any = 'this is a string';
something = 1;
something = [1, 2, 3];
```

**Void**
Void chỉ đơn giản là “không có kiểu gì cả”, thương dùng cho các hàm không cần trả về một giá trị gì.

```ts
function setName(name: string): void {
  this.name = name;
}
```

**Object**
a : object = {}

---

### Class

Đề khai báo một lớp thì chúng ta dùng từ khóa class.

```ts
class Product {}
```

Để tạo một đối tượng thuộc một lớp thì chúng ta dùng từ khóa new.

```ts
class Product {}

var p: Product = new Product();
```

**Thuộc tính**
Thuộc tính là các dữ liệu “gắn” trong một đối tượng thuộc một lớp.

```ts
class Product {
  name: string;
  description: string;
  price: number;
}
```

### Phương thức

Phương thức là các hàm của riêng một đối tượng.

```ts
class Product {
  name: string;
  description: string;
  price: number;

  getName(): string {
    return this.name;
  }

  setName(name) {
    this.name = name;
  }

  getDescription(): string {
    return this.description;
  }

  setDescription(description) {
    this.description = description;
  }

  getPrice(): number {
    return this.price;
  }

  setPrice(price) {
    this.price = price;
  }
}
```

### Phương thức khởi tạo

Phương thức khởi tạo là phương thức sẽ được gọi khi chúng ta tạo một đối tượng bằng từ khóa new. Trong TypeScript thì phương thức khởi tạo luôn có tên là constructor(), có thể nhận vào tham số nhưng không thể có giá trị trả về.

Nếu bạn không khai báo phương thức khởi tạo thì TypeScript cũng tự định nghĩa một phương thức khởi tạo riêng (nhưng chúng ta không nhìn thấy).

```ts
class Product {
  constructor() {
    console.log('Product has been created');
  }
}
var p: Product = new Product();
```

Trong TypeScript thì chúng ta **chỉ được phép khai báo một phương thức khởi tạo duy nhất cho một lớp**, do đó thông thường chúng ta sẽ khai báo phương thức khởi tạo nhận vào tham số là toàn bộ thuộc tính của lớp đó.

```ts
class Product {
  name: string;
  description: string;
  price: number;

  constructor(name: string, description: string, price: number) {
    this.name = name;
    this.description = description;
    this.price = price;
  }
}
var p: Product = new Product(
  'Angular 2',
  'Web Development with Angular 2',
  59.99
);
```

### Kế thừa

Kế thừa là một trong những tính năng quan trọng của lập trình hướng đối tượng, cho phép coder tái sử dụng code.

Để một lớp kế thừa từ lớp khác thì chúng ta chỉ cần dùng từ khóa extends.

```ts
class Product {
  name: string;
  description: string;
  price: number;

  getName(): string {
    return this.name;
  }

  setName(name) {
    this.name = name;
  }

  getDescription(): string {
    return this.description;
  }

  setDescription(description) {
    this.description = description;
  }

  getPrice(): number {
    return this.price;
  }

  setPrice(price) {
    this.price = price;
  }

  constructor(name: string, description: string, price: number) {
    this.name = name;
    this.description = description;
    this.price = price;
  }
}

class Book extends Product {}
var b: Book = new Book('Angular 2', 'Web development with Angular 2', 59.99);
console.log(b.getName(), b.getDescription(), b.getPrice());
```

Lớp kế thừa có thể sử dụng các thuộc tính và phương thức của lớp cha, và có thể có thuộc tính và phương thức của riêng nó.

### Fat Arrow Function

Mình không biết gọi là gì, trong TypeScript bạn có thể dùng từ khóa => để tạo nhanh một hàm thay vì phải viết từ khóa function như trong ES5.

```ts
ES5: var product = ['Apple', 'Lemon', 'Banana'];
product.forEach(function (p) {
  console.log(p);
});

TypeScript: var product = ['Apple', 'Lemon', 'Banana'];
product.forEach((p) => console.log(p));
```

Thao tác trên string
Chúng ta có thể chèn giá trị của một biến vào một string bằng cách dùng kí tự '\$'.

```ts
var title = 'Angular 2';
var price = 59.99;
var str = `${title} costs ${price}`;
console.log(str);
```

Lưu ý là bạn phải dùng dấu huyền ` để bọc chuỗi chứ không dùng dấu nháy đơn hay nháy kép gì cả.

Khi bọc chuỗi trong cặp dấu huyền ` thì chúng ta có thể viết chuỗi trên nhiều dòng.

```js
var html = `
<html>
    <head>
        <title>Pho Code</title>
    </head>
<body>
</body>
</html>
`;
```

---

## Angular – Kiến trúc

Một ứng dụng Angular được xây dựng từ 8 thành phần sau đây: **Module, Component, Template, Metadata, Data Binding, Directive, Service, Dependency Injection.**

### Module

Mỗi ứng dụng Angular được gọi là một module và bản thân Angular có riêng một module dùng để quản lý các module khác có tên là Root Module hay NgModule. Root Module thường được đặt tên là AppModule, ngoài root ra thì tùy ứng dụng mà sẽ có thêm các module khác, chúng ta sẽ tìm hiểu về root module trong bài sau.

Chúng ta khai báo một module bằng cách dùng từ khóa @NgModule. Các từ khóa như @NgModule này là các hàm dùng để chỉnh sửa các lớp của Javascript. Bên trong từ khóa @NgModule chúng ta khai báo các tham số sau đây:

- **declarations**: tên lớp view thuộc về module này
- **exports**: danh sách tên các module hoặc component có thể sử dụng module này
- **imports**: tên các module sẽ được dùng từ module này
- **providers**: tên các service sẽ được dùng từ module này, chúng ta sẽ tìm hiểu về service sau
- **bootstrap**: tên lớp view dành cho root module, chỉ có root module mới thiết lập tham số này. Noi component dau tien chay len
  Đây là một đoạn code module trong file có tên app.module.ts đơn giản như sau:

```ts
import { NgModule } from '@angular/core';
import { BrowserModule } from '@angular/platform-browser';
@NgModule({
  imports: [BrowserModule],
  providers: [Logger],
  declarations: [AppComponent],
  exports: [AppComponent],
  bootstrap: [AppComponent],
})
export class AppModule {}
```

Để gọi module trên thì chúng ta code như sau:

```ts
import { platformBrowserDynamic } from '@angular/platform-browser-dynamic';
import { AppModule } from './app.module';

platformBrowserDynamic().bootstrapModule(AppModule);
```

### Component

Component có chức năng điều khiển việc hiển thị, tức là điều khiển View, vậy bạn có thể hình dung Component chính là một Controller trong mô hình MVC…v.v Ví dụ một đoạn code component:

```ts
export class HeroListComponent implements OnInit {
  heroes: Hero[];
  selectedHero: Hero;

  constructor(private service: HeroService) {}

  ngOnInit() {
    this.heroes = this.service.getHeroes();
  }

  selectHero(hero: Hero) {
    this.selectedHero = hero;
  }
}
```

### Template

Template là một đoạn code HTML để component dựa vào đó mà hiển thị trên màn hình. Ví dụ:

```html
<h2>Hero List</h2>
<p><i>Pick a hero from the list</i></p>
<ul>
  <li *ngFor="let hero of heroes" (click)="selectHero(hero)">
    {{hero.name}}
  </li>
</ul>
<hero-detail *ngIf="selectedHero" [hero]="selectedHero"></hero-detail>
```

Ngoài các thẻ HTML thông thường như <h2>, <p> thì còn có những thẻ và thuộc tính đặc biệt như \*ngFor, {{hero.name}}, (click), [hero] và <hero-detail>, đây là cú pháp template của Angular.

### Metadata

Metadata (siêu dữ liệu) là những thông tin giúp Angular xử lý các lớp.

Trong đoạn code ví dụ về Component ở trên, đó chỉ là một lớp bình thường viết bằng TypeScript, không có sự xuất hiện của Angular trong này. Muốn Angular hiểu được đó là một lớp dành cho Angular thì chúng ta phải khai báo metadata. Ví dụ:

```ts
@Component({
  moduleId: module.id,
  selector: 'hero-list',
  templateUrl: 'hero-list.component.html',
  providers: [HeroService],
})
export class HeroListComponent implements OnInit {
  /* . . . */
}
```

Trong đó @Component là từ khóa bắt đầu định nghĩa metadata, phần định nghĩa lớp ngay sau phần metadata này là lớp component của metadata trên. Bên trong chúng ta khai báo một số thông tin cho Angular như moduleId, selector, templateUrl, providers. Chúng ta sẽ tìm hiểu về chúng sau.

### Data Binding

Data Binding tức là lấy dữ liệu từ model/controller đổ vào view. Trong đoạn code ví dụ về template trên có những dòng data binding như sau:

```html
<li>{{hero.name}}</li>
<hero-detail [hero]="selectedHero"></hero-detail>
<li (click)="selectHero(hero)"></li>
```

Data binding trong Angular là 2 chiều, tức là chúng ta có thể nhập dữ liệu từ view vào model/controller.

```html
<input [(ngModel)]="hero.name" />
```

### Directive

Directive (chỉ thị) là một lớp và có phần khai báo metadata là @Directive. Thường thì directive sẽ nằm trong một element – hay thẻ của HTML giống như một thuộc tính bình thường.

Có 2 loại directive là **structural và attribute**.

- Các structural directive có chức năng gán dữ liệu theo một quy tắc nào đó.

```html
<li *ngFor="let cus of customer"></li>
<customer *ngIf="selectedCustomer"></customer>
```

Trong đoạn code trên thì *ngFor và *ngIf là các structural directive.

- Các attribute directive có chức năng hiển thị dữ liệu một cách trực tiếp.

```html
<input [(ngModel)]="hero.name" />
```

Trong đoạn code trên thì ngModel là một attribute directive.

### Service

Service là các lớp có khả năng thực hiện một số chức năng thường dùng, nói đơn giản thì chúng giống như thư viện vậy. Một số service phổ biến là: logging service, data service, message bus, tax calculator, application configuration.

Ví dụ lớp Logger cho phép chúng ta in các đoạn code báo lỗi, cảnh báo…v.v:

```ts
export class Logger {
  log(msg: any) {
    console.log(msg);
  }
  error(msg: any) {
    console.error(msg);
  }
  warn(msg: any) {
    console.warn(msg);
  }
}
```

### Dependency injection

Dependency là các lớp/module/service được dùng thêm, Dependency injection là khả năng cho phép tạo các đối tượng lớp có đầy đủ các lớp/module/service được dùng thêm đó. Chẳng hạn như chúng ta có phương thức constructor() như sau:

```ts
constructor(private service: HeroService) { }

```

Tham số private service: HeroService có nghĩa là lớp này cần dùng một service có tên HeroService.

Angular có riêng một vùng bộ nhớ để lưu trữ các dependency đã được gọi, khi một module/component nào cần dùng service nào, Angular sẽ tìm trong vùng bộ nhớ đó xem có không, nếu không có thì Angular sẽ tạo một đối tượng của dependency đó và đưa vào bộ nhớ rồi trả về cho lớp đã gọi.

Khi chúng ta xây dựng root module thì chúng ta phải khai báo các dependency trong tham số providers, có như thế Angular mới có thể tìm được.

```ts
providers: [
    BackendService,
    HeroService,
    Logger
],

```

Hoặc khai báo ở phần @Component:

```ts
@Component({
    moduleId: module.id,
    selector: 'hero-list',
    templateUrl: 'hero-list.component.html',
    providers: [ HeroService ]
})

```

---

## Angular – Cấu trúc của một ứng dụng Angular

Trong thư mục quickstart mà chúng ta đã cài đặt Angular, có một thư mục project mẫu tên là app, trong thư mục này có 3 file .ts như sau:

```js
app/
|---app.component.ts
|---app.module.ts
|---app.ts

```

Tất cả các project nào cũng phải có 3 file này, mỗi file thực hiện một mục đích khác nhau, tùy theo ứng dụng mà chúng sẽ phát triển như thế nào.

app.component.ts

```js
import { Component } from '@angular/core';

@Component({
  selector: 'my-app',
  template: `<h1>Hello {{ name }}</h1>`,
})
export class AppComponent {
  name = 'Angular';
}
```

File app.component.ts định nghĩa lớp AppComponent, đây là một component nhờ có phần khai báo metadata @Component, đây còn được gọi là **root component**, tất cả các component mà chúng ta sẽ viết đều được kế thừa từ component này.

app.module.ts

```js
import { NgModule } from '@angular/core';
import { BrowserModule } from '@angular/platform-browser';
import { AppComponent } from './app.component';

@NgModule({
  imports: [BrowserModule],
  declarations: [AppComponent],
  bootstrap: [AppComponent],
})
export class AppModule {}
```

File app.module.ts định nghĩa lớp AppModule, đây là một module nhờ có phần khai báo metadata @NgModule, đây còn gọi là Root Module vì có khai báo thuộc tính bootstrap, mục đích của root module là cho Angular biết cách ứng dụng chạy như thế nào.

main.ts

```js
import { NgModule } from '@angular/core';
import { BrowserModule } from '@angular/platform-browser';
import { AppComponent } from './app.component';

@NgModule({
  imports: [BrowserModule],
  declarations: [AppComponent],
  bootstrap: [AppComponent],
})
export class AppModule {}
```

File main.ts sẽ liên kết toàn bộ các file thành một ứng dụng hoàn chỉnh.

---

## Angular – Root Module

Các lớp module có trách nhiệm gắn kết các thành phần lại với nhau, mỗi ứng dụng Angular sẽ có ít nhất một module, trong đó có một module gốc (root) luôn được chạy trước tiên khi chúng ta khởi động ứng dụng, thông thường chúng ta sẽ đặt tên nó là AppModule.

Trong thư mục quickstart/src mà chúng ta đã cài đặt cũng có một file như vậy tên là app.module.ts:

src/app.module.ts

```ts
import { NgModule } from '@angular/core';
import { BrowserModule } from '@angular/platform-browser';
import { AppComponent } from './app.component';

@NgModule({
  imports: [BrowserModule],
  declarations: [AppComponent],
  bootstrap: [AppComponent],
})
export class AppModule {}
```

Trong đoạn code trên, ba dòng đầu tiên là các dòng import thư viện, kế đến là đoạn khai báo clas AppModule, với phần khai báo decorator @NgModule.

Từ khóa @NgModule báo cho Angular biết đây là một class module trong Angular. Các tham số trong phần khai báo @NgModule giúp Angular biết cách dịch và chạy ứng dụng như thế nào, trong đó:

- **imports**: đây là một mảng dùng để khai báo tên các module khác sẽ được dùng bởi module này, ở đoạn code trên chúng ta chỉ khai báo 1 module là BrowserModule.

- **declarations**: đây cũng là một mảng chứa tên các lớp thuộc về module này.

- **bootstrap**: tên lớp View sẽ được dùng để hiển thị lên màn hình đầu tiên, chỉ có AppModule (hay root module) mới khai báo tham số này.

  Chúng ta sẽ lần lượt tìm hiểu 3 tham số trên.

### Imports

Module là tính năng cho phép Angular tách các thành phần có chung quan hệ với nhau thành các đơn vị độc lập. Rất nhiều tính năng trong Angular được tổ chức thành các module. Chẳng hạn như dịch vụ HTTP trong Angular được gói thành HttpModule. Tính năng router thì ở trong RouterModule. Chúng ta cũng có thể viết module riêng.

Để thêm một module vào thì chúng ta khai báo trong mảng imports.

Angular là một web framework, ứng dụng sẽ được chạy trên trình duyệt web, do đó sẽ cần dùng đến BrowserModule trong AppModule. BrowserModule nằm trong thư mục angular/platform-browser.

Chỉ có các lớp NgModule mới được khai báo trong mảng imports.

### Declarations

Chúng ta khai báo cho Angular biết các lớp component thuộc về AppModule trong mảng declarations, bất cứ khi nào chúng ta tạo ra một component mới thì chúng ta khai báo trong mảng này.

Ngoài ra bất cứ một component nào được tạo ra cũng phải được khai báo trong một lớp NgModule nào đó, nếu không Angular sẽ báo lỗi.

Chúng ta sẽ tìm hiểu về 2 loại lớp là directive và pipe trong các bài sau, các lớp loại này thường được khai báo trong mảng declarations.

_Chỉ có 3 loại lớp có thể khai báo trong mảng declarations là component, directive và pipe._

### Bootstrap

Ứng dụng được khởi động thông qua lớp AppModule. Khi khởi động Angular sẽ tạo ra các đối tượng được khai báo trong mảng bootstrap và lưu vào trình duyệt.

Mỗi đối tượng được tạo ra đó sẽ nằm riêng biệt với nhau, thông thường trong các lớp được khai báo sẽ tạo thêm các đối tượng con tùy vào coder.

Nhưng thông thường thì chúng ta chỉ khai báo một lớp trong mảng bootstrap thôi, và thường thì chúng ta đặt tên là AppComponent.

### Khởi động ứng dụng

Có rất nhiều cách để khởi động ứng dụng.

Cách thông dụng nhất là chúng ta code đoạn code khởi động AppModule trong một file .ts riêng và đặt trong thư mục có tên src, ví dụ như sau:

src/main.ts

```ts
import { platformBrowserDynamic } from '@angular/platform-browser-dynamic';

import { AppModule } from './app/app.module';

platformBrowserDynamic().bootstrapModule(AppModule);
```

Chúng ta khởi động bằng cách gọi phương thức platformBrowserDynamic().bootstrapModule(), truyền vào tham số là lớp AppModule.

---

## Angular – Hiển thị dữ liệu

### Tạo project Angular

Chúng ta tạo một project bằng cách lấy bộ code mẫu từ trang Github của Angular về như trong bài Cài đặt đã hướng dẫn, đầu tiên bạn mở Command Prompt (cmd) lên, sau đó gõ lệnh sau:

```ts
C:\Project>git clone https://github.com/angular/quickstart.git displaying_data

```

Lệnh trên sẽ yêu cầu git tạo một thư mục với tên displaying_data, sau đó lấy bộ code từ project quickstart về từ trang Github của Angular.

Sau đó bạn gõ các lệnh sau:

```ts

C:\Project>cd displaying_data
...
C:\Project\displaying_data>npm install
...

```

Lệnh cd displaying_data sẽ di chuyển thư mục hiện tại trong Command Prompt vào thư mục displaying_data, sau đó lệnh npm install sẽ tải và cài các module cần thiết từ hệ thống npm về.

Vậy là chúng ta tạo project xong.

Lưu ý là trong thư mục này có rất nhiều file không cần thiết, chúng ta có thể xóa chúng đi bằng cách chạy 3 lệnh sau:

```ts
C:\Project\displaying_data>for /f %i in (non-essential-files.txt) do del %i /F /S /Q
...
C:\Project\displaying_data>rd .git /s /q
...
C:\Project\displaying_data>rd e2e /s /q
...

```

### Trích xuất dữ liệu và hiển thị

Ở đây chúng ta sẽ khai báo biến trong lớp component và hiển thị lên màn hình.

Chúng ta sửa lại file app.component.ts trong thư mục src\app như sau:

src/app/app.component.ts

```ts
import { Component } from '@angular/core';

@Component({
  selector: 'my-app',
  template: `
    <h1>{{ title }}</h1>
    <h2>
      My favorite idol is: {{ myIdol }}
      <h2></h2>
    </h2>
  `,
})
export class AppComponent {
  title = 'My idol list';
  myIdol = 'Steve Jobs';
}
```

Trong file này chúng ta định nghĩa một lớp Component là AppComponent, lớp này có 2 thuộc tính là title và myIdol.

```ts
template: `        
          <h1>{{ title }}</h1>
          <h2>My favorite idol is: {{ myIdol }}
          <h2>
          `;
```

Tham số template trong phần khai báo @Component là đoạn code HTML sẽ được hiển thị lên màn hình, ở đây chúng ta hiển thị dữ liệu của 2 thuộc tính title và myIdol.

_Lưu ý: các biến sẽ được bọc trong cặp dấu ngoặc nhọn {{}}. Chuỗi được bọc trong dấu huyền `` có thể ghi trên nhiều dòng._

Sau đó bạn có thể chạy lệnh npm start để chạy project rồi.

> C:\Project\displaying-data>npm start

> angular-quickstart@1.0.0 prestart C:\Project\displaying-data
> npm run build

> angular-quickstart@1.0.0 build C:\Project\displaying-data>
> tsc -p src/

> angular-quickstart@1.0.0 start C:\Project\displaying-data>
> concurrently "npm run build:watch" "npm run serve"
> ...

Ở đây chúng ta không làm công việc gì như tạo đối tượng cả, Angular sẽ tạo giùm cho chúng ta. Tham số selector trong phần khai báo @Component ở trên định nghĩa tên thẻ sẽ được gọi trong file HTML, ở đây đã được đặt sẵn là my-app, trong file src\index.html có sẵn đoạn code tạo thẻ <my-app></my-app> để tham chiếu đến component này rồi.

Khi chúng ta chạy lệnh npm start, npm sẽ khởi động project từ file main.ts, đoạn code trong này sẽ tạo đối tượng từ lớp AppModule trong file app.module.ts, trong lớp AppModule này lại tham chiếu đến lớp AppComponent mà chúng ta vừa sửa ở trên.

### Duyệt dữ liệu với \*ngFor

Chúng ta dùng chỉ thị \*ngFor để thực hiện việc duyệt các kiểu dữ liệu danh sách (như mảng). Ví dụ chúng ta sửa lại file app.component.ts như sau:

src/app/app.component.ts

```ts
import { Component } from '@angular/core';

@Component({
  selector: 'my-app',
  template: `
    <h1>{{ title }}</h1>
    <h2>My favorite idol is: {{ myIdol }}</h2>
    There are some more:
    <ul>
      <li *ngFor="let idol of idols">
        {{ idol }}
      </li>
    </ul>
  `,
})
export class AppComponent {
  title = 'My idol list';
  idols = ['Steve Jobs', 'Bill Gates', 'Mark Zuckerberg', 'Linus Torvalds'];
  myIdol = this.idols[0];
}
```

Trong lớp AppComponent chúng ta có một mảng là idols, thuộc tính myIdol là giá trị của phần tử đầu tiên trong mảng.

Trong tham số template, chúng ta duyệt mảng idols và hiển thị trong thẻ <ul></ul>. Ở đây chúng ta dùng thuộc tính \*ngFor="let idol of idols" để thực hiện việc duyệt mảng.

### Biểu thức điều kiện

Chúng ta dùng chỉ thị \*ngIf để thực hiện biểu thức điều kiến, ví dụ chúng ta sửa lại đoạn code app.component.ts như sau:

src/app/app.component.ts

```ts
import { Component } from '@angular/core';

@Component({
  selector: 'my-app',
  template: `
    <h1>{{ title }}</h1>
    <h2>My favorite idol is: {{ myIdol }}</h2>
    <p *ngIf="idols.length > 1">There are some more:</p>
    <ul>
      <li *ngFor="let idol of idols">
        {{ idol }}
      </li>
    </ul>
  `,
})
export class AppComponent {
  title = 'My idol list';
  idols = ['Steve Jobs', 'Bill Gates', 'Mark Zuckerberg', 'Linus Torvalds'];
  myIdol = this.idols[0];
}
```

Theo sau \*ngIf là một câu lệnh so sánh hay bất cứ một biểu thức là mà có trả về giá trị true hoặc false, nếu true thì chuỗi trong cặp thẻ <p></p> mới được hiển thị.

---

## Angular – Tạo Component

Trong phần này chúng ta sẽ tìm hiểu cách tạo một Component.

### Tạo component

Chúng ta đã biết Component là một lớp và có phần khai báo @Component ở trước phần định nghĩa lớp đó, khi tạo một project Angular thì một module có thể có nhiều component dùng hiển thị các chức năng khác nhau.

Bây giờ chúng ta tạo một file có tên new.component.ts trong thư mục src/app với nội dung như sau:

src/app/my.component.ts

```ts
import { Component } from '@angular/core';

@Component({
  selector: 'my-component',
  template: ` <h2>Testing</h2> `,
})
export class MyComponent {}
```

Đây là một lớp component bình thường như bao lớp khác, ở đây chúng ta đặt tên selector là my-component. Lưu ý thường chúng ta đặt tên file có đuôi là \*.component.ts cho dễ quản lý.

Để sử dụng component mới này thì chúng ta chỉ cần gọi selector của lớp đó trong template của lớp AppComponent là được, chúng ta sửa lại file app.component.ts như sau:

src/app/app.component.ts

```ts
import { Component } from '@angular/core';
import { MyComponent } from './my.component';

@Component({
  selector: 'my-app',
  template: `
    <h1>Testing npm</h1>
    <my-component>Loading</my-component>
  `,
})
export class AppComponent {
  name = 'Angular';
}
```

Trong tham số template, chúng ta chỉ cần khai báo thêm selector của lớp MyComponent là `<my-component></my-component>`, giữa 2 thẻ này có thể để trống.

Ở đầu file chúng ta phải import lớp MyComponent, nếu không Angular sẽ báo lỗi.

Cuối cùng chúng ta phải **khai báo lớp MyComponent này trong AppModule** nữa thì mới hiển thị được, chúng ta sửa lại file app.module.ts như sau:

src/app/app.module.ts

```ts
import { NgModule } from '@angular/core';
import { BrowserModule } from '@angular/platform-browser';

import { AppComponent } from './app.component';
import { MyComponent } from './my.component';

@NgModule({
  imports: [BrowserModule],
  declarations: [AppComponent, MyComponent],
  bootstrap: [AppComponent],
})
export class AppModule {}
```

Chúng ta chỉ cần thêm dòng import và khai báo trong mảng **declarations** là xong.

### Cấu trúc của component

new-cmp.component.ts

```ts
import { Component, OnInit } from '@angular/core'; // Khai báo import angular/core

@Component({
  // Khai báo selector cho component new-cmp
  selector: 'app-new-cmp', //
  templateUrl: './new-cmp.component.html',
  // Khai báo file html mà component new-cmp "đại diện"
  styleUrls: ['./new-cmp.component.css'], // Khai báo file style sử dụng
})
export class NewCmpComponent implements OnInit {
  constructor() {}
  ngOnInit() {}
}
```

Ở đây khai báo 1 class gọi là NewCmpComponent. Class này implements class OnInit. Class OnInit có constructor là ngOnInit(), nên trong NewCmpComponent cũng sẽ override lại constructor ngOnInit() này. Constructor ngOnInit() sẽ được gọi mặc định khi class được gọi đến.
https://freetuts.net/tim-hieu-ve-component-trong-angular-4-1301.html

---

## Angular – Xử lý sự kiện

Khi người dùng tương tác với trang web thì sẽ phát sinh sự kiện, những sự kiện thường thấy nhất là click chuột, gõ phím, tải trang web…v.v Đây là các sự kiện DOM (DOM Event), chúng ta có thể lắng nghe các sự kiện đó và tương tác lại với người dùng.

### Bắt sự kiện

Trong Javascript ES5 thì chúng ta viết code bắt sự kiện như sau:

```ts
<button onclick="onClick()">
```

Còn trong TypeScript thì chúng ta viết đoạn code bắt sự kiện như sau:

```ts
<button (click)="onClick()">

```

Trong đó (click) là tên sự kiện, ở đây là sự kiện thả click chuột, onClick() là tên phương thức sẽ xử lý sự kiện đó, phương thức này chúng ta viết trong các lớp Component.

Ví dụ, bạn tạo một project mới từ quickstart, sau đó sửa trong file app.component.ts như sau:

src/app/app.component.ts

```ts
import { Component } from '@angular/core';

@Component({
  selector: 'my-app',
  template: `
    <button (click)="onClick()">Click here</button>
    {{ message }}
  `,
})
export class AppComponent {
  message = '';

  onClick() {
    this.message = 'Clicked';
  }
}
```

Rất đơn giản, chúng ta khai báo trong lớp AppComponent một thuộc tính là message, và khi click thì phương thức onClick() sẽ được gọi, trong đó chúng ta gán thuộc tính message giá trị là “Clicked”. Giá trị của thuộc tính này sẽ được hiển thị trên template.

### Lấy dữ liệu từ sự kiện từ đối tượng \$event

Có một số sự kiện sẽ mang theo cả dữ liệu, chẳng hạn như click chuột thì có thể lấy được tọa độ chuột, bấm phím thì lấy được kí tự phím vừa bấm… v.v Chúng ta có thể lấy được các dữ liệu đó.

Ví dụ chúng ta sửa lại lớp AppComponent như sau:

src/app/app.component.ts

```ts
import { Component } from '@angular/core';

@Component({
  selector: 'my-app',
  template: `
    Type here: <input (keyup)="onKey($event)" />
    <p>You typed: {{ values }}</p>
  `,
})
export class AppComponent {
  values = '';
  onKey(event: any) {
    this.values = event.target.value;
  }
}
```

Ở đây chúng ta khai báo template là một the `<input>`, với sự kiện keyup xử lý bằng phương thức onKey(). Dữ liệu sẽ được truyền vào tham số \$event.

Khi người dùng nhấn và thả một phím, sự kiễn keyup sẽ xảy ra, Angular sẽ truyền đối tượng sự kiện DOM là biến \$event vào làm tham số của phương thức onKey().

Tùy vào sự kiện là gì mà đối tượng \$event sẽ có những thông tin khác nhau.

Tất cả các đối tượng sự kiện DOM đều có một thuộc tính là target, thuộc tính này tham chiếu đến thẻ đã phát sinh ra sự kiện đó, ở đây là `<input>`, và chúng ta có thể lấy thuộc tính value của thẻ này để lấy nội dung của thẻ.

Trong phương thức onKey() ở đây chúng ta gán giá trị cho biến values là giá trị trong event.target.value.

Trong đoạn code trên chúng ta khai báo kiểu dữ liệu của \$event là any, tức là Angular sẽ tự động chuyển đổi sang kiểu dữ liệu DOM thích hợp, việc code như thế sẽ đơn giản và tránh các lỗi ngớ ngẩn.

Chúng ta có thể chỉ rõ ra kiểu dữ liệu như sau:

src/app/app.component.ts

```ts
export class AppComponent {
  values = '';
  onKey(event: KeyboardEvent) {
    this.values = (<HTMLInputElement>event.target).value;
  }
}
```

Ở đây chúng ta chỉ rõ kiểu dữ liệu của \$event là KeyboardEvent, tức là sự kiện từ bàn phím. Bạn có thể xem danh sách các kiểu dữ liệu sự kiện DOM ở đây.
https://developer.mozilla.org/en-US/docs/Web/API/Event

### Lấy dữ liệu trong template

Thay vì khai báo phương thức cho sự kiện, chúng ta có thể tham chiếu đến dữ liệu của sự kiện đó ngay trong template như sau:

src/app/app.component.ts

```ts
import { Component } from '@angular/core';

@Component({
  selector: 'my-app',
  template: `
    Type here: <input #box (keyup)="(0)" />
    <p>You typed: {{ box.value }}</p>
  `,
})
export class AppComponent {}
```

Để làm việc này thì chúng ta khai báo tên biến cho template, bằng cách ghi tên kèm với dấu #, ở đây chúng ta khai báo là #box. Ở phần bắt sự kiện chúng ta điền vào là 0, và chúng ta có thể dùng tên biến template đó để lấy giá trị của chính thẻ đó mà không cần phải dùng tới phương thức.

### Lọc sự kiện

Đôi khi chúng ta chỉ cần muốn bắt một giá trị cụ thể, chẳng hạn như phím Enter, chúng ta có thể bắt giá trị đó thông qua thuộc tính \$event.keyCode. Ví dụ:

src/app/app.component.ts

```ts
import { Component } from '@angular/core';

@Component({
  selector: 'my-app',
  template: `
    Type here: <input #box (keyup.enter)="onEnter(box.value)" />
    <p>You typed: {{ value }}</p>
  `,
})
export class AppComponent {
  value = '';
  onEnter(value: string) {
    this.value = value;
  }
}
```

Ở đây sự kiện sẽ xảy ra khi người dùng gõ phím Enter, chúng ta truyền vào giá trị của #box.value rồi gán giá trị đó vào biến value để hiển thị.

---

## Angular – Liên kết dữ liệu với Form

Angular cho phép chúng ta kết nối dữ liệu từ form tới các đối tượng trong class.

### Tạo form

Để ví dụ thì đầu tiên chúng ta sẽ tạo một form trước đã, ở đây chúng ta sẽ tạo form điền những thông tin thông thường của mô hình khách hàng.

Đầu tiên chúng ta tạo một project mới lấy từ quickstart, đặt tên là gì cũng được, form chẳng hạn.

Sau đó trong thư mục src/app, chúng ta tạo một file có tên customer.ts như sau:

src/app/customer.ts

```ts
export class Customer {
  constructor(
    public id: number,
    public name: string,
    public age: number,
    public job: string
  ) {}
}
```

Lớp Customer chỉ có một phương thức khởi tạo là constructor() và vài thuộc tính đơn giản.

Tiếp theo chúng ta tạo file customer-form.component.ts trong thư mục src/app như sau:

src/app/customer-form.component.ts

```ts
import { Component } from '@angular/core';
import { Customer } from './customer';

@Component({
  moduleId: module.id,
  selector: 'customer',
  templateUrl: './customer-form.component.html',
})
export class CustomerFormComponent {
  jobList = [
    'Software Developer',
    'Tester',
    'Project Manager',
    'Business Analyst',
  ];
  customer1 = new Customer(1, 'Pho Coder', 24, this.jobList[0]);
}
```

Ở đây chúng ta định nghĩa lớp component là CustomerFormComponent, lớp này có selector là customer, template lấy từ file khác là customer-form.component.html (chúng ta sẽ viết sau) chứ không code trực tiếp ở đây nữa, để có thể tham chiếu đến file template theo đường dẫn tương đối thì chúng ta phải khai báo tham số moduleId là module.id.

Ngoài ra ở đây chúng ta còn import lớp Customer đã định nghĩa ở trên, tạo một mảng jobList lưu danh sách nghề nghiệp, rồi tạo một đối tượng Customer là customer1 với các giá trị đơn giản, trong đó thuộc tính job lấy từ mảng jobList.

Bây giờ chúng ta tạo file template customer-form.component.html cùng thư mục src/app như sau:

src/app/customer-form.component.html

```html
<div class="container">
  <h1>Customer</h1>
  <form>
    <div class="form-group">
      <label for="name">Name</label>
      <input type="text" class="form-control" id="name" required />
    </div>

    <div class="form-group">
      <label for="age">Age</label>
      <input type="text" class="form-control" id="name" required />
    </div>

    <div class="form-group">
      <label for="job">Job</label>
      <select class="form-control" id="job" required>
        <option *ngFor="let job of jobList" [value]="job">{{job}}</option>
      </select>
    </div>

    <button type="submit" class="btn btn-success">Submit</button>
  </form>
</div>
```

Chúng ta dùng form để hiển thị các trường text, button, combobox…v.v

Ở trường dành cho jobList, chúng ta dùng chỉ thị *ngFor để lặp mảng jobList trong lớp CustomerFormComponent, rồi lấy từng phần tử mảng đó ra làm các item cho thẻ `<select>`. Cú pháp của *ngFor cũng khá đơn giản, bạn có thể tự suy ra cú pháp là:

```ts
let <tên_biến_lặp> of <tên_mảng>

```

Rồi lấy giá trị thông qua <tên_biến_lặp>.

Ngoài ở nếu bạn để ý thì ở đây chúng ta dùng các lớp CSS của thư viện Bootstrap để làm “màu mè” cho form.

Do đó bây giờ chúng ta chèn thêm đoạn code sử dụng Bootstrap vào file index.html ở trong thư mục src như sau:

src/index.html

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Angular QuickStart</title>
    <base href="/" />
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <link rel="stylesheet" href="styles.css" />

    <link
      rel="stylesheet"
      href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css"
    />
    <link
      rel="stylesheet"
      href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap-theme.min.css"
    />
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>

    <!-- Polyfill(s) for older browsers -->
    <script src="node_modules/core-js/client/shim.min.js"></script>

    <script src="node_modules/zone.js/dist/zone.js"></script>
    <script src="node_modules/systemjs/dist/system.src.js"></script>

    <script src="systemjs.config.js"></script>
    <script>
      System.import('main.js').catch(function (err) {
        console.error(err);
      });
    </script>
  </head>

  <body>
    <my-app>Loading AppComponent content here ...</my-app>
  </body>
</html>
```

Bây giờ chúng ta khai báo form này trong lớp AppComponent, chúng ta sửa file app.component.ts trong thư mục src/app như sau:

src/app/app.component.ts

```ts
import { Component } from '@angular/core';
import { CustomerFormComponent } from './customer-form.component';

@Component({
  selector: 'my-app',
  template: ` <customer></customer> `,
})
export class AppComponent {}
```

Cuối cùng chúng ta khai báo lớp **CustomerFormComponent** trong lớp AppModule, chúng ta sửa flle app.module.ts trong thư mục src/app như sau:

src/app/app.module.ts

```ts
import { NgModule } from '@angular/core';
import { BrowserModule } from '@angular/platform-browser';
import { FormsModule } from '@angular/forms';

import { AppComponent } from './app.component';
import { CustomerFormComponent } from './customer-form.component';

@NgModule({
  imports: [BrowserModule, FormsModule],
  declarations: [AppComponent, CustomerFormComponent],
  bootstrap: [AppComponent],
})
export class AppModule {}
```

Ở đây chúng ta còn import thêm một module nữa là **FormsModule**, module này hỗ trợ một số tính năng để kết nối dữ liệu giữa template và class.

Bây giờ chúng ta có thể chạy project và trang web sẽ có giao diện form như thế này:

### Liên kết dữ liệu với form

Chúng ta có thể liên kết các trường trong form với một thuộc tính nào đó trong lớp component tương ứng.

Để làm việc đó thì chúng ta sửa lại file template customer-form.component.html như sau:

src/app/customer-form.component.html

```html
<div class="container">
  <h1>Customer</h1>
  <form>
    <div class="form-group">
      <label for="name">Name</label>
      <input
        type="text"
        class="form-control"
        id="name"
        [(ngModel)]="customer1.name"
        name="cus1_name"
        required
      />
    </div>

    <div class="form-group">
      <label for="age">Age</label>
      <input
        type="text"
        class="form-control"
        id="name"
        [(ngModel)]="customer1.age"
        name="cus1_age"
        required
      />
    </div>

    <div class="form-group">
      <label for="job">Job</label>
      <select
        class="form-control"
        id="job"
        [(ngModel)]="customer1.job"
        name="cus1_job"
        required
      >
        <option *ngFor="let job of jobList" [value]="job">{{job}}</option>
      </select>
    </div>

    <button type="submit" class="btn btn-success">Submit</button>
  </form>
</div>
```

Chúng ta dùng cú pháp [(ngModel)]="..." trong các thẻ `<input>` hoặc `<select>` để kết nối dữ liệu của thẻ đó với một biến thuộc tính nào đó, ở đây chúng ta kết nối đến các thuộc tính name, age và job của đối tượng customer1.

Ngoài ra khi dùng ngModel thì thẻ đó phải khai báo thuộc tính name nữa, giá trị cho thuộc tính này đặt là gì cũng được, không nhất thiết phải là cus1_name, cus1_age…

Lưu file này lại, Angular sẽ tự reload lại trang web và bạn sẽ thấy form trên trang web đã tự động điền các giá trị tương ứng với đối tượng customer1.

- **ngModel có tính chất 2 chiều**, tức là nếu chúng ta chỉnh sửa gì trên form thì giá trị của đối tượng customer1 cũng sẽ thay đổi theo.Chúng ta có thể kiểm chứng điều này bằng cách in giá trị của đối tượng customer1 lên như sau:

src/app/customer-form.component.html

```html
...
<div class="form-group">
  <label for="name">Name</label>
  <input
    type="text"
    class="form-control"
    id="name"
    [(ngModel)]="customer1.name"
    name="cus1_name"
    required
  />
  {{ customer1.name }}
</div>
...
```

---

## Angular – Theo dõi trạng thái form với ngModel

Trong bài trước chúng ta đã tìm hiểu qua cách liên kết dữ liệu hai chiều với ngModel, ngModel không những thực hiện chức năng đó mà còn có khả năng kiểm tra trạng thái của các phần tử control trong form, chẳng hạn như nội dung textbox thay đổi, người dùng click vào…v.v

Mỗi khi có sự thay đổi trên các phần tử trong form, ngModel sẽ đổi tên class của các phần tử đó, cụ thể:

### Trạng thái

| column0                                 | column1          | column2           |
| --------------------------------------- | ---------------- | ----------------- |
| TRẠNG THÁI                              | TÊN CLASS (TRUE) | TÊN CLASS (FALSE) |
| Người dùng click vào control            | ng-touched       | ng-untouched      |
| Người dùng thay đổi dữ liệu của control | ng-dirty         | ng-pristine       |
| Dữ liệu của control không hợp lệ        | ng-valid         | ng-invalid        |

Chúng ta có thể lấy tên các lớp này thông qua biến trong template.

Bây giờ chúng ta sẽ dùng form customer đã làm trong bài trước để ví dụ, sửa lại file customer-form.component.html như sau:

src/app/customer-form.component.html

```html
<div class="container">
  <h1>Customer</h1>
  <form>
    <div class="form-group">
      <label for="name">Name</label>
      <input
        type="text"
        class="form-control"
        id="name"
        [(ngModel)]="customer1.name"
        name="cus1_name"
        required
        #cus_class
      />
      <p>Classes: {{cus_class.className}}</p>
    </div>
    ....
  </form>
</div>
```

Chúng ta khai báo biến template cho thẻ `<input>` là #cus_class, sau đó lấy thuộc tính className của biến này ra và hiển thị.

Lưu file lại, Angular sẽ reload lại trình duyệt, chúng ta có thể thấy tên các lớp của control này, ngay cả các control khác cũng thế, nếu muốn rõ hơn bạn có thể dùng chức năng insect của Google Chrome để xem.

Bạn thử click vào một ô textbox, sau đó click ra ngoài, gõ thêm kí tự vào ô, xóa nội dung trong ô đó… thì sẽ thấy tên các class này thay đổi tùy theo từng trạng thái.

Chúng ta có thể dùng các lớp này để thay đổi màu sắc, hiển thị text để thông báo cho người dùng, ví dụ chúng ta tạo file CSS có tên customer-form.css trong thư mục src như sau:

src/customer-form.css

```css
.ng-valid:required,
.ng-valid.required {
  border-left: 5px solid #42a948;
}

.ng-invalid:not(form) {
  border-left: 5px solid #a94442;
}
```

Ở đây chúng ta thay đổi màu sắc viền bên trái (border-left) cho 2 lớp ng-invalid và ng-valid. Khi người dùng xóa trống ô textbox có yêu cầu required thì viền trái sẽ chuyển thành màu đỏ.

Tiếp theo chúng ta phải thêm dòng code `<link rel="stylesheet" href="customer-form.css">` tới file này trong file index.html:

src/index.html

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Angular QuickStart</title>
    <base href="/" />
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <link rel="stylesheet" href="styles.css" />
    <link rel="stylesheet" href="customer-form.css" />

    <link
      rel="stylesheet"
      href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css"
    />
    <link
      rel="stylesheet"
      href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap-theme.min.css"
    />
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>

    <!-- Polyfill(s) for older browsers -->
    <script src="node_modules/core-js/client/shim.min.js"></script>

    <script src="node_modules/zone.js/dist/zone.js"></script>
    <script src="node_modules/systemjs/dist/system.src.js"></script>

    <script src="systemjs.config.js"></script>
    <script>
      System.import('main.js').catch(function (err) {
        console.error(err);
      });
    </script>
  </head>
  <body>
    <my-app>Loading AppComponent content here ...</my-app>
  </body>
</html>
```

Chúng ta có thể hiển thị thêm dòng chữ thông báo lỗi cho người dùng thay vì chỉ thay đổi màu sắc một cách đơn độc, như thế người dùng sẽ không biết rõ sai sót chỗ nào, chúng ta sửa lại file template như sau:

src/app/customer-form.component.html

```html
<div class="container">
  <h1>Customer</h1>
  <form>
    <div class="form-group">
      <label for="name">Name</label>
      <input
        type="text"
        class="form-control"
        id="name"
        [(ngModel)]="customer1.name"
        name="cus1_name"
        required
        #cus_class="ngModel"
      />
      <div
        [hidden]="cus_class.valid || cus_class.pristine"
        class="alert alert-danger"
      >
        Name is required
      </div>
    </div>
    ...
  </form>
</div>
```

Chúng ta gán giá trị cho biến template #cus_class là ngModel, sau đó viết thêm một đoạn `<div></div>` nữa để hiển thị thông báo ‘Name is required’ nếu người dùng bỏ trống ô `<input>`.

Lý do ở đây chúng ta gán #cus_class là ngModel là vì mỗi chỉ thị trong Angular có một thuộc tính là exportAs, thuộc tính này chẳng qua là một đối tượng của chỉ thị đó nhưng chúng ta có thể sử dụng ở bất cứ đâu, và giá trị của thuộc tính này trong chỉ thị ngModel cũng là “ngModel" luôn.

![img](angular_basic.assets/Capture2-300x268.jpg)

Ở đoạn code trên chúng ta quy định thẻ `<div></div>` mới có được hiển thị hay không thông qua thuộc tính hidden, và chúng ta gắn giá trị của biến template vào thuộc tính hidden này.

### Submit form

Form hiện tại của chúng ta chưa thực hiện chức năng submit, để có thể submit được thì chúng ta sử dụng chỉ thị ngSubmit, chúng ta sửa lại file customer-form.component.html như sau:

src/app/customer-form.component.html

```html
<div class="container">
  <h1>Customer</h1>
  <form (ngSubmit)="onSubmit()" #customerForm="ngForm">
    ...
  </form>
</div>
```

Chúng ta gán thuộc tính (ngSubmit) là phương thức onSubmit(), trong lớp CustomerFormComponent chúng ta khai báo thêm onSubmit().

src/app/customer-form.component.ts

```ts
import { Component } from '@angular/core';
import { Customer } from './customer';

@Component({
  moduleId: module.id,
  selector: 'customer',
  templateUrl: './customer-form.component.html',
})
export class CustomerFormComponent {
  jobList = [
    'Software Developer',
    'Tester',
    'Project Manager',
    'Business Analyst',
  ];
  customer1 = new Customer(1, 'Pho Coder', 24, this.jobList[0]);
  onSubmit() {}
}
```

Ở đây chúng ta chưa xử lý gì nhiều.

Ngoài ra ở trên form chúng ta còn khai báo biến template là #customerForm với giá trị là ngForm, và đây là giá trị của thuộc tính exportAs trong chỉ thị ngForm, tuy nhiên ở đây khác với ngModel là chúng ta chưa khai báo dòng nào tương tự như [(ngForm)]="..." cả, lý do chúng ta vẫn dùng được exportAs của ngForm là vì mỗi khi chúng ta khai bào một thẻ `<form>` thì Angular sẽ tự động khai báo thuộc tính ngForm cho thẻ `<form>` luôn.

Chúng ta có thể dùng biến template này để điều khiển nhiều thứ trong form, chẳng hạn như vô hiệu hóa nút Submit khi form không hợp lệ, form không hợp lệ khi có một phần tử trong form không hợp lệ. Ví dụ:

customer-form.component.html

```html
<div class="container">
  <h1>Customer</h1>
  <form (ngSubmit)="onSubmit()" #customerForm="ngForm">
    ....
    <button
      type="submit"
      class="btn btn-success"
      [disabled]="!customerForm.form.valid"
    >
      Submit
    </button>
  </form>
</div>
```

Chúng ta gán thuộc tính disabled là biểu thức !customerForm.form.valid, và nút "Submit" sẽ không thể click được khi có một phần tử trong form không hợp lệ, chẳng hạn như ô input bỏ trống.

---

## Angular – Template – Phần 1

Trong các bài trước chúng ta đã làm việc qua với cú pháp của template, trong phần này chúng ta sẽ tìm hiểu kỹ hơn.

Hệ thống template chịu trách nhiệm việc hiển thị nội dung lên trang web, trong các web framework phổ biến khác như Django, Ruby on Rails… v.v cũng có hệ thống template tương tự như của Angular.

### HTML

Ngôn ngữ chính của template là HTML, nhưng không phải các phần tử (hay các thẻ) đều hợp lệ với Angular, điển hình là thẻ `<script>`, với Angular thì `<script>` sẽ bị bỏ qua, không được biên dịch vì lý do bảo mật.

Chúng ta cũng có thể tự tạo ra các thẻ cho riêng mình thông qua component như trong các bài trước đã làm.

- Cú pháp lấy dữ liệu {{…}}

Chúng ta đã làm việc với cú pháp sử dụng cặp dấu ngoặc nhọn {{...}} nhiều rồi, đây là cú pháp dùng để lấy giá trị của thuộc tính trong lớp component.

```html
<h3>
  {{title}}
  <img src="{{name}}" style="height:30px" />
</h3>
```

Angular sẽ lấy giá trị của thuộc tính trong lớp component rồi chuyển thành chuỗi và thay vào đoạn dấu ngoặc nhọn {{...}}.

```html
<p>The sum of 1 + 1 is {{1 + 1}}</p>
```

Chúng ta cũng có thể thực hiện tính toán trong này.

### Biểu thức

Biểu thức ở đây là các phép tính cộng, trừ, nhân, chia, gán, so sánh…v.v

Hầu hết các biểu thức có thể sử dụng là các biểu thức của Javascript, các biểu thức có thể sử dụng là:

- Phép gán: =, +=, -= ...
- new
- Dấu chấm phẩy (;), dấu phẩy (,)
- Phép tăng (++), giảm (--)

Nhưng không phải tất cả đều có thể dùng được:

_Không thể sử dụng toán tử bit OR (ký hiệu |) và toán tử AND (ký hiệu &)_

### Ngữ cảnh của biểu thức

Một “ngữ cảnh” nói một cách đơn giản là các đối tượng thực hiện các biểu thức.

```html
{{title}} <span [hidden]="isUnchanged">changed </span>
```

Trong đoạn code trên thì title và isUnchanged là các thuộc tính của một lớp component nào đó, chẳng hạn như lớp AppComponent, và AppComponent chính là một “ngữ cảnh”.

Không phải tất cả các biến trong biểu thức luôn luôn thuộc về một đối tượng ngữ cảnh nào đó, ví dụ:

```html
<div *ngFor="let cus of customers">{{cus.name}}</div>
```

Ở đây cus lại là một đối tượng trong phép duyệt mảng customers thôi.

Chúng ta không thể dùng các đối tượng toàn cục của Javascript hay Node.js…v.v như console.log, Math.max, window, document… trong biểu thức được.

### Câu lệnh

Các câu lệnh là các đoạn code thực hiện một công việc gì đó để phản hồi lại các sự kiện. Ví dụ:

```html
<button (click)="createCustomer()">Register</button>
```

Trong đoạn code trên thì createCustomer() chính là một câu lệnh trả lời lại sự kiện (click).

### Ngữ cảnh của câu lệnh

Cũng tương tự như ngữ cảnh của biểu thức, ngữ cảnh của câu lệnh cũng là một đối tượng của lớp component đã tạo ra template đó. Chẳng hạn như trong đoạn code trên thì câu lệnh createCustomer() có thể có ngữ cảnh là đối tượng của một lớp AppComponent nào đó.

Câu lệnh gọi hàm có thể nhận vào tham số là các biến biểu thức, ví dụ:

```html
<button (click)="onSave($event)">Save</button>
<button *ngFor="let cus of customers" (click)="createCustomer(cus)"></button>
<form #customerForm (ngSubmit)="onSubmit(customerForm)">...</form>
```

Và cũng tương tự như ngữ cảnh của biểu thức, chúng ta không thể gọi những đối tượng toàn cục như window, document, console.log, Math.max…v.v

### Cú pháp kết nối dữ liệu

Đây là các cú pháp dùng để kết nối dữ liệu qua lại giữa lớp component và template, hỗ trợ việc đọc ghi dữ liệu một cách dễ dàng, **chiều kết nối có thể là 1 chiều hoặc 2 chiều**, tức là chỉ có thể đọc dữ liệu từ lớp component ra template hoặc ngược lại hoặc cả hai. Việc chúng ta cần làm là ghi cú pháp ra và Angular sẽ lo nốt phần bên dưới.

Nhìn chung thì có thể chia các cú pháp này ra làm 3 loại dựa theo chiều kết nối:

| CHIỀU KẾT NỐI                         | CÚ PHÁP                                                    | LOẠI (TARGET)  |
| ------------------------------------- | ---------------------------------------------------------- | -------------- |
| 1 chiều từ lớp component tới template | {{biểu thức}} [target]="biểu thức" bind-target="biểu thức" | Thuộc tính Lớp |
| 1 chiều từ template về lớp component  | (target)="câu lệnh" on-target="câu lệnh"                   | Sự kiện        |
| 2 chiều                               | [(target)]="biểu thức" bindon-target="biểu thức"           | 2 chiều        |

Loại (hay target) là tên các sự kiện, lớp, thuộc tính… và được bọc trong cặp dấu ngoặc vuông [], ngoặc tròn () hoặc sau các tiền tố bind-, on-, bindon-.

---

## Angular – Template – Phần 2

Trong phần này chúng ta tiếp tục tìm hiểu về template trong Angular.

### Bắt thuộc tính […]

Bắt thuộc tính ở đây là chúng ta gán thuộc tính của một element/thẻ cho một biểu thức của template. Khi bắt thuộc tính thì chúng ta bọc tên thuộc tính trong cặp thẻ ngoặc vuông [].

Thông thường chúng ta gán thuộc tính đó cho một giá trị nào đó trong lớp component.

```html
<img [src]="customerUrl" />
```

Chẳng hạn như trong đoạn code trên, chúng ta gán thuộc tính src của element `<img>` là giá trị của thuộc tính customerUrl, customerUrl là thuộc tính của một lớp component nào đó.

```html
<button [disabled]="isUnchanged">Cancel is disabled</button>
```

Hoặc chúng ta gán thuộc tính disabled là giá trị của thuộc tính isUnchanged.

```html
<customer [cust]="currentCustomer"></customer>
```

Thuộc tính đó cũng có thể là một đối tượng chứ không phải là các giá trị đơn lẻ như số, chuỗi…v.v

**Lưu ý:**

- Việc kết nối giá trị từ template vô lớp component là một chiều, chúng ta không thể thay đổi giá trị của thuộc tính thông qua việc bắt thuộc tính
- Không thể gán giá trị cho thuộc tính là một phương thức

Nếu element có phát sinh sự kiện thì chúng ta có thể bắt sự kiện (chúng ta sẽ tìm hiểu sau)
Ngoài việc bọc tên thuộc tính trong cặp dấu ngoặc vuông [], thì chúng ta có thể nối vào đầu tên thuộc tính tiền tố bind-, ví dụ 2 đoạn code dưới đây là giống nhau:

```html
<img [src]="customerUrl" /> <img bind-src="customerUrl" />
```

Bạn có thể dùng 1 trong 2 cách trên đều được.

Cú pháp bắt thuộc tính này cũng giống như cú pháp {{...}} vậy, 2 đoạn code dưới đây là tương đương nhau:

```html
<img src="{{customerUrl}}" /> <img [src]="customerUrl" />
```

Việc dùng cú pháp nào là tùy ở bạn, bạn thấy thích dùng cái gì thì dùng.

### Bắt sự kiện (…)

Bắt thuộc tính là lấy dữ liệu từ lớp component truyền lên template, bắt sự kiện thì ngược lại là phát sinh dữ liệu từ template và truyền về lớp component.

Sự kiện là những hành động như nhập chữ vào ôn các ô input, click chuột, chọn item từ một danh sách.

Cách duy nhất để biết sự kiện gì vừa xảy ra là lắng nghe sự kiện đó – hay bắt sự kiện đó.

Cú pháp bắt sự kiện bao gồm tên sự kiện được bọc trong cặp dấu ngoặc tròn (), dấu bằng =, và cuối cùng là một câu lệnh nằm trong cặp dấu nháy kép "". Ví dụ:

```html
<button (click)="onSave()">Save</button>
```

Trong đoạn code trên, chúng ta lắng nghe sự kiện (click), tức là click chuột, khi người dùng click chuột vào button thì sự kiện sẽ xảy ra, và câu lệnh ở bên phải sẽ được thực thi, ở đây là lời gọi hàm onSave().

Ngoài việc bọc tên sự kiện trong cặp dấu ngoặc tròn thì chúng ta có thể chèn trước tên sự kiện tiền tố on-, ví dụ 2 đoạn code dưới đây là giống nhau:

```html
<button (click)="onSave()">Save</button>
<button on-click="onSave()">On Save</button>
```

Khi sự kiện xảy ra, Angular sẽ thực thi câu lệnh trong dấu nháy kép, ngoài ra Angular còn truyền thêm dữ liệu đi kèm nữa, các dữ liệu đó sẽ được nằm trong một đối tượng có tên là \$event.

```html
<button (click)="onSave($event)">Save</button>
```

Đối tượng này chứa những gì tùy thuộc vào loại sự kiện, nếu sự kiện xảy ra là các sự kiện thông thường trong HTML, mà người ta hay gọi là sự kiện DOM, thì \$event sẽ chứa những gì mà chuẩn DOM quy định, chẳng hạn như target, target.value...v.v Bạn có thể xem các sự kiện DOM của đây:

https://developer.mozilla.org/en-US/docs/Web/Events

### Bắt dữ liệu 2 chiều [(…)]

Đây là cú pháp cho phép bạn vừa có thể lấy dữ liệu từ component, vừa có thể chỉnh sửa dữ liệu đó từ template.

Để làm việc này thì chúng ta bọc thuộc tính của element trong cặp dấu [()]. Lưu ý là dấu ngoặc tròn () bao giờ cũng nằm trong dấu ngoặc vuông []. Ví dụ:

```ts
import { Component } from '@angular/core';

@Component({
  selector: 'my-app',
  template: `
    <input [(ngModel)]="username" />

    Hello {{ username }}
  `,
})
export class AppComponent {
  username = '';
}
```

Lớp AppComponent có một thuộc tính là username. Thuộc tính ngModel có giá trị là giá trị của thuộc tính username, khi người dùng thay đổi nội dung trong element `<input>` thì giá trị của ngModel cũng được thay đổi theo.

---

## Angular – Template – Phần 3

Trong phần này chúng ta sẽ tìm hiểu về biến template và 2 thuộc tính @Input và @Output.

### Biến template (#var)

Đây là các biến mà chúng ta khai báo cho mỗi element trong một trang web, chúng ta có thể dùng biến này để đọc dữ liệu và gọi phương thức của lớp component hoặc chỉ thị.

Để khai báo biến template thì chúng ta dùng kí tự # rồi ghi tên biến ngay bên trong element.

```html
<input #phone placeholder="phone number" />
```

Trong đoạn code trên chúng ta khai báo biến #phone cho element `<input>`. Sau khi đã khai báo thì chúng ta có thể gọi đến biến này ở bất cứ đâu trong đoạn code template đó.

```html
<input #phone placeholder="phone number" />

<button (click)="callPhone(phone.value)">Call</button>
```

Khi gọi biến template thì chúng ta ghi tên biến ra nhưng không ghi dấu #.

Trong đoạn code trên, khi chúng ta click button thì biến #phone sẽ lấy dữ liệu trong thuộc tính value của element `<input>`, rồi truyền vào phương thức callPhone().

Nếu chúng ta chỉ khai báo biến template không như thế thì thuộc tính value của biến hầu như sẽ là value của element, tuy nhiên chúng ta có thể chỉ định biến template này tham chiếu tới một đối tượng khác, chẳng hạn như một chỉ thị, ví dụ:

```html
<form (ngSubmit)="onSubmit(customerorm)" #customerForm="ngForm">
  <div class="form-group">
    <label for="name">
      Name
      <input
        class="form-control"
        name="name"
        required
        [(ngModel)]="customer.name"
      />
    </label>
  </div>
  <button type="submit" [disabled]="!customerForm.form.valid">Submit</button>
</form>
```

Nếu bạn còn nhớ thì mỗi khi chúng ta tạo form thì Angular sẽ gán cho form đó một đối tượng chỉ thị ngForm luôn để chúng ta có thể thực hiện một số thao tác trên form dễ dàng, chúng ta chỉ cần gán đối tượng ngForm đó cho biến template là có thể sử dụng được.

Chúng ta có thể sử dụng tiền tố **ref-** thay cho kí tự #, tùy bạn thích dùng cái nào cũng được.

```html
<input ref-fax placeholder="fax number" />
<button (click)="callFax(fax.value)">Fax</button>
```

### Thuộc tính @Input và @Output

Hai thuộc tính này có tác dụng khai báo các biến và sự kiện dùng trong việc kết nối dữ liệu.

Trong các bài trước chúng ta đã quen với việc kết nối dữ liệu từ thuộc tính và sự kiện của element sang một thuộc tính hoặc phương thức của lớp component, ví dụ:

```html
<img [src]="iconUrl" /> <button (click)="onSave()">Save</button>
```

Trong đoạn code trên thì src là thuộc tính của element `<img>` và được kết nối tới thuộc tính iconUrl, click là sự kiện của element `<button>` và được kết nối tới phương thức onSave().

Điều này cũng có nghĩa là chúng ta chỉ được phép sử dụng các thuộc tính và sự kiện có sẵn của element như src và click thôi, trong Angular có 2 thuộc tính @Input và @Output, 2 thuộc tính này sẽ cho phép chúng ta tự tạo ra các thuộc tính và phương thức có thể bắt dữ liệu riêng cho chúng ta.

Ví dụ, chúng ta tạo một project mới và tạo một lớp tên CustomerFormComponent như sau:

src/app/customer-form.component.ts

```ts
import { Component, Input, Output, EventEmitter } from '@angular/core';
import { Customer } from './customer';

@Component({
  moduleId: module.id,
  selector: 'customer',
  template: `<button
    type="button"
    class="btn btn-primary"
    (click)="emitEvent()"
  >
    Change name
  </button> `,
})
export class CustomerFormComponent {
  @Input() name: string;
  @Output() changeName = new EventEmitter();

  emitEvent() {
    this.changeName.emit();
  }
}
```

Chúng ta khai báo các thuộc tính @Input và @Output bằng cách thêm 2 từ khóa này vào trước tên biến, sau đó khai báo kiểu dữ liệu đối với thuộc tính @Input hoặc gán một đối tượng EventEmitter cho thuộc tính @Output. Để có thể sử dụng @Input và @Output thì chúng ta phải import từ @angular/core, ngoài ra ở đây chúng ta còn import thêm cả lớp EventEmitter nữa.

Lớp **EventEmitter** là lớp giúp phát sinh sự kiện, để phát sự kiện thì chúng ta gọi phương thức emit() của lớp này. Trong đoạn code trên lớp **CustomerFormComponent** có một template bao gồm 1 button, khi click button này thì phương thức emitEvent() sẽ được gọi, trong phương thức này chúng ta gọi phương thức emit() của đối tượng changeName để phát sinh sự kiện. Chi tiết về lớp **EventEmitter** sẽ được trình bày trong bài khác.

Tiếp theo chúng ta sử dụng lớp **CustomerFormComponent** như sau:

src/app/app.component.ts

```ts
import { Component } from '@angular/core';
import { CustomerFormComponent } from './customer-form.component';

@Component({
  selector: 'my-app',
  template: `
    <customer [name]="username" (changeName)="saveNewName()"></customer>
    {{ username }}
  `,
})
export class AppComponent {
  username = 'Pho Code';

  saveNewName() {
    this.username = 'Pho Code Blog';
  }
}
```

Chúng ta import lớp CustomerFormComponent, sau đó khai báo selector, rồi bắt các thuộc tính @Input và @Output như bắt các thuộc tính và sự kiện thông thường.

---

## Angular – Directive – Phần 1

Trong phần này chúng ta sẽ tìm hiểu về các Directive (chỉ thị) có sẵn trong Angular.

**Directive** (chỉ thị) là một lớp và có phần khai báo metadata là @Directive, ở đây chúng ta chỉ tìm hiểu về các directive có sẵn trong Angular, còn việc định nghĩa directive sẽ được trình bày trong bài khác. Thường thì directive sẽ nằm trong một element – hay thẻ của HTML giống như một thuộc tính bình thường.

**Directive có 2 loại là structural và attribute.**

### Attribute directive

Đây là các chỉ thị có tác dụng lắng nghe và thay đổi cách thức hiển thị của các element, thuộc tính… trong HTML. Thông thường chúng cũng được dùng giống như một thuộc tính của một element.

Trong phần này chúng ta sẽ tìm hiểu về 3 loại chỉ thị thường dùng là:

- NgClass: thêm/bớt các lớp CSS
- NgStyle: thêm/bớt các style
- NgModel: kết nối dữ liệu 2 chiều, trong bài trước chúng ta đã có tìm hiểu sơ qua

### NgClass

Directive này cho phép bạn thêm hoặc bớt các lớp CSS một cách chủ động. Thông thường chúng ta sẽ gán giá trị cho chỉ thị ngClass là một đối tượng lưu dữ liệu theo dạng từ điển, tức là mỗi phần tử là một cặp `<key>:<value>`. Ví dụ:

```ts
export class SetClass {
  currentClasses: {};
  setCurrentClasses() {
    this.currentClasses = {
      saveable: this.canSave,
      modified: !this.isUnchanged,
      special: this.isSpecial,
    };
  }
}
```

Trong đoạn code trên, chúng ta có lớp SetClass, lớp này có một đối tượng currentClasses, phương thức setCurrentClasses() sẽ thiết lập đối tượng currentClasses() gồm 3 phần tử là saveable, modified và special, đây cũng sẽ được dùng làm tên lớp CSS luôn, giá trị của mỗi phần tử này dựa vào các thuộc tính khác, ở đây chúng ta dùng thuộc tính canSave, isUnchanged và isSpecial.

Khi sử dụng ngClass thì chúng ta chỉ cần làm như sau:

```html
<div [ngClass]="currentClasses">
  This div is initially saveable, unchanged, and special
</div>
```

Chúng ta kết nối chỉ thị ngClass tới đối tượng currentClasses là được, tất nhiên trước đó chúng ta phải gọi phương thức setCurrentClasses() để thiết lập các phần tử trong đối tượng currentClasses, và element `<div>` sẽ có class là saveable, unchanged và special.

### NgStyle

Chỉ thị ngStyle có chức năng thiết lập style của element bên trong element đó. Tương tự với ngClass, chúng ta cũng thường gán giá trị cho ngStyle là một đối tượng lưu trữ dạng từ điển.

```ts
export class SetStyle {
  currentStyles: {};
  setCurrentStyles() {
    this.currentStyles = {
      'font-style': this.canSave ? 'italic' : 'normal',
      'font-weight': !this.isUnchanged ? 'bold' : 'normal',
      'font-size': this.isSpecial ? '24px' : '12px',
    };
  }
}
```

Trong đoạn code trên chúng ta có lớp SetStyle, trong này có một đối tượng currentStyles lưu trữ các style CSS theo dạng từ điển, các key sẽ có giá trị tùy thuộc vào các thuộc tính nào đó, nói chung cũng tùy bạn quy định,

```html
<div [ngStyle]="currentStyles">
  This div is initially italic, normal weight, and extra large (24px).
</div>
```

Và chúng ta cũng thiết lập chỉ thị ngStyle cho thuộc tính currentStyles này, tất nhiên là phải gọi phương thức setCurrentStyles() ở đâu đó trước.

### NgModel

Chúng ta đã biết là chỉ thị ngModel dùng để kết nối dữ liệu 2 chiều, tức là vừa có thể đọc dữ liệu từ lớp và hiển thị lên template, vừa có thể chỉnh sửa dữ liệu trên template và cập nhật vào lớp đó. Ví dụ:

```html
<input [(ngModel)]="currentCustomer.name" />
```

Một yêu cầu cần có của chỉ thị ngModel là **bạn phải import lớp FormsModule vào lớp AppModule** trước thì mới có thể sử dụng:

```ts

import { NgModule } from '@angular/core';
import { BrowserModule } from '@angular/platform-browser';
import { FormsModule } from '@angular/forms';

@NgModule({
    imports: [
        BrowserModule,
        FormsModule
    ],
    ...
})
export class AppModule { }

```

---

## Angular – Directive – Phần 2

Trong phần này chúng ta tiếp tục tìm hiểu về directive.

### Structural directive

Các chỉ thị thuộc loại structural chịu trách nhiệm điều khiển cách dữ liệu được hiển thị, chẳng hạn như thêm, bớt, chỉnh sửa các element…v.v Ở đây chúng ta chỉ tìm hiểu 3 chỉ thị thường dùng là ngIf, ngFor và ngSwitch.

Nếu bạn để ý thì có thể nhận thấy chức năng của 3 chỉ thị này giống với các câu lệnh if, for, switch trong các ngôn ngữ lập trình.

### ngIf

Chỉ thị ngIf cho phép chúng ta thêm hoặc loại bỏ một element ra khỏi trang, chúng ta gán giá trị cho chỉ thị này là một biểu thức nào đó có trả về giá trị true hoặc false, nếu biểu thức trả về true thì element sẽ hiện ra, ngược lại thì không.

```html
<customer *ngIf="isActive"></customer>
```

Trong đoan code trên, element `<customer>` sẽ được hiển thị nếu isActive trả về true, isActive có thể là một thuộc tính/biến nào đó hoặc một phương thức…v.v

**Lưu ý luôn phải có dấu sao \* trước ngIf.**

Một điều khác là ở đây ngIf thêm hoặc bỏ element trong trang web, chứ không phải là ẩn hay hiện element đó, tức là khác với thuộc tính hidden của các element trong HTML.

Thông thường chúng ta dùng ngIf để kiểm tra xem một đối tượng nào đó có NULL hay không

```html
<div *ngIf="currentCustomer">Hello, {{currentCustomer.name}}</div>
<div *ngIf="nullCustomer">Hello, {{customer.name}}</div>
```

### Sử dụng template trong if else

```html
<p *ngIf="is_available; then true_condition else false_condition">
  Điểu kiện đúng trong thẻ ngIf
</p>
<ng-template #true_condition><p>Điều kiện đúng trong template</p></ng-template>
<ng-template #false_condition><p>Điều kiện sai trong template</p></ng-template>
```

Một lưu ý nhỏ là điều kiện trong template được ưu tiên hơn so với thẻ cha chứa cấu trúc điều khiển. Nghĩa là nếu is_available = true thì chỉ nội dung bên trong #true_condition được thực thi

### ngFor

Đây là chỉ thị lặp, có tác dụng lặp qua một danh sách các phần tử, khi chúng ta có một danh sách các phần tử, muốn hiển thị chúng lên trang web thì chúng ta lặp qua danh sách đó và hiển thị các phần tử theo một khuôn mẫu giống nhau. Ví dụ:

```html
<div *ngFor="let cus of customers">
  {{cus.name}}
</div>
```

Giá trị của ngFor là một câu lệnh có cú pháp như sau:

```ts
let <biến lặp> of <danh sách>

```

Biến lặp là do chúng ta tự đặt, bạn muốn đặt là gì cũng được, ngFor sẽ lặp qua danh sách và mỗi lần lặp thì chúng ta dùng biến lặp để lấy dữ liệu của phần tử hiện tại trong danh sách.

**Lưu ý luôn phải có dấu sao \* trước ngFor.**
Trong ngFor có một thuộc tính tên là index, thuộc tính này lưu trữ số thứ tự của phần tử đang được lặp, chúng ta có thể lấy số thứ tự giá trị index này như sau:

```html
<div *ngFor="let cus of customers; let i=index">{{i + 1}} : {{cus.name}}</div>
```

### ngSwitch

Chỉ thị ngSwitch cũng tương tự như câu lệnh switch trong Javascript vậy, chỉ thị này có tác dụng hiển thị một element trong một danh sách các element, dựa vào một điều kiện cho trước.

Trong ngSwitch lại có 2 chỉ thị khác nữa là ngSwitchCase và ngSwitchDefault.

```html
<div [ngSwitch]="currentCustomer.emotion">
    <happy-customer   *ngSwitchCase="'happy'"    [cus]="currentCustomer"></happy-customer>
    <sad-customer     *ngSwitchCase="'sad'"      [cus]="currentCustomer"></sad-customer>
    <confused-custoer *ngSwitchCase="'confused'" [cus]="currentCustomer"></confused-customer>
    <unknown-customer *ngSwitchDefault           [cus]="currentCustomer"></unknown-customer>
</div>
```

Trong đoạn code trên, ngSwitch được gán bằng giá trị của thuộc tính emotion trong đối tượng currentCustomer, thuộc tính emotion có thể là bất cứ giá trị gì, trong trường hợp này thì đây là một string “happy”, “sad” hoặc “confused”, sau đó bên trong ngSwitch, chúng ta có các element có chỉ thị ngSwitchCase, mỗi chỉ thị ngSwitchCase này được gán giá trị là một chuỗi trùng với thuộc tính emotion, nếu element nào có chỉ thị ngSwitchCase trùng với giá trị của thuộc tính emotion thì element đó được đưa vào trang web, các element còn lại thì không. Nếu không có ngSwitchCase nào trùng thì element có chỉ thị ngSwitchDefault sẽ được đưa vào.

**Lưu ý** là ngSwitch là một chỉ thị attribute, vì chỉ thị này không trực tiếp chỉnh sửa giao diện, do đó chúng ta không thêm dấu sao _ mà bọc trong cặp dấu ngoặc vuông [], còn các chỉ thị ngSwitchCase và ngSwitchDefault thì cần có dấu sao _ phía trước.

---

## Angular – Service và Dependency Injection

**Service** (dịch vụ) chẳng qua cũng là một cách giúp cho chúng ta tái sử dụng code mà thôi, chẳng hạn như bạn có một lớp Customer, thì thay vì mỗi lần cần lấy các đối tượng Customer đang có, chúng ta phải viết code để tạo đối tượng, truyền tham số…v.v ở nhiều nơi khác nhau, thì bây giờ chúng ta chỉ cần viết một lớp service làm điều đó luôn cho chúng ta, như vậy việc quản lý code sẽ dễ dàng hơn, chẳng hạn như mỗi lần thay đổi phương thức khởi tạo, thì chúng ta chỉ cần thay đổi code trong lớp service là được, thay vì phải đi sửa lại toàn bộ những dòng code khởi tạo đó.

**Dependency Injection** là chức năng cho phép chúng ta “nhúng” các lớp vào các lớp khác, giống như dùng một thư viện vậy, và chúng ta có thể dùng các lớp được nhúng vào đó giống như dùng một thuộc tính bình thường mà không cần phải thực hiện các công đoạn khai báo, khởi tạo…v.v

Ví dụ
Chúng ta sẽ viết một lớp service lấy danh sách các ngôn ngữ lập trình.

Đầu tiên chúng ta tạo một project mới từ quickstart, đặt tên là gì cũng được.

Tiếp theo chúng ta viết lớp Language bằng cách tạo một file có tên language.ts trong thư mục src/app như sau:

src/app/language.ts

```ts
export class Language {
  id: number;
  name: string;
}
```

Ở đây chúng ta chỉ lưu 2 thông tin đơn giản là id và name.

Kế tiếp chúng ta tạo một file có tên language-list.ts trong thư mục src/app như sau:

src/app/language-list.ts

```ts
import { Language } from './language';

export const LANGUAGES: Language[] = [
  { id: 1, name: 'C++' },
  { id: 2, name: 'Java' },
  { id: 3, name: 'Python' },
  { id: 4, name: 'Ruby' },
  { id: 5, name: 'Go' },
  { id: 6, name: 'Javascript' },
];
```

File này chỉ chứa một đối tượng LANGUAGES là một mảng chứa các đối tượng Language.

Bây giờ chúng ta sẽ viết lớp service, chúng ta tạo một file có tên language.service.ts trong thư mục src/app như sau:

src/app/language.service.ts

```ts
import { Injectable } from '@angular/core';

import { Language } from './language';
import { LANGUAGES } from './languages-list';

@Injectable()
export class LanguageService {
  getLanguages(): Language[] {
    return LANGUAGES;
  }
}
```

Lớp service ở đây chúng ta đặt tên là LanguageService, trong lớp này có một phương thức là getLanguages(), phương thức này sẽ trả về mảng các đối tượng Language. Mảng này chúng ta lấy từ đối tượng LANGUAGES đã dược định nghĩa ở trên.

Thông thường chúng ta sẽ đặt tên file cho các lớp Service có phần đuôi là .service.ts cho dễ quản lý.

Điểm đáng chú ý ở đây chúng ta có import thêm lớp **Injectable** từ @angular/core và khai báo @Injectable trước phần khai báo lớp nữa, từ khóa @Injectable cho Angular biết lớp này có thể được “nhúng” vào các lớp khác.

Bây giờ chúng ta sửa lại lớp AppComponent trong file src/app/app.component.ts như sau:

src/app/app.component.ts

```ts
import { Component } from '@angular/core';
import { LanguageService } from './language.service';
import { Language } from './language';

@Component({
  selector: 'my-app',
  template: `
    <div class="container">
      <h1>Programming languages:</h1>
      <ul class="list-group">
        <li class="list-group-item" *ngFor="let lang of languages">
          {{ lang.id }} - {{ lang.name }}
        </li>
      </ul>
    </div>
  `,
  providers: [LanguageService],
})
export class AppComponent {
  languages: Language[];
  constructor(private languageService: LanguageService) {
    this.languages = languageService.getLanguages();
  }
}
```

Trong lớp AppComponent chúng ta khai báo một thuộc tính là languages, thuộc tính này có kiểu là mảng các đối tượng Language.

Sau đó chúng ta khai báo phương thức constructor(), phương thức này có nhận vào một tham số là:

**private languageService: LanguageService**

Khai báo như thế thì Angular sẽ tạo một đối tượng thuộc lớp LanguageService cho lớp AppComponent với tên là languageService, và kể từ bây giờ chúng ta có thể dùng đối tượng languageService giống như một thuộc tính bình thường của một lớp luôn. Do đó ngay trong phương thức khởi tạo chúng ta gọi phương thức getLanguages() để lấy danh sách các đối tượng Language rồi gán vào thuộc tính languages.

Một lớp để được khai báo trong constructor() thì ngoài phần import ra, còn phải được khai báo trong tham số mảng providers nữa.

Trong template chúng ta in danh sách các ngôn ngữ lập trình ra, lưu ý ở đây chúng ta có sử dụng bootstrap (bạn có thể lấy link CDN của bootstrap tại đây rồi chèn vào file src/index.html).

Bây giờ bạn có thể lưu file lại và chạy ra được như hình dưới đây:

Tuy nhiên bản chất của các service thường là chạy ngầm, song song với ứng dụng chính, nhưng ở đây service của chúng ta không phải chạy như thế mà vẫn chạy theo thứ tự trước sau cùng với ứng dụng chính. Để lớp service chạy đúng nghĩa với tính chất của một dịch vụ thì ở đây chúng ta dùng lớp Promise, lớp Promise sẽ giúp công việc lấy dữ liệu được thực hiện một cách bất đồng bộ (asynchronous).

Ở đây mình chỉ nói về cách sử dụng chứ không đi sâu vào tìm hiểu cơ chế bất đồng bộ làm gì. Đầu tiên chúng ta sửa lại lớp LanguageService như sau:

src/app/language.service.ts

```ts
import { Injectable } from '@angular/core';

import { Language } from './language';
import { LANGUAGES } from './languages-list';

@Injectable()
export class LanguageService {
  getLanguages(): Promise<Language[]> {
    return Promise.resolve(LANGUAGES);
  }
}
```

Chúng ta cho phương thức getLanguages() có kiểu trả về là một đối tượng Promise. Bên trong chúng ta gọi phương thức Promise.resolve(LANGUAGES) để lấy đối tượng LANGUAGES, việc lấy dữ liệu này sẽ được thực hiện ngầm song song với ứng dụng chính.

Ở bên lớp AppComponent chúng ta sửa như sau:

src/app/app.component.ts

```ts
import { Component } from '@angular/core';
import { LanguageComponent } from './language.component';
import { LanguageService } from './language.service';
import { Language } from './language';
@Component({
    selector: 'my-app',
    template: `
        <div class="container">
            <h1>Programming languages:</h1>
            <ul class="list-group">
                <li class="list-group-item" *ngFor="let lang of languages">
                    {{lang.id}} - {{lang.name}}
                </li>
            </ul>
        </div>
    `,
    providers: [ LanguageService ]
})
export class AppComponent {
    languages: Language[];
    constructor(private languageService: LanguageService) {
        languageService.getLanguages().then( (values) {
            this.languages = values;
        });
    }
}

```

Phương thức getLanguages() sẽ sau khi thực thi xong việc lấy dữ liệu thì sẽ gọi một phương thức khác và truyền dữ liệu trả về vào phương thức đó, nếu bạn chưa biết thì đây là cơ chế callback (bạn có thể tìm hiểu thêm ở [đây](http://phocode.com/javascript/nodejs/nodejs-ham-callback/)), ở đây phương thức getLanguages() sẽ trả về một đối tượng Promise, để bắt được phương thức callback đó thì chúng ta gọi phương thức then() và truyền vào tham số là một hàm, hàm đó sẽ nhận tham số trả về là mảng LANGUAGES, ở đây chúng ta đặt tên là lang rồi gán giá trị của tham số đó cho thuộc tính this.languages.

---

## Angular – Routing

Nếu bạn chưa biết Routing là gì thì có thể giải thích ngắn gọn đây là một tính năng cho phép chúng ta điều hướng các URL tới các hàm/phương thức/lớp/controller nào đó trong ứng dụng, đây là tính năng có trong hầu hết các web framework phổ biến ngày nay.

Trong Angular thì một URL sẽ được điều hướng tới một lớp Component, tức là khi người dùng trỏ URL nào vào trong trình duyệt thì Angular sẽ hiển thị template của lớp Component được điều hướng tương ứng.

Ví dụ
Chúng ta sẽ viết trang hiển thị danh sách các ngôn ngữ lập trình và trang hiển thị thông tin chi tiết của ngôn ngữ đó.

Đầu tiên chúng ta tạo một project từ quickstart.

Trong project này mình có sử dụng các lớp CSS của bootstrap, bạn có thể lấy link CDN của bootstrap tại [đây](https://getbootstrap.com/docs/4.3/getting-started/introduction/) và thêm vào trong file index.html.

Tiếp theo chúng ta tạo một file có tên language.ts có nội dung như sau:

src/app/language.ts

```ts
export class Language {
  id: number;
  name: string;
}

export const LANGUAGES: Language[] = [
  { id: 1, name: 'C++' },
  { id: 2, name: 'Java' },
  { id: 3, name: 'Javascript' },
  { id: 4, name: 'Ruby' },
  { id: 5, name: 'Python' },
  { id: 6, name: 'Golang' },
];
```

Chúng ta định nghĩa lớp Language có 2 thuộc tính là id và name. Và một biến LANGUAGES lưu danh sách các đối tượng Language.

Tiếp theo chúng ta tạo file có tên language.component.ts như sau:

src/app/language.component.ts

```ts
import { Component } from '@angular/core';
import { Language, LANGUAGES } from './language';

@Component({
  selector: 'language',
  template: `
    <h1>List of programming languages:</h1>
    <ul *ngFor="let lang of languages" class="list-group">
      <li class="list-group-item">{{ lang.id }} - {{ lang.name }}</li>
    </ul>
  `,
})
export class LanguageComponent {
  languages: Language[];

  constructor() {
    this.languages = LANGUAGES;
  }
}
```

Trong này chúng ta định nghĩa lớp LanguageComponent dùng để hiển thị danh sách các ngôn ngữ lập trình, danh sách này chúng ta lấy từ biến LANGUAGES đã định nghĩa ở trên.

Bây giờ đến phần chính là phần định nghĩa routing. Đầu tiên chúng ta sửa lại file app.module.ts như sau:

src/app/app.module.ts

```ts
import { NgModule } from '@angular/core';
import { BrowserModule } from '@angular/platform-browser';

import { AppComponent } from './app.component';
import { RouterModule } from '@angular/router';
import { LanguageComponent } from './language.component';

@NgModule({
  imports: [
    BrowserModule,
    RouterModule.forRoot([
      {
        path: 'languages',
        component: LanguageComponent,
      },
    ]),
  ],
  declarations: [AppComponent, LanguageComponent],
  bootstrap: [AppComponent],
})
export class AppModule {}
```

Điểm cần lưu ý ở đây là chúng ta cần import lớp RouterModule từ @angular/router, sau đó khai báo trong mảng imports. Khi khai báo lớp RouterModule thì chúng ta phải gọi phương thức forRoot() của lớp này, bên trong phương thức này chúng ta truyền vào một mảng, các phần tử của mảng là các đối tượng gồm 2 thuộc tính là path và component, trong đó path là đường dẫn URL do chúng ta định nghĩa, component là tên lớp Component sẽ được dùng để hiển thị trên trang web (lưu ý nhớ import lớp này vô trước và cũng phải khai báo trong mảng declarations).

Và kể từ bây giờ, khi người dùng gõ vào thanh địa chỉ trên trình duyệt là http://localhost:3000/languages thì phần template của lớp LanguageComponent sẽ được hiển thị, nhưng hiển thị ở đâu? Chúng ta phải chỉ định vị trí hiển thị nữa mới đủ.

Angular sẽ hiển thị ở những nơi có element `<router-outlet>`, do đó bây giờ chúng ta sửa lại lớp AppComponent như sau:

src/app/app.component.ts

```ts
import { Component } from '@angular/core';

@Component({
  selector: 'my-app',
  template: `
    <div class="container">
      <router-outlet></router-outlet>
    </div>
  `,
})
export class AppComponent {}
```

Và bây giờ nếu bạn trỏ tới đường dẫn http://localhost:3000/languages thì sẽ ra được trang có hình như bên dưới:

Chúng ta có thể thêm một element `<a>` để click vào URL như sau:

src/app/app.component.ts

```ts
import { Component } from '@angular/core';

@Component({
  selector: 'my-app',
  template: `
    <div class="container">
      <a routerLink="/languages">Languages</a>
      <router-outlet></router-outlet>
    </div>
  `,
})
export class AppComponent {}
```

Ở đây chúng ta dùng thuộc tính routerLink của lớp RouterModule, bạn cũng có thể sử dụng thuộc tính href, tuy nhiên chúng ta nên dùng routerLink là để tận dụng tính năng lấy tham số trong URL của lớp này.

### Tham số URL

Bây giờ chúng ta sẽ định nghĩa URL /detail để hiển thị thông tin chi tiết của các ngôn ngữ lập trình. Đầu tiên chúng ta sửa lại file app.module.ts như sau:

src/app/app.module.ts

```ts
import { NgModule } from '@angular/core';
import { BrowserModule } from '@angular/platform-browser';

import { AppComponent } from './app.component';
import { RouterModule } from '@angular/router';
import { LanguageComponent } from './language.component';
import { LanguageDetailComponent } from './language-detail.component';

@NgModule({
  imports: [
    BrowserModule,
    RouterModule.forRoot([
      {
        path: 'languages',
        component: LanguageComponent,
      },
      {
        path: 'detail/:id',
        component: LanguageDetailComponent,
      },
    ]),
  ],
  declarations: [AppComponent, LanguageComponent, LanguageDetailComponent],
  bootstrap: [AppComponent],
})
export class AppModule {}
```

Chúng ta định nghĩa URL mới với path là detail/:id, với component là lớp LanguageDetailComponent.

detail/:id có nghĩa là url có dạng localhost:3000/detail/1, localhost:3000/detail/abc…v.v Tức là có kèm theo tham số, và tham số này chúng ta đặt tên là :id (lưu ý phải có dấu 2 chấm `':'`).

Tiếp theo chúng ta định nghĩa lớp LanguageDetailComponent, chúng ta tạo file language-detail.component.ts như sau:

src/app/language-detail.component.ts

```ts
import { Component, OnInit } from '@angular/core';
import { Language, LANGUAGES } from './language';
import { ActivatedRoute, Params } from '@angular/router';

@Component({
  selector: 'lang-detail',
  template: `
    <h1>Detail:</h1>
    <div *ngIf="language">
      <h4>id: {{ language.id }}</h4>
      <h4>Name: {{ language.name }}</h4>
    </div>
  `,
})
export class LanguageDetailComponent {
  language: Language;

  constructor(private route: ActivatedRoute) {}

  ngOnInit() {
    this.route.params.subscribe((params) => {
      for (let lang of LANGUAGES) {
        if (lang.id == +params['id']) {
          this.language = {
            id: +params['id'],
            name: lang.name,
          };
        }
      }
    });
  }
}
```

Để có thể lấy giá trị tham số thì đầu tiên chúng ta phải import 2 lớp cần thiết là ActivatedRoute và Params từ @angular/router, đây là các lớp service của Angular. Sau đó chúng ta khởi tạo thuộc tính route trong phương thức constructor().

Tiếp theo chúng ta định nghĩa phương thức ngOnInit() (nhớ phải import lớp OnInit trước), phương thức này được gọi mỗi khi lớp này được gọi, trong phương thức này chúng ta lấy đối tượng Language theo tham số được gửi đến trong URL.

Để lấy tham số trong URL thì chúng ta gọi phương thức route.params.subscribe(). Phương thức này nhận vào một hàm callback có tham số là một đối tượng lưu giữ các tham số của URL, chúng ta đặt tên là params. Để lấy giá trị của các tham số, ví dụ như lấy tham số :id thì chúng ta chỉ cần ghi +params['id'] là được, chú ý phải có dấu cộng '+'. Ở đây chúng ta lặp mảng LANGUAGES và tìm xem phần tử nào có thuộc tính id trùng với tham số :id thì gán phần tử đó cho thuộc tính language.

Cuối cùng chúng ta hiển thị nội dung của thuộc tính đó lên template.

Bây giờ bạn có thể gõ vào trình duyệt các URL như localhost:3000/details/1 và sẽ thấy thông tin của ngôn ngữ lập trình tương ứng.

RouterModule cũng cung cấp url có tham số với cú pháp riêng, chúng ta sửa lại lớp LanguageComponent như sau:

language.component.ts

```ts
import { Component } from '@angular/core';
import { Language, LANGUAGES } from './language';

@Component({
  selector: 'language',
  template: `
    <h1>List of programming languages:</h1>
    <ul *ngFor="let lang of languages" class="list-group">
      <li class="list-group-item">
        <a [routerLink]="['/detail', lang.id]">
          {{ lang.id }} - {{ lang.name }}
        </a>
      </li>
    </ul>
  `,
})
export class LanguageComponent {
  languages: Language[];

  constructor() {
    this.languages = LANGUAGES;
  }
}
```

Chúng ta gán routerLink là một mảng với 2 phần tử, phần tử đầu tiên là path, phần tử thứ 2 là giá trị của tham số sẽ được gửi đi, ở đây là lang.id, tức là id của ngôn ngữ lập trình đó.

---

## Angular – HTTP

Trong phần này chúng ta sẽ tìm hiểu cách gửi các gói tin đến một web server và nhận dữ liệu trả về từ server đó.

### Tạo web server API

Để có thể gửi các truy vấn API thì trước hết chúng ta phải có một web server có các URL mẫu đã, may mắn là trong Angular có sẵn các lớp service có khả năng tạo một web server “mini” chạy cục bộ để chúng ta có thể thử nghiệm tính năng truy vấn API này.

Đầu tiên chúng ta tạo một project từ quickstart.

Trong project này mình có sử dụng bootstrap, bạn có thể lấy link CDN của bootstrap ở đây và chèn vào file index.html.

Trong web server này chúng ta sẽ lưu danh sách các ngôn ngữ lập trình và cho phép truy vấn, chỉnh sửa, xóa các thông tin này.

Đầu tiên chúng ta tạo một file có tên language.ts trong thư mục src/app như sau:

src/app/language.ts

```ts
export class Language {
  id: number;
  name: string;
}
```

Trong file này chúng ta định nghĩa lớp Language gồm 2 trường là id và name.

Tiếp theo chúng tạo một file có tên language-db.service.ts trong thư mục src/app như sau:

src/app/language-db.service.ts

```ts
import { InMemoryDbService } from 'angular-in-memory-web-api';

export class LanguageDBService implements InMemoryDbService {
  createDb() {
    let languages = [
      { id: 1, name: 'C++' },
      { id: 2, name: 'Java' },
      { id: 3, name: 'Javascript' },
      { id: 4, name: 'Ruby' },
      { id: 5, name: 'Python' },
      { id: 6, name: 'Golang' },
    ];
    return { languages };
  }
}
```

Lớp này có implement lớp giao diện InMemoryDbService, đây là lớp hỗ trợ tạo webserver cục bộ, khi implement lớp đó chúng ta phải code phương thức createDb(), phương thức này phải trả về một đối tượng mảng (lưu ý trong câu lệnh return thì mảng phải được bọc trong cặp dấu ngoặc nhọn {}), nên chúng ta tạo một đối tượng có tên languages lưu thông tin các ngôn ngữ lập trình. Một lưu ý khác là các phần tử mảng phải có một phần tử tên là id.

Khi biên dịch thì InMemoryDbService sẽ hiểu là tạo một dịch vụ web API cục bộ cho phép thao tác trên mảng đó, và cung cấp một số URL cho các API, ở đây mình chỉ liệt kê một số URL thường dùng:

GET – api/languages: lấy danh sách
GET – api/languages/{id}: lấy theo id
POST – api/languages: tạo mới đối tượng
PUT – api/languages/{id}: cập nhật theo id
DELETE – api/languages/{id}: xóa theo id
Bạn có thể tìm hiểu thêm tại đây: https://github.com/angular/in-memory-web-api

### Truy vấn API

Để có thể truy vấn các API này thì chúng ta sử dụng lớp Http có trong Angular.

Chúng ta sửa lại lớp AppComponent trong file app.component.ts như sau:

src/app/app.component.ts

```ts
import { Component, OnInit } from '@angular/core';

import { Headers, Http } from '@angular/http';
import 'rxjs/add/operator/toPromise';

import { LanguageComponent } from './language.component';

import { Language } from './language';

@Component({
  selector: 'my-app',
  template: `
    <div class="container">
      <h1>List of programming languages:</h1>
      <ul class="list-group">
        <li *ngFor="let lang of languages" class="list-group-item">
          {{ lang.id }} - {{ lang.name }}
        </li>
      </ul>
    </div>
  `,
})
export class AppComponent {
  private languages: Language[];
  private headers = new Headers({ 'Content-Type': 'application/json' });

  constructor(private http: Http) {}

  ngOnInit() {
    this.http
      .get('http://localhost:3000/api/languages')
      .toPromise()
      .then((response) => {
        this.languages = response.json().data as Language[];
      })
      .catch(this.handleError);
  }

  private handleError(error: any): Promise<any> {
    return Promise.reject(error.message || error);
  }
}
```

Chúng ta sẽ cần đến các lớp Headers, Http từ @angular/http, hàm toPromise() từ rxjs/add/operator. Lớp Language từ file language.ts đã định nghĩa ở trên. OnInit từ @angular/core để định nghĩa phương thức ngOnInit().

Đầu tiên chúng ta khai báo thuộc tính languages có kiểu mảng đối tượng của lớp Language. Sau đó khai báo thuộc tính headers từ lớp Headers, đây là lớp hỗ trợ khai báo các metadata trong gói tin HTTP.

Lớp HTTP là một lớp service, do đó chúng ta tạo biến http trong phương thức constructor() luôn.

Ở trong phương thức ngOnInit(), chúng ta gọi phương thức http.get(). Đây là phương thức dùng để gửi gói tin HTTP lên các webserver dùng phương thức GET, tham số là một đường url, phương thức này sẽ trả về một đối tượng thuộc lớp Observable, nói đơn giản thì Observable cũng có chức năng lấy dữ liệu bất đồng bộ (asynchronous) như Promise nhưng hiện đại hơn, tuy nhiên chúng ta sẽ không đi sâu vào tìm hiểu, do đó chúng ta sử dụng phương thức toPromise() để chuyển về một đối tượng Promise. Rồi gọi phương thức then() để thực hiện hàm callback, tham số của hàm callback này là dữ liệu về các ngôn ngữ lập trình mà lớp InMemoryDbService cung cấp, chúng ta đặt tên tham số là response, chúng ta gọi phương thức json().data, chuyển thành mảng Language[] và gán vào thuộc tính languages. Cuối cùng chúng ta gọi phương thức catch(), phương thức này dùng để bắt lỗi ngoại lệ nếu có, tham số của phương thức này là một phương thức khác, ở đây là handleError() do chúng ta tự đặt.

Trong phương thức handleError() chúng ta trả về một đối tượng Promise từ phương thức Promise.reject() với thông báo lỗi từ error.message.

Cuối cùng để chạy được thì chúng ta phải khai báo các lớp cần thiết trong lớp AppModule (app.module.ts):

src/app/app.module.ts

```ts
import { NgModule } from '@angular/core';
import { BrowserModule } from '@angular/platform-browser';

import { AppComponent } from './app.component';

import { HttpModule } from '@angular/http';
import { InMemoryWebApiModule } from 'angular-in-memory-web-api';

import { LanguageDBService } from './language-db.service';
import { LanguageComponent } from './language.component';

@NgModule({
  imports: [
    BrowserModule,
    HttpModule,
    InMemoryWebApiModule.forRoot(LanguageDBService),
  ],
  declarations: [AppComponent, LanguageComponent],
  bootstrap: [AppComponent],
})
export class AppModule {}
```

Chúng ta import các lớp tự định nghĩa là LanguageComponent, LanguageDBService và khai báo trong mảng declarations. Khai báo 2 module cần dùng để tạo webserver và truy vấn webserver là HttpModule và InMemoryWebApiModule, rồi khai báo trong mảng imports. Khi khai báo module InMemoryWebApiModule thì chúng ta phải gọi phương thức forRoot() và truyền vào một lớp đã implements lớp InMemoryDbService, ở đây là lớp LanguageDBService.

Bây giờ giao diện trang web sẽ như thế này:

Để gửi truy vấn POST thì chúng ta dùng phương thức post() như sau:

src/app/app.component.ts

```ts
...
ngOnInit() {
    this.http.post(
                      "http://localhost:3000/api/languages",
                      JSON.stringify({name: 'Pascal'}),
                      {headers: this.headers}
                  )
             .toPromise()
             .then(res => res.json().data as Language)
             .catch(this.handleError);
    this.http.get("http://localhost:3000/api/languages")
             .toPromise()
             .then(response => {
                 this.languages = response.json().data as Language[];
             })
             .catch(this.handleError);
}
...

```

Tham số đầu tiên là URL, tham số thứ 2 là một chuỗi JSON, tham số thứ 3 là đối tượng Headers. API này sẽ trả về thông tin về đối tượng mới được tạo.

Để gửi gói tin DELETE thì chúng ta dùng phương thức delete(), ví dụ:

src/app/app.component.ts

```ts

...
ngOnInit() {
    this.http.delete(
                        "http://localhost:3000/api/languages/2",
                        {headers: this.headers}
                    )
             .toPromise()
             .then(() => null)
             .catch(this.handleError);

    this.http.post(
                      "http://localhost:3000/api/languages",
                      JSON.stringify({name: 'Pascal'}),
                      {headers: this.headers}
                  )
             .toPromise()
             .then(res => res.json().data as Language)
             .catch(this.handleError);

    this.http.get("http://localhost:3000/api/languages")
             .toPromise()
             .then(response => {
                 this.languages = response.json().data as Language[];
             })
             .catch(this.handleError);
 }
...

```

Phương thức delete() nhận vào url và một đối tượng Headers, không trả về cái gì cả nên chúng ta cho return null.

Để cập nhật một đối tượng thì chúng ta gọi phương thức put(), ví dụ:

src/app/app.component.ts

```ts
...
ngOnInit() {
    let language: Language = {
        id: 3,
        name: 'Javascript and TypeScript'
    };
    this.http.put(
                     "http://localhost:3000/api/languages/3",
                     JSON.stringify(language),
                     {headers: this.headers}
                 )
            .toPromise()
            .then(res => res.json().data as Language)
            .catch(this.handleError);

    this.http.delete(
                        "http://localhost:3000/api/languages/2",
                        {headers: this.headers}
                    )
             .toPromise()
             .then(() => null)
             .catch(this.handleError);

    this.http.post(
                      "http://localhost:3000/api/languages",
                      JSON.stringify({name: 'Pascal'}),
                      {headers: this.headers}
                  )
             .toPromise()
             .then(res => res.json().data as Language)
             .catch(this.handleError);

    this.http.get("http://localhost:3000/api/languages")
             .toPromise()
             .then(response => {
                 this.languages = response.json().data as Language[];
             })
             .catch(this.handleError);
}
...

```

Phương thức put() nhận vào url, chuỗi JSON của đối tượng cần chỉnh sửa, và một đối tượng Headers, phương thức này trả về đối tượng đã được chỉnh sửa thành công.

---

## Angular 4 nghiep UIT

https://www.youtube.com/watch?v=Cj_dNjhbM58&list=PLJ5qtRQovuENHYHqlQP5XT7zwbCA5Q5He&index=3

### Các câu lệnh thường sử dụng trong Angular CLI

| Câu lênh                                                               | Ghi chú                                                                              |
| ---------------------------------------------------------------------- | ------------------------------------------------------------------------------------ |
| ng new PROJECT-NAME                                                    | Tạo project Angular mới tên là PROJECT-NAME                                          |
| ng g component new-component ng g component new-component --spec false | Tạo component mới có tên là new-component(bo file spec)                              |
| ng g directive new-directive                                           | Tạo directive mới có tên là new-directive                                            |
| ng g pipe new-pipe                                                     | Tạo pipe mới có tên là new-pipe                                                      |
| ng g service new-service                                               | Tạo service mới có tên là new-service                                                |
| ng g module my-module                                                  | Tạo module mới có tên là my-module                                                   |
| ng serve --port 3006 --open                                            | Biên dịch project, chạy ở cổng 3006 và tự động mở lên trình duyệt khi biên dịch xong |

### Component

Tao folder components

```ts
cd components/
ng g c hello
```

Để tạo component mới, ta sử dụng lệnh Angular CLI:

```ts
ng g component <ten-component>

```

Ví dụ, để tạo component có tên là new-cmp, ta chạy lệnh ng g component new-cmp

Ngoài việc tạo ra mới 4 file này, angular CLI cũng giúp chúng ta khai báo new component này cho project trong file app.module.ts

```ts
import { BrowserModule } from '@angular/platform-browser';
import { NgModule } from '@angular/core';

import { AppComponent } from './app.component';
import { NewCmpComponent } from './new-cmp/new-cmp.component';

@NgModule({
  declarations: [
    AppComponent,
    NewCmpComponent, // Dòng này mới được thêm vào
  ],
  imports: [BrowserModule],
  providers: [],
  bootstrap: [AppComponent],
})
export class AppModule {}
```

SD bootstrap dat link css len dau file index.html
Vao link tren url download file js css ve va luu trong assets/css,....

Data binding: Hien thi du lieu

- component => view
- view => component
- 2 chieu

### Component to view

**1. Interpolation: {{}}**
Bien, toan tu 3 ngoi, method

```ts
show() {
    return `Name: ${this.user['name']}`;
}
---
{{ show() }}
<img src="{{link}}"/>>
```

**2. Property: [prop]="value"**
src, href, value, disabled, hidden
Cach 2: bind-prop="value"
**3. Attribute binding**

```ts
[attr.attr_name] = 'value';
```

vd: colspan, href, border, width, height
**4. Class binding**

```ts
[class.ClassName] = "true"
Class css duoc active khi nao
bien kieu: boolean, number, string
[class.label_dangered] = "num === 1"

```

**5. Style binding**

```ts
[style.style_name][style.color] = 'true ? mau 1 : mau 2'[style.fonsize.px] =
  'num';
```

### View to Component

1. Event binding

https://www.w3schools.com/jsref/dom_obj_event.asp
keyup.enter, dbclick, keyup

```ts
(click)="onClick()"

event.target.innerText: ten su kien
```

### Two way binding

Phai Import FormsModule o file app.modules.ts
Cu phap:
[(ngModule)]="name"

Luu y: Neu dat trong the form thi can co:
[ngModelOptions]="{standalone: true}"

### Structural Directive : \*ngIf
