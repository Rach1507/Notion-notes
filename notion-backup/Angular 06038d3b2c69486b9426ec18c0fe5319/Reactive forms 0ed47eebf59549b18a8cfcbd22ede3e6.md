# Reactive forms

To achieve all of this, we track the state of each input element and the state of the form itself. Angular has a set of predefined form and input element states. These states define whether the user has changed a value in an input element.

![Untitled](Reactive%20forms%200ed47eebf59549b18a8cfcbd22ede3e6/Untitled.png)

Angular has building blocks that define a form model which tracks all of this state, plus the value of each input element. These building blocks are used by both template‑driven and reactive forms to track state and values

These building blocks are **actually classes** provided when we work with Angular forms. 

Instances of these classes define the form model. 

 **What is a form model exactly?** 

**A** form model is the data structure that represents the HTML form, and it looks like this. The structure of the form model reflects the form and input elements in the template.

![Untitled](Reactive%20forms%200ed47eebf59549b18a8cfcbd22ede3e6/Untitled%201.png)

![Untitled](Reactive%20forms%200ed47eebf59549b18a8cfcbd22ede3e6/Untitled%202.png)

![Untitled](Reactive%20forms%200ed47eebf59549b18a8cfcbd22ede3e6/Untitled%203.png)

when we use the template‑driven approach :

Angular automatically generates the form model by creating the FormGroup and FormControl instances for us, 

and we use ngModel for two‑way binding to keep the user's entries and the data model properties in sync. 

With the reactive forms approach

we define the form model by creating the FormGroup and FormControl instances ourselves in our component class. We then bind the template to the form model. This means that our form is not directly modifying our data model.

## 3 ways of accessing the form

![Untitled](Reactive%20forms%200ed47eebf59549b18a8cfcbd22ede3e6/Untitled%204.png)