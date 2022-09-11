---
sidebar_position: 2
#
# This file is autogenerated. DO NOT MODIFY DIRECTLY
#
---

import ScriptEventPreview from '@site/src/components/ScriptEventPreview';

# Sterowanie

## Przycisk Joypad: przypisz skrypt
Run the specified script any time a joypad button is pressed.
<ScriptEventPreview title={"Przycisk Joypad: przypisz skrypt"} fields={[{"key":"input","label":"Button","description":"The joypad button to check.","type":"input","defaultValue":["b"]},{"key":"override","type":"checkbox","label":"Nadpisz domyślny przycisk akcji","description":"Set if the script should replace the default game action for the specified button.","defaultValue":true},{"key":"__scriptTabs","type":"tabs","defaultValue":"press","values":{"press":"Na naciśnięcie"}},{"key":"true","label":"Na naciśnięcie","description":"The script to run when the button is pressed.","type":"events","allowedContexts":["global","entity"],"conditions":[{"key":"__scriptTabs","in":[null,"press"]}]}]} />

- **Button**: The joypad button to check.  
- **Nadpisz domyślny przycisk akcji**: Set if the script should replace the default game action for the specified button.  
- **Na naciśnięcie**: The script to run when the button is pressed.  

## Warunek: naciśnięty przycisk joypada
Conditionally run part of the script if the specified joypad button is currently pressed. Will not wait for user input and will only execute once, if you wish to run a script every time a button is pressed use Attach Script To Button instead.

**Odniesienia**  
[/docs/scripting/script-glossary/input#attach-script-to-button](/docs/scripting/script-glossary/input#attach-script-to-button)  
<ScriptEventPreview title={"Warunek: naciśnięty przycisk joypada"} fields={[{"key":"input","label":"Każde z","description":"The input buttons to check.","type":"input","defaultValue":["a","b"]},{"key":"true","label":"Prawda","description":"The script to run if the condition is true.","type":"events"},{"key":"__collapseElse","label":"W innym wypadku","type":"collapsable","defaultValue":true,"conditions":[{"key":"__disableElse","ne":true}]},{"key":"false","label":"Fałsz","description":"The script to run if the condition is false.","conditions":[{"key":"__collapseElse","ne":true},{"key":"__disableElse","ne":true}],"type":"events"}]} />

- **Każde z**: The input buttons to check.  
- **Prawda**: The script to run if the condition is true.  
- **Fałsz**: The script to run if the condition is false.  

## Przycisk Joypad: czekaj na przycisk
Pauses the script until one of the specified joypad buttons are pressed.
<ScriptEventPreview title={"Przycisk Joypad: czekaj na przycisk"} fields={[{"key":"input","label":"Każde z","description":"The input buttons to check.","type":"input","defaultValue":["a","b"]}]} />

- **Każde z**: The input buttons to check.  

## Przycisk Joypad: usuń przypisany skrypt
Remove an attached script from a joypad button restoring the default functionality of the button.
<ScriptEventPreview title={"Przycisk Joypad: usuń przypisany skrypt"} fields={[{"key":"input","label":"Usuń skrypt dołączony do wykonania","description":"The joypad button to remove the attached script from.","type":"input","defaultValue":["b"]}]} />

- **Usuń skrypt dołączony do wykonania**: The joypad button to remove the attached script from.  
