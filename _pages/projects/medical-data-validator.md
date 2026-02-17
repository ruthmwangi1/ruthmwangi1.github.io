---
title: "Medical Data Validator-Python Program"
layout: single
permalink: /projects/medical-data-validator/
search: true
---

This is a Python program meant to validate medical records based on the following set of rules. 
- The data type should be a list or a tuple.
- Each patient's records should be in dictionary format.
- All dictionaries must have all the predetermined keys.
- The values in the dictionaries should follow specific formats.
  For instance, patient id should be in a string format and it should begin with letter "p" followed by one or more numbers,
  The gender should be either male or female, last_visit_id should start with letter v followed by one or more numbers,
  Medications should follow the list format etc.
If the data is invalidated, the different causative messages are printed in the output. Otherwise, "Valid Format" is printed as the output.

