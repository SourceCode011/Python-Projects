# face_recognition_project

<!-- 
Pip install opencv
Pip install Pandas
Pip install Streamlit
Pip install Scikit-learn
Pip install pywin32
Pip install Streamlit-autofresh
 -->

<!--
Windows PowerShell
Copyright (C) Microsoft Corporation. All rights reserved.

Install the latest PowerShell for new features and improvements! https://aka.ms/PSWindows
PS G:\Other computers\My Desktop PC\Documents\Python-Projects\face_recognition_project-main> pip install opRequirement already satisfied: opencv-python in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (4.9.0.80)
Requirement already satisfied: numpy>=1.21.2 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from opencv-python) (1.26.4)

[notice] A new release of pip is available: 23.2.1 -> 24.0
[notice] To update, run: python.exe -m pip install --upgrade pip
PS G:\Other computers\My Desktop PC\Documents\Python-Projects\face_recognition_project-main> pip install csv
ERROR: Could not find a version that satisfies the requirement csv (from versions: none)
ERROR: No matching distribution found for csv

[notice] A new release of pip is available: 23.2.1 -> 24.0
[notice] To update, run: python.exe -m pip install --upgrade pip
PS G:\Other computers\My Desktop PC\Documents\Python-Projects\face_recognition_project-main> pip install sklearn
Collecting sklearn
  Downloading sklearn-0.0.post12.tar.gz (2.6 kB)
  Installing build dependencies ... done
  Getting requirements to build wheel ... error
  error: subprocess-exited-with-error

  × Getting requirements to build wheel did not run successfully.
  │ exit code: 1
  ╰─> [15 lines of output]
      The 'sklearn' PyPI package is deprecated, use 'scikit-learn'
      rather than 'sklearn' for pip commands.

      Here is how to fix this error in the main use cases:
      - use 'pip install scikit-learn' rather than 'pip install sklearn'
      - replace 'sklearn' by 'scikit-learn' in your pip requirements files
        (requirements.txt, setup.py, setup.cfg, Pipfile, etc ...)
      - if the 'sklearn' package is used by one of your dependencies,
        it would be great if you take some time to track which package uses
        'sklearn' instead of 'scikit-learn' and report it to their issue tracker
      - as a last resort, set the environment variable
        SKLEARN_ALLOW_DEPRECATED_SKLEARN_PACKAGE_INSTALL=True to avoid this error

      More information is available at
      https://github.com/scikit-learn/sklearn-pypi-package
      [end of output]

  note: This error originates from a subprocess, and is likely not a problem with pip.
error: subprocess-exited-with-error

× Getting requirements to build wheel did not run successfully.
│ exit code: 1
╰─> See above for output.

note: This error originates from a subprocess, and is likely not a problem with pip.

