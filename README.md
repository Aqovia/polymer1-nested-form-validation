# Web Components - Nested Form Validation Samples

This repository is for highlighting how various JavaScript frameworks/libraries handle form validation when using nested validatable Web Components (Custom Elements).

Although one of the early use cases of Custom Elements has been the creation of form input fields, they actually [do not work well in native HTML Forms](https://github.com/w3c/webcomponents/issues/187). The early solution to this is Polymer's [`<iron-form>`](https://www.webcomponents.org/element/@polymer/iron-form), but this is not always intuitive - in particular we faced a'gotcha' that nested components were not included in form validation unless the intermediate components called the `validate()` method on their children. Using `<iron-form>` also imposes the overhead of the Polymer library when we are moving on to lighter-weight base classes, such as [lit](https://lit-element.polymer-project.org/).

Pull requests adding examples of other frameworks / approaches are welcome, provided they demonstrate an implementation of the same nesting use case using Custom Elements.
