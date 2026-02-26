# Objective: Create prompts that produce structured machine-readable output.

> Write a prompt that asks for unstructured information (e.g., “List three cities with their populations.”).

Rewrite the prompt to enforce structured JSON output:

Example: “Return the following in JSON format: [{city: string, population: number}].”
## Example:
### Extract applicant details from this text;
“My name is Emmanuel Ayegba. I am 26 years old and live in Abuja. I apply for the Data Entry Officer position.”

Extract the following fields from the text and return ONLY valid JSON format:
{name: string, age: number, location: string, position: string}
```JSON
{
  "name": "Emmanuel Ayegba",
  "age": 26,
  "location": "Abuja",
  "position": "Data Entry Officer"
}
```
## Test with multiple inputs and verify the JSON stays valid.

## Test 1:

A smart city receives sensor messages like:

“Sensor A12 detected temperature 34°C at Ikeja at 14:05.”

Extract the following fields and return valid JSON only:

{sensor_id: string, temperature: number, location: string, time: string}
```JSON
{
  "sensor_id": "A12",
  "temperature": 34,
  "location": "Ikeja",
  "time": "14:05"
}
```
Test 2:

“Patient Mary Okafor, age 45, complains of chest pain.”

Extract patient information and return JSON:
{name: string, age: number, symptom: string}
```JSON
{
  "name": "Mary Okafor",
  "age": 45,
  "symptom": "chest pain"
}
```