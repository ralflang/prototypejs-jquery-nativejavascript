# Convert ancient PrototypeJS or jQuery code to Native Javascript

Cheat Sheet and more elaborate conversion from PrototypeJs and jQuery to Native Javascript.

| Capability | PrototypeJs | jQuery | Javascript | Comment |
| ---------- | ----------- | ------ | ---------- | ------- |
| Select single Element by ID string | $('EltId') | $( "#EltId" ) | document.getElementById('EltId') or document.querySelector('#EltId')  or document.querySelector('[id="EltId"]')| getElementById is the oldest option |
