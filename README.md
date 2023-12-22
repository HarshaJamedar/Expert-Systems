E-Garage: Expert System for Electronic Devices Recommendations

Overview:

E-Garage is an expert system designed to assist users in selecting electronic devices based on their preferences and budget. This system recommends mobile phones, tablets, and laptops by asking users questions and offering suitable options.

Features:

•	Device Recommendations: Recommends devices based on user inputs regarding device type, price range, and preferred company.
•	Device Categories: Supports mobile phones, tablets, and laptops.
•	Budget-Friendly Suggestions: Provides options within various price ranges.
•	Company Preferences: Considers user-preferred brands while suggesting devices.

How to Use:
Launch the System: Run the system using the specified programming language and environment (e.g., CLIPS).

Input Preferences: Answer system queries about device type, price range, and preferred companies.
Get Recommendations: Receive recommendations based on your input.

Getting Started

Prerequisites:
CLIPS Programming Environment
Installation
Open the CLIPS environment.
Load the project files into CLIPS.
Execute the system by running (reset) and (run) commands.

Contributors:
Harshavardhan Jemedar
Priya Keshri









WORKFLOW:

In the provided CLIPS project file, the data flow begins with user inputs and progresses through a series of rules matching user preferences to suggest the appropriate electronic device. Here's a detailed breakdown of the data flow after the user provides inputs:

1. User Input Collection
   - The system prompts the user for the device they want to purchase: mobile, tablet, or laptop.
   - Once the device type is selected, the system asks for the preferred price range based on the selected device type.
   - Following the price range input, the system asks for the preferred company or brand of the device.

2. Rule Matching Based on User Inputs
   - Rules in the system (e.g., `buy_mobile`, `buy_tablet`, `buy_laptop`) match the user inputs against predefined conditions.
   - For instance, if the user selects a mobile phone with a price range above $1000 and prefers Apple, the `mob_apple_above1000$` rule is triggered.

3. Suggested Device Generation
   - Once a rule matches the user's inputs, it triggers actions to suggest suitable devices.
   - The suggestion action (`put-suggested_device`) assigns a string containing recommended device names and prices to the `[which_device]` object.

4. Final Recommendation Output
   - At the end of the rule execution, a final rule (`choose_device`) is triggered, which prints the suggested device(s) based on the matched criteria.
   - The system generates output in a format that shows the recommended device(s) that best suit the user's preferences.

Example Flow:

1. User inputs:
   - Device type: Mobile
   - Price range: above1000$
   - Preferred company: Apple

2. The system matches these inputs against the rules (`mob_apple_above1000$`) and triggers the rule.

3. The rule action generates suggested devices:
   - Suggested devices for Apple mobile phones above $1000.

4. The final recommendation is printed in the desired format.

 Data Flow Summary:

- User inputs -> Rule matching based on inputs -> Suggested device generation -> Final recommendation output

Each step in the process involves matching the user's preferences with predefined rules and generating device suggestions accordingly. The flow ends with a clear recommendation based on the user's input criteria.

Learning Outcomes:

-Learn CLIPS Features: Understand and experiment with various features, functionalities, and constructs within CLIPS, such as defining classes (defclass), creating instances (dev instances), defining rules (default), and managing data flow.

-  Develop an expert system that recommends electronic devices (mobiles, tablets, laptops) based on user-defined criteria.

- Explore the rule-based decision-making process using CLIPS, where user inputs drive the selection of suitable devices by matching against predefined rules.
