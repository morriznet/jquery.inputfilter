#jquery.inputfilter

jQuery plugin for adding filters to forms input and textarea, like numeric input only.

##Demo
[Simple demo](http://www.morriz.net/demo/jquery.inputfilter/examples/Index.html)

##Usage
Include *jquery.inputfilter.js* after jQuery (1.7+) and set it to the objects you want to filter
```
<form>
    <input type="text" />
    <textarea></textarea>
</form>
<script src="jquery.js"></script>
<script src="jquery.inputfilter.js"></script>
<script>
    //Standard options
    $("input, textarea").inputfilter();
    //Set options
    var options = {allowNumeric: true, allowText: true}
    $("input, textarea").inputfilter(options);
</script>
```

##Options
```
var options = {
    allowNumeric: true, // is numbers allowed [0-9]
    allowText: false,   // is text allowed [a-z|A-Z]
    allowEnter: true,   // is Enter allowed
    allowCustom: [],    // Array of chars to allow
    regex: null,        // Regular expression of allowed chars
    maxLength: null,    // Numeric value representing the maximum number of chars permitted
    actionLog: false    // Log actions
}
```

##License
Copyright &copy; 2015 Anders Fj&auml;llstr&ouml;m, licensed under the MIT License 

