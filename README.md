# tttt-pyats-demo

**_Demo code for pyATS/Genie TTTT - December 2021_**

## Usage

### Installation

Create a Python 3 virtual environment and activate it.
_All testing was done using Python 3.8, but Python 3.7+ should work._

```
python3 -m venv pyats-venv
source pyats-venv/bin/activate
```

With the virtual environment activated, install all the dependencies from requirements.txt

```
pip install -r requirements.txt
```

Lastly, you will need to create a `.env` file in the project root directory with two environment variables for the device login credentials (username and password). For testing purposes, I used the variable names `EVE_USER` and `EVE_PASS` since I used EVE-NG to virtually simulate my test network.

```
EVE_USER=<your username>
EVE_PASS=<your password>
```

If you would like to use different variable names, please make sure to update the appropriate script files. More specifically, the Scrapli inventory file (`scrapli_inv.py`) and the Genie parser file (`genie_parse.py`). You'll need to make sure the scripts look for the new environment variable names.

## Contribution

As most of this repository contains introductory demo code, there are definitely ways to improve the code (i.e. error handling, improving modularity, etc.). Please feel free to make a pull request with whatever changes you find would help improve the content!

## Feedback

If you have any questions or would like to provide further feedback, please feel free to message me or open an issue. Thanks!