[notice] A new release of pip is available: 23.2.1 -> 24.0
[notice] To update, run: python.exe -m pip install --upgrade pip
PS G:\Other computers\My Desktop PC\Documents\Python-Projects\face_recognition_project-main> pip install streamlit
Requirement already satisfied: streamlit in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (1.32.2)
Requirement already satisfied: altair<6,>=4.0 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit) (5.2.0)
Requirement already satisfied: blinker<2,>=1.0.0 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit) (1.7.0)
Requirement already satisfied: cachetools<6,>=4.0 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit) (5.3.3)
Requirement already satisfied: click<9,>=7.0 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit) (8.1.7)
Requirement already satisfied: numpy<2,>=1.19.3 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit) (1.26.4)
Requirement already satisfied: packaging<24,>=16.8 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit) (23.2)
Requirement already satisfied: pandas<3,>=1.3.0 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit) (2.2.1)
Requirement already satisfied: pillow<11,>=7.1.0 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit) (10.2.0)
Requirement already satisfied: protobuf<5,>=3.20 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit) (4.25.3)
Requirement already satisfied: pyarrow>=7.0 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit) (15.0.1)
Requirement already satisfied: requests<3,>=2.27 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit) (2.31.0)
Requirement already satisfied: rich<14,>=10.14.0 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit) (13.7.1)
Requirement already satisfied: tenacity<9,>=8.1.0 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit) (8.2.3)
Requirement already satisfied: toml<2,>=0.10.1 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit) (0.10.2)
Requirement already satisfied: typing-extensions<5,>=4.3.0 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit) (4.10.0)
Requirement already satisfied: gitpython!=3.1.19,<4,>=3.0.7 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit) (3.1.42)
Requirement already satisfied: pydeck<1,>=0.8.0b4 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit) (0.8.1b0)
Requirement already satisfied: tornado<7,>=6.0.3 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit) (6.4)
Requirement already satisfied: watchdog>=2.1.5 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit) (4.0.0)
Requirement already satisfied: jinja2 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from altair<6,>=4.0->streamlit) (3.1.3)
Requirement already satisfied: jsonschema>=3.0 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from altair<6,>=4.0->streamlit) (4.21.1)
Requirement already satisfied: toolz in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from altair<6,>=4.0->streamlit) (0.12.1)
Requirement already satisfied: colorama in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from click<9,>=7.0->streamlit) (0.4.6)
Requirement already satisfied: gitdb<5,>=4.0.1 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from gitpython!=3.1.19,<4,>=3.0.7->streamlit) (4.0.11)
Requirement already satisfied: python-dateutil>=2.8.2 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from pandas<3,>=1.3.0->streamlit) (2.9.0.post0)
Requirement already satisfied: pytz>=2020.1 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from pandas<3,>=1.3.0->streamlit) (2024.1)
Requirement already satisfied: tzdata>=2022.7 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from pandas<3,>=1.3.0->streamlit) (2024.1)
Requirement already satisfied: charset-normalizer<4,>=2 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from requests<3,>=2.27->streamlit) (3.3.2)
Requirement already satisfied: idna<4,>=2.5 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from requests<3,>=2.27->streamlit) (3.6)
Requirement already satisfied: urllib3<3,>=1.21.1 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from requests<3,>=2.27->streamlit) (2.2.1)
Requirement already satisfied: certifi>=2017.4.17 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from requests<3,>=2.27->streamlit) (2024.2.2)
Requirement already satisfied: markdown-it-py>=2.2.0 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from rich<14,>=10.14.0->streamlit) (3.0.0)
Requirement already satisfied: pygments<3.0.0,>=2.13.0 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from rich<14,>=10.14.0->streamlit) (2.17.2)
Requirement already satisfied: smmap<6,>=3.0.1 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from gitdb<5,>=4.0.1->gitpython!=3.1.19,<4,>=3.0.7->streamlit) (5.0.1)
Requirement already satisfied: MarkupSafe>=2.0 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from jinja2->altair<6,>=4.0->streamlit) (2.1.5)
Requirement already satisfied: attrs>=22.2.0 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from jsonschema>=3.0->altair<6,>=4.0->streamlit) (23.2.0)
Requirement already satisfied: jsonschema-specifications>=2023.03.6 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from jsonschema>=3.0->altair<6,>=4.0->streamlit) (2023.12.1)
Requirement already satisfied: referencing>=0.28.4 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from jsonschema>=3.0->altair<6,>=4.0->streamlit) (0.33.0)
Requirement already satisfied: rpds-py>=0.7.1 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from jsonschema>=3.0->altair<6,>=4.0->streamlit) (0.18.0)
Requirement already satisfied: mdurl~=0.1 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from markdown-it-py>=2.2.0->rich<14,>=10.14.0->streamlit) (0.1.2)
Requirement already satisfied: six>=1.5 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from python-dateutil>=2.8.2->pandas<3,>=1.3.0->streamlit) (1.16.0)

[notice] A new release of pip is available: 23.2.1 -> 24.0
[notice] To update, run: python.exe -m pip install --upgrade pip
PS G:\Other computers\My Desktop PC\Documents\Python-Projects\face_recognition_project-main> pip install streamlit-autorefresh
Collecting streamlit-autorefresh
  Obtaining dependency information for streamlit-autorefresh from https://files.pythonhosted.org/packages/2
