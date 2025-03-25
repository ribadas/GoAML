goAML Suspicious Transaction Report Visualization
Summary
This project creates an interactive visualization of a goAML Suspicious Transaction Report (STR) in XML format, as specified by the Zoll goAML schema (fiu_goaml_handbuch_anlage2_entwurf.pdf). The visualization is an expandable tree structure displayed in a web browser, with the following features:

Expandable Tree: Users can expand/collapse nodes to explore the report's structure.
Tooltips on Hover: Hovering over a field displays a tooltip with the field's description.
Lookup Values on Click: Clicking a field displays its possible values (if applicable), including both the code and description, as defined in Section 5 of the goAML XML Reporting Schema Description v4.0.
The project addresses the following requirements:

Added a missing <activity> node to the goAML XML to describe the suspicious activity, linking transactions and involved parties.
Built a dictionary (fieldDictionary) of all fields in the XML, with descriptions and lookup values (code and description) sourced from the goAML schema documentation.
Updated the HTML/JavaScript to display field descriptions on hover and lookup values on click in a formatted list.
The final code includes a comprehensive fieldDictionary covering all fields in the XML, with lookup values for enumerated fields like report_type, account_type, id_type, etc. The visualization ensures compliance with goAML schema rules (e.g., mutual exclusivity of t_to, t_to_my_client, and t_to_my_account in transactions).


