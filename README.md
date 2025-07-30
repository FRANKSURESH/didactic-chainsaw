import requests

# Example payload to simulate Fe-C alloy
payload = {
    "database": "TCFE",
    "elements": {"Fe": 0.92, "C": 0.08},
    "temperature_range": [600, 1600]
}

response = requests.post("https://thermocalcapi.example.com/simulate", json=payload)
print(response.json())
