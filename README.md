# Freechains-Node

The file Main.js creates a client to use in conjunction with the Freechains server. With a version of Node installed in your local device you can run the program by typing:

~~~shell
nodejs Main.js "freechains command"
~~~

As an example you can retrive an encrypted shared key using freechains by typing:

~~~shell
nodejs Main.js freechains crypto shared teste
~~~

Main.js can also be used as an module in a javascript application. It exports the main function contained within the module.

The next example demonstrates how to call a Freechains command using Main.js. 

~~~javascript
const Main = require("./Main");

Main.main(["freechains", "crypto", "shared", "teste"]);
~~~
