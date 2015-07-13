# amber-branding-widget
Version reporting and amber project linkback widget

<h1>How to use</h1>
In after your amber initialize call. Call either 

* amber.globals._begin() 
* amber.globals.\_begin_ ('Your messaage')

That will insert the branding widget into to page.

Next call your main widget to be inserted into the page.

```
  <script type='text/javascript'>
      require(['app'], function (amber) {
          amber.initialize({
            //used for all new packages in IDE
            'transport.defaultAmdNamespace': "amber-demo"
          });
          amber.globals.DemoHeader._begin_('The ProfStef Example, ');
          amber.globals.TrySmalltalkWidget._open();
      });
  </script>
  ```
