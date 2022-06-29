1.Explain difference between Props and State ?

<table>
  <thead>
  <tr>
  <td>Props<td>
  <td>State</td>
  </tr>
  </thead>
  <tbody>
  <tr>
    <td>The Data is passed from one component to another.</td>
    <td>The Data is passed within the component only.</td>
  </tr>

  <tr>
    <td>It is Immutable (cannot be modified).</td>
    <td>It is Mutable ( can be modified)</td>
  </tr>

  <tr>
    <td>Props can be used with state and functional components.</td>
    <td>State can be used only with the state components/class component</td>
  </tr>

  <tr>
    <td>Props are read-only.</td>
    <td>State is both read and write.</td>
  </tr> 
  </tbody>
</table>

2.What is useState Api ?

<p>
-useState is a Hook that allows you to have state variables in functional components. You pass the initial state to this function and it returns a variable with the current state value (not necessarily the initial state) and another function to update this value
</p>
3.Create your own map, filter, reducer methods and attach it to an array using prototype chain .

<h3>Map:</h3>
<p>map is a method built to do exactly that. It's defined on Array.prototype, so you can call it on any array, and it accepts a callback as its first argument</p>
<h5>Example for map:</h5>
<p>let newArray = arr.map(callback(currentValue[, index[, array]]) {
  // return element for newArray, after executing something
}[, thisArg]);</p>

<h3>Filter:</h3>
<p>The next of our array operations is filter. It does exactly what it sounds like: It takes an array and filters out unwanted elements.</p>
<h5>Example for filter:</h5>
<p>let newArray = arr.filter(callback(currentValue[, index[, array]]) {
  // return element for newArray, if true
}[, thisArg]);</p>

<h3>Reducer:</h3>
<p>map creates a new array by transforming every element in an array individually. filter creates a new array by removing elements that don't belong. reduce, on the other hand, takes all of the elements in an array and reduces them into a single value</p>
<p>Just like map and filter, reduce is defined on Array.prototype and so is available on any array, and you pass a callback as its first argument. But it also takes a second argument: the value to start combining all your array elements into. </p>
<h5>Example for reduce:</h5>
<p>const total = [1, 2, 3, 4, 5].reduce((previous, current) => previous+current),0;
console.log(total) // 15</p>