0/82/e378f178498f1d99a672d81df71ebe9693a106cec6a628ee52ce3288cd6d/streamlit_autorefresh-1.0.1-py3-none-any.whl.metadata
  Downloading streamlit_autorefresh-1.0.1-py3-none-any.whl.metadata (436 bytes)
Requirement already satisfied: streamlit>=0.75 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit-autorefresh) (1.32.2)
Requirement already satisfied: altair<6,>=4.0 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit>=0.75->streamlit-autorefresh) (5.2.0)
Requirement already satisfied: blinker<2,>=1.0.0 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit>=0.75->streamlit-autorefresh) (1.7.0)
Requirement already satisfied: cachetools<6,>=4.0 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit>=0.75->streamlit-autorefresh) (5.3.3)
Requirement already satisfied: click<9,>=7.0 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit>=0.75->streamlit-autorefresh) (8.1.7)
Requirement already satisfied: numpy<2,>=1.19.3 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit>=0.75->streamlit-autorefresh) (1.26.4)
Requirement already satisfied: packaging<24,>=16.8 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit>=0.75->streamlit-autorefresh) (23.2)
Requirement already satisfied: pandas<3,>=1.3.0 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit>=0.75->streamlit-autorefresh) (2.2.1)
Requirement already satisfied: pillow<11,>=7.1.0 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit>=0.75->streamlit-autorefresh) (10.2.0)
Requirement already satisfied: protobuf<5,>=3.20 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit>=0.75->streamlit-autorefresh) (4.25.3)
Requirement already satisfied: pyarrow>=7.0 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit>=0.75->streamlit-autorefresh) (15.0.1)
Requirement already satisfied: requests<3,>=2.27 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit>=0.75->streamlit-autorefresh) (2.31.0)
Requirement already satisfied: rich<14,>=10.14.0 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit>=0.75->streamlit-autorefresh) (13.7.1)
Requirement already satisfied: tenacity<9,>=8.1.0 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit>=0.75->streamlit-autorefresh) (8.2.3)
Requirement already satisfied: toml<2,>=0.10.1 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit>=0.75->streamlit-autorefresh) (0.10.2)
Requirement already satisfied: typing-extensions<5,>=4.3.0 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit>=0.75->streamlit-autorefresh) (4.10.0)
Requirement already satisfied: gitpython!=3.1.19,<4,>=3.0.7 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit>=0.75->streamlit-autorefresh) (3.1.42)
Requirement already satisfied: pydeck<1,>=0.8.0b4 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit>=0.75->streamlit-autorefresh) (0.8.1b0)
Requirement already satisfied: tornado<7,>=6.0.3 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit>=0.75->streamlit-autorefresh) (6.4)
Requirement already satisfied: watchdog>=2.1.5 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from streamlit>=0.75->streamlit-autorefresh) (4.0.0)
Requirement already satisfied: jinja2 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from altair<6,>=4.0->streamlit>=0.75->streamlit-autorefresh) (3.1.3)
Requirement already satisfied: jsonschema>=3.0 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from altair<6,>=4.0->streamlit>=0.75->streamlit-autorefresh) (4.21.1)
Requirement already satisfied: toolz in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from altair<6,>=4.0->streamlit>=0.75->streamlit-autorefresh) (0.12.1)
Requirement already satisfied: colorama in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from click<9,>=7.0->streamlit>=0.75->streamlit-autorefresh) (0.4.6)
Requirement already satisfied: gitdb<5,>=4.0.1 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from gitpython!=3.1.19,<4,>=3.0.7->streamlit>=0.75->streamlit-autorefresh) (4.0.11)       
Requirement already satisfied: python-dateutil>=2.8.2 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from pandas<3,>=1.3.0->streamlit>=0.75->streamlit-autorefresh) (2.9.0.post0)       
Requirement already satisfied: pytz>=2020.1 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from pandas<3,>=1.3.0->streamlit>=0.75->streamlit-autorefresh) (2024.1)
Requirement already satisfied: tzdata>=2022.7 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from pandas<3,>=1.3.0->streamlit>=0.75->streamlit-autorefresh) (2024.1)
Requirement already satisfied: charset-normalizer<4,>=2 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from requests<3,>=2.27->streamlit>=0.75->streamlit-autorefresh) (3.3.2)
Requirement already satisfied: idna<4,>=2.5 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from requests<3,>=2.27->streamlit>=0.75->streamlit-autorefresh) (3.6)
Requirement already satisfied: urllib3<3,>=1.21.1 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from requests<3,>=2.27->streamlit>=0.75->streamlit-autorefresh) (2.2.1)
Requirement already satisfied: certifi>=2017.4.17 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from requests<3,>=2.27->streamlit>=0.75->streamlit-autorefresh) (2024.2.2)
Requirement already satisfied: markdown-it-py>=2.2.0 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from rich<14,>=10.14.0->streamlit>=0.75->streamlit-autorefresh) (3.0.0)
Requirement already satisfied: pygments<3.0.0,>=2.13.0 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from rich<14,>=10.14.0->streamlit>=0.75->streamlit-autorefresh) (2.17.2)
Requirement already satisfied: smmap<6,>=3.0.1 in c:\users\shubh\appdata\local\programs\python\python312\li
b\site-packages (from gitdb<5,>=4.0.1->gitpython!=3.1.19,<4,>=3.0.7->streamlit>=0.75->streamlit-autorefresh) (5.0.1)
Requirement already satisfied: MarkupSafe>=2.0 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from jinja2->altair<6,>=4.0->streamlit>=0.75->streamlit-autorefresh) (2.1.5)
Requirement already satisfied: attrs>=22.2.0 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from jsonschema>=3.0->altair<6,>=4.0->streamlit>=0.75->streamlit-autorefresh) (23.2.0)      
Requirement already satisfied: jsonschema-specifications>=2023.03.6 in c:\users\shubh\appdata\local\program
s\python\python312\lib\site-packages (from jsonschema>=3.0->altair<6,>=4.0->streamlit>=0.75->streamlit-autorefresh) (2023.12.1)
Requirement already satisfied: referencing>=0.28.4 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from jsonschema>=3.0->altair<6,>=4.0->streamlit>=0.75->streamlit-autorefresh) (0.33.0)
Requirement already satisfied: rpds-py>=0.7.1 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from jsonschema>=3.0->altair<6,>=4.0->streamlit>=0.75->streamlit-autorefresh) (0.18.0)     
Requirement already satisfied: mdurl~=0.1 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from markdown-it-py>=2.2.0->rich<14,>=10.14.0->streamlit>=0.75->streamlit-autorefresh) (0.1.2) 
Requirement already satisfied: six>=1.5 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from python-dateutil>=2.8.2->pandas<3,>=1.3.0->streamlit>=0.75->streamlit-autorefresh) (1.16.0)  
Downloading streamlit_autorefresh-1.0.1-py3-none-any.whl (700 kB)
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 700.8/700.8 kB 1.4 MB/s eta 0:00:00
Installing collected packages: streamlit-autorefresh
Successfully installed streamlit-autorefresh-1.0.1

