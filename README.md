# CamcodeHW1
Terminal Script for Camcode Virtualenv from VS Code

nishanth@Chandans-Air ~ % /usr/local/bin/python3 /Users/nishanth/camcodehw.py

nishanth@Chandans-Air ~ % python3
Python 3.12.1 (v3.12.1:2305ca5144, Dec  7 2023, 17:23:38) [Clang 13.0.0 (clang-1300.0.29.30)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>> exit()

nishanth@Chandans-Air ~ % which python3
/Library/Frameworks/Python.framework/Versions/3.12/bin/python3

nishanth@Chandans-Air ~ % python3 -m pip install virtualenv
Requirement already satisfied: virtualenv in /Library/Frameworks/Python.framework/Versions/3.12/lib/python3.12/site-packages (20.25.0)
Requirement already satisfied: distlib<1,>=0.3.7 in /Library/Frameworks/Python.framework/Versions/3.12/lib/python3.12/site-packages (from virtualenv) (0.3.8)
Requirement already satisfied: filelock<4,>=3.12.2 in /Library/Frameworks/Python.framework/Versions/3.12/lib/python3.12/site-packages (from virtualenv) (3.13.1)
Requirement already satisfied: platformdirs<5,>=3.9.1 in /Library/Frameworks/Python.framework/Versions/3.12/lib/python3.12/site-packages (from virtualenv) (4.1.0)
nishanth@Chandans-Air ~ % python3 -m virtualenv venv3      
created virtual environment CPython3.12.1.final.0-64 in 429ms
  creator CPython3Posix(dest=/Users/nishanth/venv3, clear=False, no_vcs_ignore=False, global=False)
  seeder FromAppData(download=False, pip=bundle, via=copy, app_data_dir=/Users/nishanth/Library/Application Support/virtualenv)
    added seed packages: Babel==2.14.0, Jinja2==3.1.3, MarkupSafe==2.1.4, PyYAML==6.0.1, QtPy==2.4.1, Send2Trash==1.8.2, annotated_types==0.6.0, anyio==4.2.0, appnope==0.1.3, argon2_cffi==23.1.0, argon2_cffi_bindings==21.2.0, arrow==1.3.0, asttokens==2.4.1, async_lru==2.0.4, attrs==23.2.0, beautifulsoup4==4.12.3, bleach==6.1.0, certifi==2023.11.17, cffi==1.16.0, charset_normalizer==3.3.2, comm==0.2.1, debugpy==1.8.0, decorator==5.1.1, defusedxml==0.7.1, executing==2.0.1, fastapi==0.50.0, fastjsonschema==2.19.1, fqdn==1.5.1, idna==3.6, ipykernel==6.29.0, ipython==8.20.0, ipywidgets==8.1.1, isoduration==20.11.0, jedi==0.19.1, json5==0.9.14, jsonpointer==2.4, jsonschema==4.21.1, jsonschema_specifications==2023.12.1, jupyter==1.0.0, jupyter_client==8.6.0, jupyter_console==6.6.3, jupyter_core==5.7.1, jupyter_events==0.9.0, jupyter_lsp==2.2.2, jupyter_server==2.12.5, jupyter_server_terminals==0.5.2, jupyterlab==4.0.12, jupyterlab_pygments==0.3.0, jupyterlab_server==2.25.2, jupyterlab_widgets==3.0.9, matplotlib_inline==0.1.6, mistune==3.0.2, nbclient==0.9.0, nbconvert==7.14.2, nbformat==5.9.2, nest_asyncio==1.6.0, notebook==7.0.7, notebook_shim==0.2.3, numpy==1.26.3, overrides==7.7.0, packaging==23.2, pandas==2.2.0, pandocfilters==1.5.1, parso==0.8.3, pexpect==4.9.0, pip==23.3.2, platformdirs==4.1.0, prometheus_client==0.19.0, prompt_toolkit==3.0.43, psutil==5.9.8, ptyprocess==0.7.0, pure_eval==0.2.2, pycparser==2.21, pydantic==1.10.14, pydantic_core==2.16.1, pygments==2.17.2, python_dateutil==2.8.2, python_json_logger==2.0.7, pytz==2023.4, pyzmq==25.1.2, qtconsole==5.5.1, referencing==0.33.0, requests==2.31.0, rfc3339_validator==0.1.4, rfc3986_validator==0.1.1, rpds_py==0.17.1, six==1.16.0, sniffio==1.3.0, soupsieve==2.5, stack_data==0.6.3, starlette==0.13.2, terminado==0.18.0, tinycss2==1.2.1, tornado==6.4, traitlets==5.14.1, types_python_dateutil==2.8.19.20240106, typing_extensions==4.9.0, tzdata==2023.4, uri_template==1.3.0, urllib3==2.2.0, wcwidth==0.2.13, webcolors==1.13, webencodings==0.5.1, websocket_client==1.7.0, widgetsnbextension==4.0.9
  activators BashActivator,CShellActivator,FishActivator,NushellActivator,PowerShellActivator,PythonActivator
nishanth@Chandans-Air ~ % ls
Applications            Homework1               Pictures                dir2                    nishblaze.pem
Desktop                 Library                 Public                  dirl                    requirements.txt
Documents               Movies                  README.md               hwcam.py                us-counties.csv
Downloads               Music                   camcodehw.py            ner.dataset.jsonl       venv3
nishanth@Chandans-Air ~ % source venv3/bin/activate
(venv3) nishanth@Chandans-Air ~ % which python
/Users/nishanth/venv3/bin/python
(venv3) nishanth@Chandans-Air ~ % deactivate
nishanth@Chandans-Air ~ % cat venv3/bin/activate
# This file must be used with "source bin/activate" *from bash*
# you cannot run it directly


if [ "${BASH_SOURCE-}" = "$0" ]; then
    echo "You must source this script: \$ source $0" >&2
    exit 33
fi

deactivate () {
    unset -f pydoc >/dev/null 2>&1 || true

    # reset old environment variables
    # ! [ -z ${VAR+_} ] returns true if VAR is declared at all
    if ! [ -z "${_OLD_VIRTUAL_PATH:+_}" ] ; then
        PATH="$_OLD_VIRTUAL_PATH"
        export PATH
        unset _OLD_VIRTUAL_PATH
    fi
    if ! [ -z "${_OLD_VIRTUAL_PYTHONHOME+_}" ] ; then
        PYTHONHOME="$_OLD_VIRTUAL_PYTHONHOME"
        export PYTHONHOME
        unset _OLD_VIRTUAL_PYTHONHOME
    fi

    # The hash command must be called to get it to forget past
    # commands. Without forgetting past commands the $PATH changes
    # we made may not be respected
    hash -r 2>/dev/null

    if ! [ -z "${_OLD_VIRTUAL_PS1+_}" ] ; then
        PS1="$_OLD_VIRTUAL_PS1"
        export PS1
        unset _OLD_VIRTUAL_PS1
    fi

    unset VIRTUAL_ENV
    unset VIRTUAL_ENV_PROMPT
    if [ ! "${1-}" = "nondestructive" ] ; then
    # Self destruct!
        unset -f deactivate
    fi
}

# unset irrelevant variables
deactivate nondestructive

VIRTUAL_ENV='/Users/nishanth/venv3'
if ([ "$OSTYPE" = "cygwin" ] || [ "$OSTYPE" = "msys" ]) && $(command -v cygpath &> /dev/null) ; then
    VIRTUAL_ENV=$(cygpath -u "$VIRTUAL_ENV")
fi
export VIRTUAL_ENV

_OLD_VIRTUAL_PATH="$PATH"
PATH="$VIRTUAL_ENV/bin:$PATH"
export PATH

if [ "x" != x ] ; then
    VIRTUAL_ENV_PROMPT=""
else
    VIRTUAL_ENV_PROMPT=$(basename "$VIRTUAL_ENV")
fi
export VIRTUAL_ENV_PROMPT

# unset PYTHONHOME if set
if ! [ -z "${PYTHONHOME+_}" ] ; then
    _OLD_VIRTUAL_PYTHONHOME="$PYTHONHOME"
    unset PYTHONHOME
fi

if [ -z "${VIRTUAL_ENV_DISABLE_PROMPT-}" ] ; then
    _OLD_VIRTUAL_PS1="${PS1-}"
    PS1="(${VIRTUAL_ENV_PROMPT}) ${PS1-}"
    export PS1
fi

# Make sure to unalias pydoc if it's already there
alias pydoc 2>/dev/null >/dev/null && unalias pydoc || true

pydoc () {
    python -m pydoc "$@"
}

# The hash command must be called to get it to forget past
# commands. Without forgetting past commands the $PATH changes
# we made may not be respected
hash -r 2>/dev/null
nishanth@Chandans-Air ~ % source venv3/bin/activate

(venv3) nishanth@Chandans-Air ~ % python3 -m pip install pandas fastapi 
Requirement already satisfied: pandas in ./venv3/lib/python3.12/site-packages (2.2.0)
Requirement already satisfied: fastapi in ./venv3/lib/python3.12/site-packages (0.50.0)
Requirement already satisfied: numpy<2,>=1.26.0 in ./venv3/lib/python3.12/site-packages (from pandas) (1.26.3)
Requirement already satisfied: python-dateutil>=2.8.2 in ./venv3/lib/python3.12/site-packages (from pandas) (2.8.2)
Requirement already satisfied: pytz>=2020.1 in ./venv3/lib/python3.12/site-packages (from pandas) (2023.4)
Requirement already satisfied: tzdata>=2022.7 in ./venv3/lib/python3.12/site-packages (from pandas) (2023.4)
Requirement already satisfied: starlette==0.13.2 in ./venv3/lib/python3.12/site-packages (from fastapi) (0.13.2)
Requirement already satisfied: pydantic<2.0.0,>=0.32.2 in ./venv3/lib/python3.12/site-packages (from fastapi) (1.10.14)
Requirement already satisfied: typing-extensions>=4.2.0 in ./venv3/lib/python3.12/site-packages (from pydantic<2.0.0,>=0.32.2->fastapi) (4.9.0)
Requirement already satisfied: six>=1.5 in ./venv3/lib/python3.12/site-packages (from python-dateutil>=2.8.2->pandas) (1.16.0)
(venv3) nishanth@Chandans-Air ~ % python3 -m pip                       

Usage:   
  /Users/nishanth/venv3/bin/python3 -m pip <command> [options]

Commands:
  install                     Install packages.
  download                    Download packages.
  uninstall                   Uninstall packages.
  freeze                      Output installed packages in requirements format.
  inspect                     Inspect the python environment.
  list                        List installed packages.
  show                        Show information about installed packages.
  check                       Verify installed packages have compatible dependencies.
  config                      Manage local and global configuration.
  search                      Search PyPI for packages.
  cache                       Inspect and manage pip's wheel cache.
  index                       Inspect information available from package indexes.
  wheel                       Build wheels from your requirements.
  hash                        Compute hashes of package archives.
  completion                  A helper command used for command completion.
  debug                       Show information useful for debugging.
  help                        Show help for commands.

General Options:
  -h, --help                  Show help.
  --debug                     Let unhandled exceptions propagate outside the main subroutine, instead of logging them to stderr.
  --isolated                  Run pip in an isolated mode, ignoring environment variables and user configuration.
  --require-virtualenv        Allow pip to only run in a virtual environment; exit with an error otherwise.
  --python <python>           Run pip with the specified Python interpreter.
  -v, --verbose               Give more output. Option is additive, and can be used up to 3 times.
  -V, --version               Show version and exit.
  -q, --quiet                 Give less output. Option is additive, and can be used up to 3 times (corresponding to WARNING, ERROR, and CRITICAL logging
                              levels).
  --log <path>                Path to a verbose appending log.
  --no-input                  Disable prompting for input.
  --keyring-provider <keyring_provider>
                              Enable the credential lookup via the keyring library if user input is allowed. Specify which mechanism to use [disabled,
                              import, subprocess]. (default: disabled)
  --proxy <proxy>             Specify a proxy in the form scheme://[user:passwd@]proxy.server:port.
  --retries <retries>         Maximum number of retries each connection should attempt (default 5 times).
  --timeout <sec>             Set the socket timeout (default 15 seconds).
  --exists-action <action>    Default action when a path already exists: (s)witch, (i)gnore, (w)ipe, (b)ackup, (a)bort.
  --trusted-host <hostname>   Mark this host or host:port pair as trusted, even though it does not have valid or any HTTPS.
  --cert <path>               Path to PEM-encoded CA certificate bundle. If provided, overrides the default. See 'SSL Certificate Verification' in pip
                              documentation for more information.
  --client-cert <path>        Path to SSL client certificate, a single file containing the private key and the certificate in PEM format.
  --cache-dir <dir>           Store the cache data in <dir>.
  --no-cache-dir              Disable the cache.
  --disable-pip-version-check
                              Don't periodically check PyPI to determine whether a new version of pip is available for download. Implied with --no-index.
  --no-color                  Suppress colored output.
  --no-python-version-warning
                              Silence deprecation warnings for upcoming unsupported Pythons.
  --use-feature <feature>     Enable new functionality, that may be backward incompatible.
  --use-deprecated <feature>  Enable deprecated functionality, that will be removed in the future.
(venv3) nishanth@Chandans-Air ~ % python3 -m pip freeze                
annotated-types==0.6.0
anyio==4.2.0
appnope==0.1.3
argon2-cffi==23.1.0
argon2-cffi-bindings==21.2.0
arrow==1.3.0
asttokens==2.4.1
async-lru==2.0.4
attrs==23.2.0
Babel==2.14.0
beautifulsoup4==4.12.3
bleach==6.1.0
certifi==2023.11.17
cffi==1.16.0
charset-normalizer==3.3.2
comm==0.2.1
debugpy==1.8.0
decorator==5.1.1
defusedxml==0.7.1
executing==2.0.1
fastapi==0.50.0
fastjsonschema==2.19.1
fqdn==1.5.1
idna==3.6
ipykernel==6.29.0
ipython==8.20.0
ipywidgets==8.1.1
isoduration==20.11.0
jedi==0.19.1
Jinja2==3.1.3
json5==0.9.14
jsonpointer==2.4
jsonschema==4.21.1
jsonschema-specifications==2023.12.1
jupyter==1.0.0
jupyter-console==6.6.3
jupyter-events==0.9.0
jupyter-lsp==2.2.2
jupyter_client==8.6.0
jupyter_core==5.7.1
jupyter_server==2.12.5
jupyter_server_terminals==0.5.2
jupyterlab==4.0.12
jupyterlab-widgets==3.0.9
jupyterlab_pygments==0.3.0
jupyterlab_server==2.25.2
MarkupSafe==2.1.4
matplotlib-inline==0.1.6
mistune==3.0.2
nbclient==0.9.0
nbconvert==7.14.2
nbformat==5.9.2
nest-asyncio==1.6.0
notebook==7.0.7
notebook_shim==0.2.3
numpy==1.26.3
overrides==7.7.0
packaging==23.2
pandas==2.2.0
pandocfilters==1.5.1
parso==0.8.3
pexpect==4.9.0
platformdirs==4.1.0
prometheus-client==0.19.0
prompt-toolkit==3.0.43
psutil==5.9.8
ptyprocess==0.7.0
pure-eval==0.2.2
pycparser==2.21
pydantic==1.10.14
pydantic_core==2.16.1
Pygments==2.17.2
python-dateutil==2.8.2
python-json-logger==2.0.7
pytz==2023.4
PyYAML==6.0.1
pyzmq==25.1.2
qtconsole==5.5.1
QtPy==2.4.1
referencing==0.33.0
requests==2.31.0
rfc3339-validator==0.1.4
rfc3986-validator==0.1.1
rpds-py==0.17.1
Send2Trash==1.8.2
six==1.16.0
sniffio==1.3.0
soupsieve==2.5
stack-data==0.6.3
starlette==0.13.2
terminado==0.18.0
tinycss2==1.2.1
tornado==6.4
traitlets==5.14.1
types-python-dateutil==2.8.19.20240106
typing_extensions==4.9.0
tzdata==2023.4
uri-template==1.3.0
urllib3==2.2.0
wcwidth==0.2.13
webcolors==1.13
webencodings==0.5.1
websocket-client==1.7.0
widgetsnbextension==4.0.9
(venv3) nishanth@Chandans-Air ~ % python3 -m pip freeze | grep pandas
pandas==2.2.0
(venv3) nishanth@Chandans-Air ~ % python3 -m pip install fastapi==0.50.0
Requirement already satisfied: fastapi==0.50.0 in ./venv3/lib/python3.12/site-packages (0.50.0)
Requirement already satisfied: starlette==0.13.2 in ./venv3/lib/python3.12/site-packages (from fastapi==0.50.0) (0.13.2)
Requirement already satisfied: pydantic<2.0.0,>=0.32.2 in ./venv3/lib/python3.12/site-packages (from fastapi==0.50.0) (1.10.14)
Requirement already satisfied: typing-extensions>=4.2.0 in ./venv3/lib/python3.12/site-packages (from pydantic<2.0.0,>=0.32.2->fastapi==0.50.0) (4.9.0)
(venv3) nishanth@Chandans-Air ~ % python3 -m pip freeze | grep fastapi  
fastapi==0.50.0
(venv3) nishanth@Chandans-Air ~ % pip freeze > requirements.txt

(venv3) nishanth@Chandans-Air ~ % cat requirements.txt 
annotated-types==0.6.0
anyio==4.2.0
appnope==0.1.3
argon2-cffi==23.1.0
argon2-cffi-bindings==21.2.0
arrow==1.3.0
asttokens==2.4.1
async-lru==2.0.4
attrs==23.2.0
Babel==2.14.0
beautifulsoup4==4.12.3
bleach==6.1.0
certifi==2023.11.17
cffi==1.16.0
charset-normalizer==3.3.2
comm==0.2.1
debugpy==1.8.0
decorator==5.1.1
defusedxml==0.7.1
executing==2.0.1
fastapi==0.50.0
fastjsonschema==2.19.1
fqdn==1.5.1
idna==3.6
ipykernel==6.29.0
ipython==8.20.0
ipywidgets==8.1.1
isoduration==20.11.0
jedi==0.19.1
Jinja2==3.1.3
json5==0.9.14
jsonpointer==2.4
jsonschema==4.21.1
jsonschema-specifications==2023.12.1
jupyter==1.0.0
jupyter-console==6.6.3
jupyter-events==0.9.0
jupyter-lsp==2.2.2
jupyter_client==8.6.0
jupyter_core==5.7.1
jupyter_server==2.12.5
jupyter_server_terminals==0.5.2
jupyterlab==4.0.12
jupyterlab-widgets==3.0.9
jupyterlab_pygments==0.3.0
jupyterlab_server==2.25.2
MarkupSafe==2.1.4
matplotlib-inline==0.1.6
mistune==3.0.2
nbclient==0.9.0
nbconvert==7.14.2
nbformat==5.9.2
nest-asyncio==1.6.0
notebook==7.0.7
notebook_shim==0.2.3
numpy==1.26.3
overrides==7.7.0
packaging==23.2
pandas==2.2.0
pandocfilters==1.5.1
parso==0.8.3
pexpect==4.9.0
platformdirs==4.1.0
prometheus-client==0.19.0
prompt-toolkit==3.0.43
psutil==5.9.8
ptyprocess==0.7.0
pure-eval==0.2.2
pycparser==2.21
pydantic==1.10.14
pydantic_core==2.16.1
Pygments==2.17.2
python-dateutil==2.8.2
python-json-logger==2.0.7
pytz==2023.4
PyYAML==6.0.1
pyzmq==25.1.2
qtconsole==5.5.1
QtPy==2.4.1
referencing==0.33.0
requests==2.31.0
rfc3339-validator==0.1.4
rfc3986-validator==0.1.1
rpds-py==0.17.1
Send2Trash==1.8.2
six==1.16.0
sniffio==1.3.0
soupsieve==2.5
stack-data==0.6.3
starlette==0.13.2
terminado==0.18.0
tinycss2==1.2.1
tornado==6.4
traitlets==5.14.1
types-python-dateutil==2.8.19.20240106
typing_extensions==4.9.0
tzdata==2023.4
uri-template==1.3.0
urllib3==2.2.0
wcwidth==0.2.13
webcolors==1.13
webencodings==0.5.1
websocket-client==1.7.0
widgetsnbextension==4.0.9
(venv3) nishanth@Chandans-Air ~ % pip install jupyter
Requirement already satisfied: jupyter in ./venv3/lib/python3.12/site-packages (1.0.0)
Requirement already satisfied: notebook in ./venv3/lib/python3.12/site-packages (from jupyter) (7.0.7)
Requirement already satisfied: qtconsole in ./venv3/lib/python3.12/site-packages (from jupyter) (5.5.1)
Requirement already satisfied: jupyter-console in ./venv3/lib/python3.12/site-packages (from jupyter) (6.6.3)
Requirement already satisfied: nbconvert in ./venv3/lib/python3.12/site-packages (from jupyter) (7.14.2)
Requirement already satisfied: ipykernel in ./venv3/lib/python3.12/site-packages (from jupyter) (6.29.0)
Requirement already satisfied: ipywidgets in ./venv3/lib/python3.12/site-packages (from jupyter) (8.1.1)
Requirement already satisfied: appnope in ./venv3/lib/python3.12/site-packages (from ipykernel->jupyter) (0.1.3)
Requirement already satisfied: comm>=0.1.1 in ./venv3/lib/python3.12/site-packages (from ipykernel->jupyter) (0.2.1)
Requirement already satisfied: debugpy>=1.6.5 in ./venv3/lib/python3.12/site-packages (from ipykernel->jupyter) (1.8.0)
Requirement already satisfied: ipython>=7.23.1 in ./venv3/lib/python3.12/site-packages (from ipykernel->jupyter) (8.20.0)
Requirement already satisfied: jupyter-client>=6.1.12 in ./venv3/lib/python3.12/site-packages (from ipykernel->jupyter) (8.6.0)
Requirement already satisfied: jupyter-core!=5.0.*,>=4.12 in ./venv3/lib/python3.12/site-packages (from ipykernel->jupyter) (5.7.1)
Requirement already satisfied: matplotlib-inline>=0.1 in ./venv3/lib/python3.12/site-packages (from ipykernel->jupyter) (0.1.6)
Requirement already satisfied: nest-asyncio in ./venv3/lib/python3.12/site-packages (from ipykernel->jupyter) (1.6.0)
Requirement already satisfied: packaging in ./venv3/lib/python3.12/site-packages (from ipykernel->jupyter) (23.2)
Requirement already satisfied: psutil in ./venv3/lib/python3.12/site-packages (from ipykernel->jupyter) (5.9.8)
Requirement already satisfied: pyzmq>=24 in ./venv3/lib/python3.12/site-packages (from ipykernel->jupyter) (25.1.2)
Requirement already satisfied: tornado>=6.1 in ./venv3/lib/python3.12/site-packages (from ipykernel->jupyter) (6.4)
Requirement already satisfied: traitlets>=5.4.0 in ./venv3/lib/python3.12/site-packages (from ipykernel->jupyter) (5.14.1)
Requirement already satisfied: widgetsnbextension~=4.0.9 in ./venv3/lib/python3.12/site-packages (from ipywidgets->jupyter) (4.0.9)
Requirement already satisfied: jupyterlab-widgets~=3.0.9 in ./venv3/lib/python3.12/site-packages (from ipywidgets->jupyter) (3.0.9)
Requirement already satisfied: prompt-toolkit>=3.0.30 in ./venv3/lib/python3.12/site-packages (from jupyter-console->jupyter) (3.0.43)
Requirement already satisfied: pygments in ./venv3/lib/python3.12/site-packages (from jupyter-console->jupyter) (2.17.2)
Requirement already satisfied: beautifulsoup4 in ./venv3/lib/python3.12/site-packages (from nbconvert->jupyter) (4.12.3)
Requirement already satisfied: bleach!=5.0.0 in ./venv3/lib/python3.12/site-packages (from nbconvert->jupyter) (6.1.0)
Requirement already satisfied: defusedxml in ./venv3/lib/python3.12/site-packages (from nbconvert->jupyter) (0.7.1)
Requirement already satisfied: jinja2>=3.0 in ./venv3/lib/python3.12/site-packages (from nbconvert->jupyter) (3.1.3)
Requirement already satisfied: jupyterlab-pygments in ./venv3/lib/python3.12/site-packages (from nbconvert->jupyter) (0.3.0)
Requirement already satisfied: markupsafe>=2.0 in ./venv3/lib/python3.12/site-packages (from nbconvert->jupyter) (2.1.4)
Requirement already satisfied: mistune<4,>=2.0.3 in ./venv3/lib/python3.12/site-packages (from nbconvert->jupyter) (3.0.2)
Requirement already satisfied: nbclient>=0.5.0 in ./venv3/lib/python3.12/site-packages (from nbconvert->jupyter) (0.9.0)
Requirement already satisfied: nbformat>=5.7 in ./venv3/lib/python3.12/site-packages (from nbconvert->jupyter) (5.9.2)
Requirement already satisfied: pandocfilters>=1.4.1 in ./venv3/lib/python3.12/site-packages (from nbconvert->jupyter) (1.5.1)
Requirement already satisfied: tinycss2 in ./venv3/lib/python3.12/site-packages (from nbconvert->jupyter) (1.2.1)
Requirement already satisfied: jupyter-server<3,>=2.4.0 in ./venv3/lib/python3.12/site-packages (from notebook->jupyter) (2.12.5)
Requirement already satisfied: jupyterlab-server<3,>=2.22.1 in ./venv3/lib/python3.12/site-packages (from notebook->jupyter) (2.25.2)
Requirement already satisfied: jupyterlab<5,>=4.0.2 in ./venv3/lib/python3.12/site-packages (from notebook->jupyter) (4.0.12)
Requirement already satisfied: notebook-shim<0.3,>=0.2 in ./venv3/lib/python3.12/site-packages (from notebook->jupyter) (0.2.3)
Requirement already satisfied: qtpy>=2.4.0 in ./venv3/lib/python3.12/site-packages (from qtconsole->jupyter) (2.4.1)
Requirement already satisfied: six>=1.9.0 in ./venv3/lib/python3.12/site-packages (from bleach!=5.0.0->nbconvert->jupyter) (1.16.0)
Requirement already satisfied: webencodings in ./venv3/lib/python3.12/site-packages (from bleach!=5.0.0->nbconvert->jupyter) (0.5.1)
Requirement already satisfied: decorator in ./venv3/lib/python3.12/site-packages (from ipython>=7.23.1->ipykernel->jupyter) (5.1.1)
Requirement already satisfied: jedi>=0.16 in ./venv3/lib/python3.12/site-packages (from ipython>=7.23.1->ipykernel->jupyter) (0.19.1)
Requirement already satisfied: stack-data in ./venv3/lib/python3.12/site-packages (from ipython>=7.23.1->ipykernel->jupyter) (0.6.3)
Requirement already satisfied: pexpect>4.3 in ./venv3/lib/python3.12/site-packages (from ipython>=7.23.1->ipykernel->jupyter) (4.9.0)
Requirement already satisfied: python-dateutil>=2.8.2 in ./venv3/lib/python3.12/site-packages (from jupyter-client>=6.1.12->ipykernel->jupyter) (2.8.2)
Requirement already satisfied: platformdirs>=2.5 in ./venv3/lib/python3.12/site-packages (from jupyter-core!=5.0.*,>=4.12->ipykernel->jupyter) (4.1.0)
Requirement already satisfied: anyio>=3.1.0 in ./venv3/lib/python3.12/site-packages (from jupyter-server<3,>=2.4.0->notebook->jupyter) (4.2.0)
Requirement already satisfied: argon2-cffi in ./venv3/lib/python3.12/site-packages (from jupyter-server<3,>=2.4.0->notebook->jupyter) (23.1.0)
Requirement already satisfied: jupyter-events>=0.9.0 in ./venv3/lib/python3.12/site-packages (from jupyter-server<3,>=2.4.0->notebook->jupyter) (0.9.0)
Requirement already satisfied: jupyter-server-terminals in ./venv3/lib/python3.12/site-packages (from jupyter-server<3,>=2.4.0->notebook->jupyter) (0.5.2)
Requirement already satisfied: overrides in ./venv3/lib/python3.12/site-packages (from jupyter-server<3,>=2.4.0->notebook->jupyter) (7.7.0)
Requirement already satisfied: prometheus-client in ./venv3/lib/python3.12/site-packages (from jupyter-server<3,>=2.4.0->notebook->jupyter) (0.19.0)
Requirement already satisfied: send2trash>=1.8.2 in ./venv3/lib/python3.12/site-packages (from jupyter-server<3,>=2.4.0->notebook->jupyter) (1.8.2)
Requirement already satisfied: terminado>=0.8.3 in ./venv3/lib/python3.12/site-packages (from jupyter-server<3,>=2.4.0->notebook->jupyter) (0.18.0)
Requirement already satisfied: websocket-client in ./venv3/lib/python3.12/site-packages (from jupyter-server<3,>=2.4.0->notebook->jupyter) (1.7.0)
Requirement already satisfied: async-lru>=1.0.0 in ./venv3/lib/python3.12/site-packages (from jupyterlab<5,>=4.0.2->notebook->jupyter) (2.0.4)
Requirement already satisfied: jupyter-lsp>=2.0.0 in ./venv3/lib/python3.12/site-packages (from jupyterlab<5,>=4.0.2->notebook->jupyter) (2.2.2)
Requirement already satisfied: babel>=2.10 in ./venv3/lib/python3.12/site-packages (from jupyterlab-server<3,>=2.22.1->notebook->jupyter) (2.14.0)
Requirement already satisfied: json5>=0.9.0 in ./venv3/lib/python3.12/site-packages (from jupyterlab-server<3,>=2.22.1->notebook->jupyter) (0.9.14)
Requirement already satisfied: jsonschema>=4.18.0 in ./venv3/lib/python3.12/site-packages (from jupyterlab-server<3,>=2.22.1->notebook->jupyter) (4.21.1)
Requirement already satisfied: requests>=2.31 in ./venv3/lib/python3.12/site-packages (from jupyterlab-server<3,>=2.22.1->notebook->jupyter) (2.31.0)
Requirement already satisfied: fastjsonschema in ./venv3/lib/python3.12/site-packages (from nbformat>=5.7->nbconvert->jupyter) (2.19.1)
Requirement already satisfied: wcwidth in ./venv3/lib/python3.12/site-packages (from prompt-toolkit>=3.0.30->jupyter-console->jupyter) (0.2.13)
Requirement already satisfied: soupsieve>1.2 in ./venv3/lib/python3.12/site-packages (from beautifulsoup4->nbconvert->jupyter) (2.5)
Requirement already satisfied: idna>=2.8 in ./venv3/lib/python3.12/site-packages (from anyio>=3.1.0->jupyter-server<3,>=2.4.0->notebook->jupyter) (3.6)
Requirement already satisfied: sniffio>=1.1 in ./venv3/lib/python3.12/site-packages (from anyio>=3.1.0->jupyter-server<3,>=2.4.0->notebook->jupyter) (1.3.0)
Requirement already satisfied: parso<0.9.0,>=0.8.3 in ./venv3/lib/python3.12/site-packages (from jedi>=0.16->ipython>=7.23.1->ipykernel->jupyter) (0.8.3)
Requirement already satisfied: attrs>=22.2.0 in ./venv3/lib/python3.12/site-packages (from jsonschema>=4.18.0->jupyterlab-server<3,>=2.22.1->notebook->jupyter) (23.2.0)
Requirement already satisfied: jsonschema-specifications>=2023.03.6 in ./venv3/lib/python3.12/site-packages (from jsonschema>=4.18.0->jupyterlab-server<3,>=2.22.1->notebook->jupyter) (2023.12.1)
Requirement already satisfied: referencing>=0.28.4 in ./venv3/lib/python3.12/site-packages (from jsonschema>=4.18.0->jupyterlab-server<3,>=2.22.1->notebook->jupyter) (0.33.0)
Requirement already satisfied: rpds-py>=0.7.1 in ./venv3/lib/python3.12/site-packages (from jsonschema>=4.18.0->jupyterlab-server<3,>=2.22.1->notebook->jupyter) (0.17.1)
Requirement already satisfied: python-json-logger>=2.0.4 in ./venv3/lib/python3.12/site-packages (from jupyter-events>=0.9.0->jupyter-server<3,>=2.4.0->notebook->jupyter) (2.0.7)
Requirement already satisfied: pyyaml>=5.3 in ./venv3/lib/python3.12/site-packages (from jupyter-events>=0.9.0->jupyter-server<3,>=2.4.0->notebook->jupyter) (6.0.1)
Requirement already satisfied: rfc3339-validator in ./venv3/lib/python3.12/site-packages (from jupyter-events>=0.9.0->jupyter-server<3,>=2.4.0->notebook->jupyter) (0.1.4)
Requirement already satisfied: rfc3986-validator>=0.1.1 in ./venv3/lib/python3.12/site-packages (from jupyter-events>=0.9.0->jupyter-server<3,>=2.4.0->notebook->jupyter) (0.1.1)
Requirement already satisfied: ptyprocess>=0.5 in ./venv3/lib/python3.12/site-packages (from pexpect>4.3->ipython>=7.23.1->ipykernel->jupyter) (0.7.0)
Requirement already satisfied: charset-normalizer<4,>=2 in ./venv3/lib/python3.12/site-packages (from requests>=2.31->jupyterlab-server<3,>=2.22.1->notebook->jupyter) (3.3.2)
Requirement already satisfied: urllib3<3,>=1.21.1 in ./venv3/lib/python3.12/site-packages (from requests>=2.31->jupyterlab-server<3,>=2.22.1->notebook->jupyter) (2.2.0)
Requirement already satisfied: certifi>=2017.4.17 in ./venv3/lib/python3.12/site-packages (from requests>=2.31->jupyterlab-server<3,>=2.22.1->notebook->jupyter) (2023.11.17)
Requirement already satisfied: argon2-cffi-bindings in ./venv3/lib/python3.12/site-packages (from argon2-cffi->jupyter-server<3,>=2.4.0->notebook->jupyter) (21.2.0)
Requirement already satisfied: executing>=1.2.0 in ./venv3/lib/python3.12/site-packages (from stack-data->ipython>=7.23.1->ipykernel->jupyter) (2.0.1)
Requirement already satisfied: asttokens>=2.1.0 in ./venv3/lib/python3.12/site-packages (from stack-data->ipython>=7.23.1->ipykernel->jupyter) (2.4.1)
Requirement already satisfied: pure-eval in ./venv3/lib/python3.12/site-packages (from stack-data->ipython>=7.23.1->ipykernel->jupyter) (0.2.2)
Requirement already satisfied: fqdn in ./venv3/lib/python3.12/site-packages (from jsonschema[format-nongpl]>=4.18.0->jupyter-events>=0.9.0->jupyter-server<3,>=2.4.0->notebook->jupyter) (1.5.1)
Requirement already satisfied: isoduration in ./venv3/lib/python3.12/site-packages (from jsonschema[format-nongpl]>=4.18.0->jupyter-events>=0.9.0->jupyter-server<3,>=2.4.0->notebook->jupyter) (20.11.0)
Requirement already satisfied: jsonpointer>1.13 in ./venv3/lib/python3.12/site-packages (from jsonschema[format-nongpl]>=4.18.0->jupyter-events>=0.9.0->jupyter-server<3,>=2.4.0->notebook->jupyter) (2.4)
Requirement already satisfied: uri-template in ./venv3/lib/python3.12/site-packages (from jsonschema[format-nongpl]>=4.18.0->jupyter-events>=0.9.0->jupyter-server<3,>=2.4.0->notebook->jupyter) (1.3.0)
Requirement already satisfied: webcolors>=1.11 in ./venv3/lib/python3.12/site-packages (from jsonschema[format-nongpl]>=4.18.0->jupyter-events>=0.9.0->jupyter-server<3,>=2.4.0->notebook->jupyter) (1.13)
Requirement already satisfied: cffi>=1.0.1 in ./venv3/lib/python3.12/site-packages (from argon2-cffi-bindings->argon2-cffi->jupyter-server<3,>=2.4.0->notebook->jupyter) (1.16.0)
Requirement already satisfied: pycparser in ./venv3/lib/python3.12/site-packages (from cffi>=1.0.1->argon2-cffi-bindings->argon2-cffi->jupyter-server<3,>=2.4.0->notebook->jupyter) (2.21)
Requirement already satisfied: arrow>=0.15.0 in ./venv3/lib/python3.12/site-packages (from isoduration->jsonschema[format-nongpl]>=4.18.0->jupyter-events>=0.9.0->jupyter-server<3,>=2.4.0->notebook->jupyter) (1.3.0)
Requirement already satisfied: types-python-dateutil>=2.8.10 in ./venv3/lib/python3.12/site-packages (from arrow>=0.15.0->isoduration->jsonschema[format-nongpl]>=4.18.0->jupyter-events>=0.9.0->jupyter-server<3,>=2.4.0->notebook->jupyter) (2.8.19.20240106)

(venv3) nishanth@Chandans-Air ~ % which jupyter
/Users/nishanth/venv3/bin/jupyter
(venv3) nishanth@Chandans-Air ~ % python3 -m pip freeze | grep jupyter
jupyter==1.0.0
jupyter-console==6.6.3
jupyter-events==0.9.0
jupyter-lsp==2.2.2
jupyter_client==8.6.0
jupyter_core==5.7.1
jupyter_server==2.12.5
jupyter_server_terminals==0.5.2
jupyterlab==4.0.12
jupyterlab-widgets==3.0.9
jupyterlab_pygments==0.3.0
jupyterlab_server==2.25.2

(venv3) nishanth@Chandans-Air ~ % python -m jupyter
usage: jupyter.py [-h] [--version] [--config-dir] [--data-dir] [--runtime-dir] [--paths] [--json] [--debug] [subcommand]

Jupyter: Interactive Computing

positional arguments:
  subcommand     the subcommand to launch

options:
  -h, --help     show this help message and exit
  --version      show the versions of core jupyter packages and exit
  --config-dir   show Jupyter config dir
  --data-dir     show Jupyter data dir
  --runtime-dir  show Jupyter runtime dir
  --paths        show all Jupyter paths. Add --json for machine-readable format.
  --json         output paths as machine-readable json
  --debug        output debug information about paths

Available subcommands: console dejavu events execute kernel kernelspec lab labextension labhub migrate nbconvert notebook qtconsole run server
troubleshoot trust

Please specify a subcommand or one of the optional arguments.
(venv3) nishanth@Chandans-Air ~ % deactivate
nishanth@Chandans-Air ~ % git init
Reinitialized existing Git repository in /Users/nishanth/.git/

nishanth@Chandans-Air ~ % ls
Applications            Homework1               Pictures                dir2                    nishblaze.pem
Desktop                 Library                 Public                  dirl                    requirements.txt
Documents               Movies                  README.md               hwcam.py                us-counties.csv
Downloads               Music                   camcodehw.py            ner.dataset.jsonl       venv3
nishanth@Chandans-Air ~ % git add requirements.txt
nishanth@Chandans-Air ~ % git commit -m "Add requirements.txt file for camcodehw"

Auto packing the repository in background for optimum performance.
See "git help gc" for manual housekeeping.
[main 4144f87] Add requirements.txt file for camcodehw
 Committer: Nish Chandan <nishanth@Chandans-Air.lan>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 104 insertions(+)
 create mode 100644 requirements.txt
nishanth@Chandans-Air ~ % git push origin main

Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 1.30 KiB | 1.30 MiB/s, done.
Total 3 (delta 0), reused 3 (delta 0), pack-reused 0
To https://github.com/nishblaze7/CamcodeHW1
   90f6578..4144f87  main -> main
