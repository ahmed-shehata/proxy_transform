# proxy_transform
Spark AR Helper: Modify a given SceneObject’s transform properties to match a given proxy SceneObject depending on the screen orientation (landscape or portrait).

# Usage example 
Check out Spark AR example project

```const Scene = require('Scene');
var ProxyTrans = require('./proxyTransform.js');


var h_proxy = Scene.root.find("h_proxy");
var v_proxy = Scene.root.find("v_proxy");
var myObject = Scene.root.find('myObject');

// Change myObject's transfrom properties to match a proxy object, depending on the screen orientation.
ProxyTrans.MoveTo(myObject, v_proxy, h_proxy);