[notice] A new release of pip is available: 23.2.1 -> 24.0
[notice] To update, run: python.exe -m pip install --upgrade pip
PS G:\Other computers\My Desktop PC\Documents\Python-Projects\face_recognition_project-main> pip install pypiwin32
Collecting pypiwin32
  Obtaining dependency information for pypiwin32 from https://files.pythonhosted.org/packages/d0/1b/2f292bbd742e369a100c91faa0483172cd91a1a422a6692055ac920946c5/pypiwin32-223-py3-none-any.whl.metadata
  Downloading pypiwin32-223-py3-none-any.whl.metadata (236 bytes)
Collecting pywin32>=223 (from pypiwin32)
  Obtaining dependency information for pywin32>=223 from https://files.pythonhosted.org/packages/83/1c/25b79fc3ec99b19b0a0730cc47356f7e2959863bf9f3cd314332bddb4f68/pywin32-306-cp312-cp312-win_amd64.whl.metadata    
  Downloading pywin32-306-cp312-cp312-win_amd64.whl.metadata (6.5 kB)
Downloading pypiwin32-223-py3-none-any.whl (1.7 kB)
Downloading pywin32-306-cp312-cp312-win_amd64.whl (9.2 MB)
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 9.2/9.2 MB 3.5 MB/s eta 0:00:00
Installing collected packages: pywin32, pypiwin32
Successfully installed pypiwin32-223 pywin32-306

