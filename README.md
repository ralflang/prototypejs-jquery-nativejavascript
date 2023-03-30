# Convert ancient PrototypeJS or jQuery code to Native Javascript

Cheat Sheet and more elaborate conversion from [PrototypeJs](http://prototypejs.org/learn/) and [jQuery](https://jquery.com/) to Native Javascript. Both libraries had their prime time in the days of monolithic javascript written-as-run and have become a liability in many cases. 

## DOM Selection, Traversal and Write Access

| Capability | PrototypeJs | jQuery | Javascript | Comment |
| ---------- | ----------- | ------ | ---------- | ------- |
| Select single Element by ID string | $('EltId') | $( "#EltId" ) | document.getElementById('EltId') or document.querySelector('#EltId')  or document.querySelector('[id="EltId"]')| getElementById is the oldest option |

## Events

### Observing DOM Loaded Event

| Library | Implementation | Comment |
| --- | --- | --- |
| PrototypeJs | document.observe('dom:loaded', function(){ foo; }); | -- |
| jQuery | $(document).ready(function(){ foo; }) ; | Also: $(function(){ foo; }); |
| Native | document.addEventListener('DOMContentLoaded', function () { foo; }, false); | use DOMContentLoaded to wait for the full DOM hierarchy to be constructed or use load for all images and other assets to be loaded first. Usually DOMContentLoaded is what you want |



## Ajaxy stuff

## Array and Object Traversal

## 