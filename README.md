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
- Step 1 : Select the docx file by clicking on the button or drag and drop the file
<div align="center">
<img width="409" alt="image" src="https://user-images.githubusercontent.com/63895917/182398096-c60b5438-6940-4f79-8df7-580d36df4a9d.png">
</div>

- Step 2 : Choose the required format from xml, pdf, or txt by clicking on their respective image. When it will be selected their will be dark purple background signifing that the format has been choosen. Since, those are radio button only one will be selected at a time. 
<div align="center">
<img width="340" alt="image" src="https://user-images.githubusercontent.com/63895917/182400569-b7cfbdd4-7b64-4ced-8368-14c50cbc223f.png">
</div>

- Step 3 : Click on convert button and it will start converting your file landing you to the loading page.
<div align="center">
<img width="227" alt="image" src="https://user-images.githubusercontent.com/63895917/182402923-bfac4550-ee2b-4176-aa88-59ee7b13afe3.png">
</div>


##### Your task is now finished. Simply relax as your file will be converted in just a fraction of a second.


- Step 4 : You will be taken to a different page where you can view your converted file.
<div align="center">
<img width="466" alt="image" src="https://user-images.githubusercontent.com/63895917/182403708-8383b61b-bd1b-4729-8806-b08ec4a61381.png">
</div>

- Step 5 : Finally, you can download your converted file by clicking on download button.
<div align="center">
<img width="291" alt="image" src="https://user-images.githubusercontent.com/63895917/182403974-c7cc20b4-0dd9-4e4f-8688-69c94a2174d3.png">
</div>

### Its backend part can be utilized independently as a module and imported into your project as needed. 
Get the <a href="https://github.com/Abhishek-kumar82078/docx-converter/tree/main/backend"> code here </a>.

Backend part has been implemented using FastAPI. <a href="https://fastapi.tiangolo.com/">FastAPI </a> is a modern, fast (high-performance), web framework for building APIs with Python 3.6+ based on standard Python type hints.



To run this project follow the following steps:
- Activate virtual environment as "venv/scripts/activate" in windows.
- Install all the requirements as "pip install -r requirements.txt".
- Run the backend after navigating to backend folder as uvicorn main:app --raload or you can directly run from current directory also but make sure to provide correct path.
- Open the index.html in frontend folder in your browser and enjoy using the application.

## Cheers!
