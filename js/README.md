##How to use FlyJSONP?

First include the script, preferably just before the body tag, call init to setup initial options. Then just call get or post methods.

```javascript
<script src="/path/to/flyjsonp.js"></script>
<script>
FlyJSONP.init({debug: true});
//For GET operation
FlyJSONP.get({
  url: 'http://storify.com/xdamman.json',
  success: function(data) {
    console.log(data);
  },
  error: function(errorMsg) {
    console.log(errorMsg);
  }
});

//For POST operation
FlyJSONP.post({
  url: 'http://storify.com/story/new',
  parameters: {
    username: 'your-username',
    api_key: 'secret-api-key',
    title: 'FlyJSONP',
    description: 'Testing it out'
  },
  success: function(data) {
    console.log(data);
  }
});
</script>
```    
