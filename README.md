-# Import necessary library
import streamlit as st

# Title of the app
st.title("🌡️ Temperature Converter")

# User input for temperature in Fahrenheit
fahrenheit = st.number_input("Enter temperature in Fahrenheit:", format="%.2f")

# Function to convert Fahrenheit to Celsius
def fahrenheit_to_celsius(fahrenheit):
    celsius = (fahrenheit - 32) * 5 / 9
    return celsius

# Button to trigger conversion
if st.button("Convert to Celsius"):
    celsius = fahrenheit_to_celsius(fahrenheit)
    # Add styled output
    st.markdown(
        f"""
        <div style="background-color: #e8f4f8; padding: 10px; border-radius: 5px; text-align: center;">
            <h4 style="color: #0078a8;">The temperature in Celsius is:</h4>
            <p style="font-size: 20px; font-weight: bold; color: #005f73;">{celsius:.2f} °C</p>
        </div>
        """,
        unsafe_allow_html=True
    )
 👋 Hi, I’m @wajidalipahore
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
wajidalipahore/wajidalipahore is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
