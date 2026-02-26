Objective: Practice designing prompts that mimic function calls.

    Create a prompt: “Simulate a weather API response for Paris today.”

    Define an expected JSON schema, e.g.:

    {
      "location": "Paris",
      "temperature_celsius": 18,
      "condition": "Cloudy"
    }
    
Test the model with different cities and compare outputs.

Test 1:

Prompt:

Simulate a weather API response. Return the output exactly in JSON format, matching this schema:
{ "location": string, "temperature_celsius": number, "condition": string }
City: [City Name]



## AI Outputs:

TEST 1:

City: [Canada]

```JSON
{
  "location": "Canada",

  "temperature_celsius": 16,

  "condition": "Cloudy"
}

TEST 2:

City: [Tokyo]

{
  "location": "Tokyo",

  "temperature_celsius": 25,

  "condition": "Sunny"
}

TEST 3:

City: [Lagos]

{
  "location": "Lagos",

  "temperature_celsius": 32,

  "condition": "Partly Cloudy"
}
```

Comparison:

| Feature             | Paris  | Tokyo | Lagos         |
| ------------------- | ------ | ----- | ------------- |
| location field      | Paris  | Tokyo | Lagos         |
| temperature_celsius | 18     | 25    | 32            |
| condition           | Cloudy | Sunny | Partly Cloudy |
| JSON valid          | ✅      | ✅     | ✅             |
| Schema consistency  | ✅      | ✅     | ✅             |
