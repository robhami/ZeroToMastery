# ZeroToMastery

### Inline script ###

Initially used in inline scripts: 

e.g. 

```
<script type ="text/javascript">
  function a() {
    alert('a')
  }
  
   function b() {
    alert('b')
  }
  
   function c() {
    alert('c')
  }
  </script>
  ```
  
  Issues: 
  
  1. Lack of code reusability- have to retype each time 
  2. Pollution of Global Namespace- e.g. once I use 'a' as a variable in window object, can never use it again
  
  ### Script tags ref separate files ###
  
  Issues:
  1. Every page needs tags at top
  2. Lack of dependency resolution- u r responsible to make sure script added in correct order 
  (e.g. if later entered tag has function called in earlier tag it wont work)
  3. Pollutes Global Namespace still- as all in window object still
  
  
  ### Immediately Invoked Function Execution ###