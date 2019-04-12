# random-sentence-generator
Random sentence generator web componenet. Built with lit-element

## Usage
```html
<body>
    <random-sentence-generator id="myRandSentence" template="adjective noun verb adverb."></random-sentence-generator>
    
    <script src="dist/random-sentence-generator.iife.js">
</body>
```
Just include the component and use it :)
`template` can be any string. You can use any of the following parts of speech.
 - noun
 - adverb/adv
 - verb
 - interjection
 - adjective/adj
 Any of those keywords will be replaced with randomly generated words.

## Api
Any time the template attribute is changed the sentence will be re-generated. A regeneration can be triggered with
```javascript
document.getElementById('myRandSentence').generate()
```

## Development
Lint with `npm run lint` - uses eslint with standardjs preset

Build with `npm run build` or `npm run watch`. Builds with rollup.
