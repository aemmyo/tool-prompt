# Objective: Combine multiple prompts to simulate a tool-using agent.

### Step 1 prompt: Ask for a user’s query (e.g., “What’s the temperature in Paris?”).

## What’s the temperature in Lagos today?

### Step 2 prompt: Simulate a call to the weather API.

{

"location": string,

"temperature_celsius": number,

"condition": string

}

City: Lagos

```JSON
{
  "location": "Lagos",

  "temperature_celsius": 31,

  "condition": "Partly Cloudy"

}
```
### Step 3 prompt: Format the final answer back to the user.

The current temperature in Lagos is 31°C, with partly cloudy weather conditions.

### Document the chained process and outputs.

 | Step   | Function           | Output Type      |
| ------ | ------------------ | ---------------- |
| Step 1 | Understand request | Structured text  |
| Step 2 | Tool simulation    | JSON data        |
| Step 3 | User response      | Natural language |
