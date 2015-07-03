# generator-angular-crud-custom-module

> generator-angular-crud-custom-module is basically [Yeoman](http://yeoman.io) generator,which generate controller,services and view files of given module. To generate dynamic form from given fields of module, we used [angular formly](http://docs.angular-formly.com/).

## Getting Started

To use generator-angular-curd-custom-module generator, please go through below steps.
<ol>
    <li> Install ``yo``.
        <br>
        <pre>
        npm install -g yo
        </pre>
        </li>
    <li> Install `generator-angular-crud-custom-module` from npm.
        <br>
        <pre>
        npm install -g generator-angular-crud-custom-module
        </pre>
        </li>
    <li> To initiate the generator, create a new folder and change terminal directory to the folder, Run:
        <br>
        <pre>
        yo generator-angular-crud-custom-module
        </pre>
        This command will generate following items:
        <ul>
            <li>app
                <ul>
                    <li>modules</li>
                    <ul>
                        <li>common</li>
                         <ul>
                            <li>assets</li>
                            <li>directives.js</li>
                            <li>filters.js</li>
                            <li>startUpController.js</li>
                         </ul>
                    </ul>
                    <li>vendor</li>
                    <li>app.js</li>
                    <li>index.html</li>
                </ul>
            </li>
            <li>gulp</li>
            <li>.bowerrc</li>
            <li>bower.json</li>
        </ul>
        </li>
    <li> To create dynamic module, run:
        <br>
        <pre>
        yo angular-crud-custom-module:module
        </pre>
        This will asked you couple of questions.Like module name,path to generate it and fields of the module. After applying this command, controllers,services and view files of this module will be generated and generated items:
        <br>Lets take `customer` as module
        <ul>
            <li>customer
                <ul>
                    <li>views</li>
                    <ul>
                        <li>customers.html</li>
                        <li>addCustomer.html</li>
                        <li>editCustomer.html</li>
                        <li>deleteCustomer.html</li>
                    </ul>
                    <li>customerController.js</li>
                    <li>customerServices.js</li>
                </ul></li></ul></li><ol>
If you want to add more modules,then repeat step 4.

## Example

Lets create `Customer contact` application for your organization,in which you can maintain `customers` and `employees` information.Create a new folder and apply below steps:

<pre>
npm install -g yo
npm install -g generator-angular-crud-custom-module
yo angular-crud-custom-module
</pre>
Last command will asked you application name, so lets give it as `customerContactApp`
<pre>
yo angular-crud-custom-module:module
</pre>
Please refer below image for reference:

![alt text](https://github.com/ShivaliPatel/generator-angular-crud-custom-module/blob/master/images/createModule.png)

So,your customer contact application is created within 10 minutes.

## Output
### Customers list
![alt text](https://github.com/ShivaliPatel/generator-angular-crud-custom-module/blob/master/images/customers.png)
### Add Customer
![alt text](https://github.com/ShivaliPatel/generator-angular-crud-custom-module/blob/master/images/addCustomer.png)
### Edit Customer
![alt text](https://github.com/ShivaliPatel/generator-angular-crud-custom-module/blob/master/images/updateCustomer.png)
### Delete Customer
![alt text](https://github.com/ShivaliPatel/generator-angular-crud-custom-module/blob/master/images/deleteCustomer.png)

## Generated files
### app.js
![alt text](https://github.com/ShivaliPatel/generator-angular-crud-custom-module/blob/master/images/appJs.png)
### controller.js
![alt text](https://github.com/ShivaliPatel/generator-angular-crud-custom-module/blob/master/images/controllerJs.png)
### services.js
![alt text](https://github.com/ShivaliPatel/generator-angular-crud-custom-module/blob/master/images/servicesJs.png)

## Note

Here,add/update form is generated by `angular formly`. So if you want to add extra fields that are not provided in this generator,then add it manually to controller file of that module.
## License

MIT
