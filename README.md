# OBBJECT in js
>Compare it with a cup, for example. A
cup is an object, with properties. A cup
has a color, a design, weight, a material
it is made of, etc. The same way,
JavaScript objects can have properties,
which define their characteristics.


# Description
>Nearly all objects in JavaScript are instances of Object; a typical object inherits properties (including methods) from Object.prototype, although these properties may be shadowed (a.k.a. overridden). The only objects that don't inherit from Object.prototype are those with null prototype, or descended from other null prototype objects.

Changes to the Object.prototype object are seen by all objects through prototype chaining, unless the properties and methods subject to those changes are overridden further along the prototype chain. This provides a very powerful although potentially dangerous mechanism to override or extend object behavior. To make it more secure, Object.prototype is the only object in the core JavaScript language that has immutable prototype — the prototype of Object.prototype is always null and not changeable.


# delete
>There isn't any method in an Object itself to delete its own properties (such as Map.prototype.delete()). To do so, one must use the delete operator.

# method keys
>Object.keys() creates an array containing the keys of an object.

We can create an object and print the array of keys.
>// Initialize an object
const employees = { <br>
	boss: 'Michael',
	secretary: 'Pam',
	sales: 'Jim',
	accountant: 'Oscar'
};

// Get the keys of the object
const keys = Object.keys(employees);

console.log(keys);
>
>
>As Object.keys converts your object’s keys into an array of keys, the forEach() array method can be used to iterate through the keys and values.

# method entries
>Object.entries() creates a nested array of the key/value pairs of an object.
>// Initialize an object <br>
const operatingSystem = { <br>
    name: 'Ubuntu', <br>
    version: 18.04, <br>
    license: 'Open Source' <br>
};

// Get the object key/value pairs
const entries = Object.entries(operatingSystem);

console.log(entries);
>
>Once we have the key/value pair arrays, we can use the forEach() method to loop through and work with the results.
>
>The Object.entries() method will only return the object instance’s own properties, and not any properties that may be inherited through its prototype


# method value
>Object.values() creates an array containing the values of an object.

>// Initialize an object <Br>
const session = { <br>
    id: 1,  <br>
    time: `26-July-2018`, <br>
    device: 'mobile', <br>
    browser: 'Chrome' <br>
};

// Get all values of the object
const values = Object.values(session);

console.log(values);


# this
>In JavaScript, the this keyword refers to an object.

Which object depends on how this is being invoked (used or called).

The this keyword refers to different objects depending on how it is used:
>
>
In an object method, this refers to the object.
Alone, this refers to the global object.
In a function, this refers to the global object.
In a function, in strict mode, this is undefined.
In an event, this refers to the element that received the event.
Methods like call(), apply(), and bind() can refer this to any object.
# this is not a variable. It is a keyword. You cannot change the value of this.

>When used in an object method, this refers to the object.

In the example on top of this page, this refers to the person object.

Because the fullName method is a method of the person object.# lecture_5
