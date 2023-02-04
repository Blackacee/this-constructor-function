# this-constructor-function

function Cat(name) {
 this.name = name;
 this.sound = "Meow";
}
var cat = new Cat("Tom"); // is a Cat object
cat.sound; // Returns "Meow"
var cat2 = Cat("Tom"); // is undefined -- function got executed in global context
window.name; // "Tom"
cat2.name; // error! cannot access property of undefined