[notice] A new release of pip is available: 23.2.1 -> 24.0
[notice] To update, run: python.exe -m pip install --upgrade pip
PS G:\Other computers\My Desktop PC\Documents\Python-Projects\face_recognition_project-main> pip install scikit-learn
Collecting scikit-learn
  Obtaining dependency information for scikit-learn from https://files.pythonhosted.org/packages/76/d8/02fa
68de37f657e6bb241e6f9ec6240bafa43222d3ef836a248145d9548f/scikit_learn-1.4.1.post1-cp312-cp312-win_amd64.whl.metadata
  Downloading scikit_learn-1.4.1.post1-cp312-cp312-win_amd64.whl.metadata (11 kB)
Requirement already satisfied: numpy<2.0,>=1.19.5 in c:\users\shubh\appdata\local\programs\python\python312\lib\site-packages (from scikit-learn) (1.26.4)
Collecting scipy>=1.6.0 (from scikit-learn)
  Obtaining dependency information for scipy>=1.6.0 from https://files.pythonhosted.org/packages/f3/31/91a2a3c5eb85d2bfa86d7c98f2df5d77dcdefb3d80ca9f9037ad04393acf/scipy-1.12.0-cp312-cp312-win_amd64.whl.metadata   
  Downloading scipy-1.12.0-cp312-cp312-win_amd64.whl.metadata (60 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 60.4/60.4 kB 1.1 MB/s eta 0:00:00
Collecting joblib>=1.2.0 (from scikit-learn)
  Obtaining dependency information for joblib>=1.2.0 from https://files.pythonhosted.org/packages/10/40/d551139c85db202f1f384ba8bcf96aca2f329440a844f924c8a0040b6d02/joblib-1.3.2-py3-none-any.whl.metadata
  Downloading joblib-1.3.2-py3-none-any.whl.metadata (5.4 kB)
Collecting threadpoolctl>=2.0.0 (from scikit-learn)
  Obtaining dependency information for threadpoolctl>=2.0.0 from https://files.pythonhosted.org/packages/b1
/2c/f504e55d98418f2fcf756a56877e6d9a45dd5ed28b3d7c267b300e85ad5b/threadpoolctl-3.3.0-py3-none-any.whl.metadata
  Downloading threadpoolctl-3.3.0-py3-none-any.whl.metadata (13 kB)
Downloading scikit_learn-1.4.1.post1-cp312-cp312-win_amd64.whl (10.6 MB)
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 10.6/10.6 MB 3.3 MB/s eta 0:00:00
Downloading joblib-1.3.2-py3-none-any.whl (302 kB)
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 302.2/302.2 kB 6.2 MB/s eta 0:00:00
Downloading scipy-1.12.0-cp312-cp312-win_amd64.whl (45.8 MB)
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 45.8/45.8 MB 3.5 MB/s eta 0:00:00
Downloading threadpoolctl-3.3.0-py3-none-any.whl (17 kB)
Installing collected packages: threadpoolctl, scipy, joblib, scikit-learn
Successfully installed joblib-1.3.2 scikit-learn-1.4.1.post1 scipy-1.12.0 threadpoolctl-3.3.0

[notice] A new release of pip is available: 23.2.1 -> 24.0
[notice] To update, run: python.exe -m pip install --upgrade pip
PS G:\Other computers\My Desktop PC\Documents\Python-Projects\face_recognition_project-main> exit
 -->
