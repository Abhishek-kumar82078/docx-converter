# Docxconverter
A full-stack website application to convert a word document into either pdf, XML, or text format. <br>
Tech stack used : HTML5, CSS3, JavaScript, FastApi, Python, AJAX, jQuery
### Some highlighted features of this project:-
- Take a word document and the required format as input.
- Convert that file into the required format among any of the three formats XML, text, or pdf. 
- Return the converted file with the same name as that of the input which can be visualized as well as downloaded
- Releases log messages for every action it start performing. Hence easy to debug anf fix the error when generated.
<br>
This also make use of 3 modules - docx2txt==0.8, docx_util & docx2pdf. 

### Steps to be followed to convert your file:-
- Step 1 : Select the 

To run this project follow the following steps:
- Activate virtual environment as "venv/scripts/activate" in windows.
- Install all the requirements as "pip install -r requirements.txt".
- Run the backend after navigating to backend folder as uvicorn main:app --raload or you can directly run from current directory also but make sure to provide correct path.
- Open the index.html in frontend folder in your browser and enjoy using the application.

## Cheers!
