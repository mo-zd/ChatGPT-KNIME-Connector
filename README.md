# ChatGPT-KNIME Connector

The ChatGPT-KNIME Connector is a Python package that allows you to integrate OpenAI's ChatGPT and KNIME Analytics Platform for drug design research. It includes functions for generating molecules with ChatGPT and screening them with a KNIME workflow, as well as a function for outputting data to KNIME.

![chat-gpt](https://user-images.githubusercontent.com/91246296/221000655-d7ae7c48-73a0-467a-9bcd-35b2fdafdcdf.png)

## Requirements

    Python 3
    OpenAI API key
    KNIME Analytics Platform
    Molecule Screening workflow in KNIME

Installation

1. Clone the repository to your local machine.
2. Install the required packages with pip install -r requirements.txt.

Usage

3. Import the package in your Python script with import ChatGPT_KNIME_Connector.
4. Set your OpenAI API key with openai.api_key = "YOUR_API_KEY".
5. Call the generate_molecules() function to generate a list of molecules based on a starting sequence.
6. Call the screen_molecules() function to screen the generated molecules with a KNIME workflow.
7. Call the knime_output() function to output the screened molecules back to KNIME.

Here is an example code snippet:

```python

import ChatGPT_KNIME_Connector
import pandas as pd

# Set your OpenAI API key
openai.api_key = "YOUR_API_KEY"

# Generate molecules with ChatGPT
molecules = ChatGPT_KNIME_Connector.generate_molecules('C')

# Screen molecules with KNIME
screened_molecules = ChatGPT_KNIME_Connector.screen_molecules(molecules)

# Output data to KNIME
ChatGPT_KNIME_Connector.knime_output(screened_molecules)
```
## Credits

The ChatGPT-KNIME Connector package was created by Mohsen Yazdani.

## Contributing

If you find any bugs or would like to contribute to the development of the ChatGPT-KNIME Connector, please open an issue or a pull request on this repository.

## License

This package is released under the MIT license. See LICENSE for more information.
