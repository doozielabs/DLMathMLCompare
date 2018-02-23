# DLMathMLCompare
You can use this library to compare two MathML expressions

 1. Install via `npm install dl-mathml-compare`
 2. Require in your code using `var DLMathMLCompare = require('dl-mathml-compare');`
 3. Use in your code as `DLMathMLCompare('Your MathML expression here', 'Your another MathML expression');`
 4. It will return `true` if matched otherwise returns `false`
 5. Does styling insensitive MathML comparison

**Example:**

```JS
DLMathMLCompare('<math xmlns="http://www.w3.org/1998/Math/MathML"><mfrac><mn>1</mn><mrow><mn>2</mn><msqrt><mo>&#xA0;</mo></msqrt><mo>&#xA0;</mo></mrow></mfrac></math>', '<math xmlns="http://www.w3.org/1998/Math/MathML"><mfrac><mn>1</mn><mrow><mn>2</mn><msqrt/><mo>&#xA0;</mo></mrow></mfrac><mo>&#xA0;</mo><mo>&#xA0;</mo> </math> ');
// This will return true
```