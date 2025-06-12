# Checks #
python3 --version
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
uv tool install crewai
uv tool list
uv tool install crewai --upgrade

## ONLY IF YOU ARE DOING IT FOR THE START OF A PROJECT ##
## Creating a CREW   ##           
crewai create crew <your_project_name>

## ONLY IF YOU ARE DOING IT FOR THE START OF A PROJECT
## Creating a Flow ##
crewai create flow travelagent 

## SET INTO YOUR VIRTUAL ENVIRONMENT  ##
python -m venv ta_env
source ta_env/Scripts/activate

## In Windows ##
./ta_env\Scripts\Activate.bat

## INSTALL ALL DEPDENDENCIES { Takes a while } ##
crewai install
pip install streamlit
pip install markdown
pip install crewai
pip install crewai_tools

## Run from the src directory ##
streamlit run streamlit_app.py

