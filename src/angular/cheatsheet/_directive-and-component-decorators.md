<table id="class-field-decorators">

<tr>
  <th>Class field decorators for directives and components</th>
  <th markdown="1">
  `import 'package:angular/angular.dart';`
  </th>
</tr>

<tr>
  <td class="nowrap"><code class="prettyprint lang-dart">
    <b>@Input()</b> myProperty;
  </code></td>
  <td markdown="1">
  Declares an input property that you can update via property binding (example:
  `<my-cmp [myProperty]="someExpression">`).

  See: [Template Syntax](/angular/guide/template-syntax),
  [Input class](/api/angular/angular/Input-class)
  </td>
</tr>

<tr>
  <td class="nowrap"><code class="prettyprint lang-dart">
    final _myEvent = new StreamController&lt;T>();<br>
    <b>@Output()</b> Stream&lt;T> get myEvent => _myEvent.stream;
  </code></td>
  <td markdown="1">
  Declares an output property that fires events that you can subscribe to with an event binding (example: `<my-cmp (myEvent)="doSomething()">`).

  See: [Template Syntax](/angular/guide/template-syntax),
  [Output class](/api/angular/angular/Output-class)
  </td>
</tr>

<tr>
  <td class="nowrap"><code class="prettyprint lang-dart">
    <b>@HostBinding('class.valid')</b> isValid;
  </code></td>
  <td markdown="1">
  Binds a host element property (here, the CSS class `valid`) to a directive/component property (`isValid`).

  See: [HostBinding class](/api/angular/angular/HostBinding-class)
  </td>
</tr>

<tr>
  <td class="nowrap"><code class="prettyprint lang-dart">
    <b>@HostListener('click', ['$event'])</b><br>
    onClick(e) {...}
  </code></td>
  <td markdown="1">
  Subscribes to a host element event (`click`) with a directive/component method (`onClick`), optionally passing an argument (`$event`).

  See: [Attribute Directives](/angular/guide/attribute-directives),
  [HostListener class](/api/angular/angular/HostListener-class)
  </td>
</tr>

<tr>
  <td class="nowrap"><code class="prettyprint lang-dart">
    <b>@ContentChild(myPredicate)</b> myChildComponent;
  </code></td>
  <td markdown="1">
  Binds the first result of the component content query (`myPredicate`) to a property (`myChildComponent`) of the class.

  See: [ContentChild class](/api/angular/angular/ContentChild-class)
  </td>
</tr>

<tr>
  <td class="nowrap"><code class="prettyprint lang-dart">
    <b>@ContentChildren(myPredicate)</b> myChildComponents;
  </code></td>
  <td markdown="1">
  Binds the results of the component content query (`myPredicate`) to a property (`myChildComponents`) of the class.

  See: [ContentChildren class](/api/angular/angular/ContentChildren-class)
  </td>
</tr>

<tr>
  <td class="nowrap"><code class="prettyprint lang-dart">
    <b>@ViewChild(myPredicate)</b> myChildComponent;
  </code></td>
  <td markdown="1">
  Binds the first result of the component view query (`myPredicate`) to a property (`myChildComponent`) of the class. Not available for directives.

  See: [ViewChild class](/api/angular/angular/ViewChild-class)
  </td>
</tr>

<tr>
  <td class="nowrap"><code class="prettyprint lang-dart">
    <b>@ViewChildren(myPredicate)</b> myChildComponents;
  </code></td>
  <td markdown="1">
  Binds the results of the component view query (`myPredicate`) to a property (`myChildComponents`) of the class. Not available for directives.

  See: [ViewChildren class](/api/angular/angular/ViewChildren-class)
  </td>
</tr>

</table>
