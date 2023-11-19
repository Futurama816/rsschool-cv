# David Mdzinarishvili
## contact info
 * Telephone: 599 49 55 05
 * E-Mail: DMsaqartvelo@gmail.com
## About Me
My name is David Mdzinarishvili and I am a Computer Science student who is studying to become a fulll stack web developer.
## Skills
* Knowledgeable in C, C++ and c#
* Knowledgeable in HTML/CSS, Javascript and React 
## Coding Samples 
> const express = require("express");

> const app = express();

> const port = process.env.port || 4000;

> function intValidation(obj, objName, value){//the subject code, experience and lecturer ID should all be integers
>   if (Number.isInteger(value)) {
>       obj[objName] = value
>   } else {
>      throw new Error(`${objName} should be an integer.`)
>   }
> }
> class subject{
>    constructor(name, code, department){
>       this.name = name
>       intValidation(this, 'code', code)// numerical code for the class
>       this.department = department
>   }
>   getDetails(){`Name: ${this.name}, Code: ${this.code}, department: ${this.department}`;}
> }
> class Lecturer{
>   constructor(lastName, firstName, track, department, experience, lecturerID){
>       this.lastName = lastName
>        this.firstName = firstName
>       this.track = track/* assuming the university follows the American system the tracks would be part-time adjunct,
>       full time adjunct, tenure track, fully tenured along with guest lecturers*/
>       this.department = department
>       intValidation(this, 'experience', experience)//experience is in years
>       intValidation(this, 'lecturerID', lecturerID)
>   }

>   getDetails(){return `Last Name: ${this.lastName}, First Name: ${this.firstName}, Track: ${this.track}, Department: ${this.department}, Experience:
>     ${this.experience} years, ID: ${this.lecturerID}`;}
> }

> const introToStats = new subject ("Introduction to Statistics", 21101, "math")
> const calcII = new subject ("Calculus II", 21232, "math")
> const medivalIslam = new subject ("The Islamic Golden Ages: from the 7th to 13th century", 46202, "history")

> const profI = new Lecturer("Hoffman", "Mordecai", "full time adjunct", "math", 5, 578320)
> const profII = new Lecturer("Grim", "Noah", "guest", "history", 0, 201896)

> function assignSubjects(lecturer, subject){
>    lecturer.subjects = lecturer.subjects || [] // creates an array of subjects for each lecturer
>   lecturer.subjects.push(subject)
> }

> function getSubjects(lecturer) {
>   if (lecturer.subjects && lecturer.subjects.length > 0) {
>     return lecturer.subjects.map(subject => subject.name);
>   } else {
>     return "No subjects assigned yet.";
>   }
> }

> assignSubjects(profI, introToStats);
> assignSubjects(profI, calcII);
> assignSubjects(profII, medivalIslam);
 
> console.log(getSubjects(profI));
> console.log(getSubjects(profII));
>

## Experience
* Created and employed SQL and MongoDB databases
* Developed several basic applications in C#, React and Javascript
## Education
* IB diploma from New School of Geogia
* C# certificate
* Currently enrolled in Ilia State university
## Language
* Fluent in both English and Georgian
