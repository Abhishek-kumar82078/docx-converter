# Docxconverter
A full-stack website application to convert a word document into either pdf, XML, or text format. <br>
Tech stack used : HTML5, CSS3, JavaScript, FastApi, Python, AJAX, jQuery
### Some highlighted features of this application:-
- Take a word document and the required format as input.
- Convert that file into the required format among any of the three formats XML, text, or pdf. 
- Return the converted file with the same name as that of the input which can be viewed as well as downloaded
- Releases log messages for every action it starts performing. Hence easy to debug and fix the error when generated.


### This application also make use of 3 modules:-
- <a href="https://pypi.org/project/docx2txt/"> docx2txt==0.8 </a> for converting to text format
- <a href="https://pypi.org/project/docx-utils/"> docx_util </a> for converting to XML format
- <a href="https://pypi.org/project/docx2pdf/"> docx2pdf </a> for converting to pdf format

## This project can be used in two ways. 
### A. Use the UI to convert your file.<br> B. Use the backend code either to convert your file or use the API to implement your own project.

### 1. Follow the below steps to use the UI to convert your file:- <br>
- Step 1 : Select the docx file by clicking on the button or drag and drop the file
<div align="center">
<img width="409" alt="image" src="https://user-images.githubusercontent.com/63895917/182398096-c60b5438-6940-4f79-8df7-580d36df4a9d.png">
</div>

- Step 2 : Choose the required format from XML, pdf, or txt by clicking on their respective image. When it will be selected there will be a dark purple background signifying that the format has been chosen. Since those are radio buttons only one will be selected at a time. 
<div align="center">
<img width="340" alt="image" src="https://user-images.githubusercontent.com/63895917/182400569-b7cfbdd4-7b64-4ced-8368-14c50cbc223f.png">
</div>

- Step 3 : Click on the convert button and it will start converting your file landing you on the loading page.
<div align="center">
<img width="227" alt="image" src="https://user-images.githubusercontent.com/63895917/182402923-bfac4550-ee2b-4176-aa88-59ee7b13afe3.png">
</div>


##### Your task is now finished. Simply relax as your file will be converted in just a fraction of a second.


- Step 4 : You will be taken to a different page where you can view your converted file.
<div align="center">
<img width="466" alt="image" src="https://user-images.githubusercontent.com/63895917/182403708-8383b61b-bd1b-4729-8806-b08ec4a61381.png">
</div>

- Step 5 : Finally, you can download your converted file by clicking on the download button.
<div align="center">
<img width="291" alt="image" src="https://user-images.githubusercontent.com/63895917/182403974-c7cc20b4-0dd9-4e4f-8688-69c94a2174d3.png">
</div>

## Its backend part can be utilized independently as a module and imported into your project as needed. 
Get the <a href="https://github.com/Abhishek-kumar82078/docx-converter/tree/main/backend"> code here </a>.

Backend part has been implemented using FastAPI. <a href="https://fastapi.tiangolo.com/">FastAPI </a> is a modern, fast (high-performance), web framework for building APIs with Python 3.6+ based on standard Python type hints.


### 2. Follow the below steps to use the backend code to convert your file:

- Create a virtual environment after deciding a directory where you want to place it, and run the venv module as a script with the directory path:
```
      python3 -m venv local-env
```

- Once you’ve created a virtual environment, activate it as 

```
      local-env/scripts/activate
```
on Windows Or
```
      source local-env/bin/activate
```
 on Unix or MacOS.
 
 - Installs all of the modules listed in my Python requirements file into your project environment using
 
 ```
pip install -r requirements.txt
```

- Make a small changes in the main.py file present inside backend directory. Replace
```
 return {"Destination File Path": dest_file} 
 ```
 with
 ```
 return {"Destination File Path": f"{SERVER_ADDRESS}/output_files/{dest_file}"} 
```
- Navigate to the backend directory and then run your application using the below command:
```
uvicorn main:app --raload
```

- You can now go to the below URL and try uploading the file and format
```
http://127.0.0.1:8000/docs
```

- Click on "Try it out" in top right corner as shown in the image.
<img width="929" alt="image" src="https://user-images.githubusercontent.com/63895917/182897318-83d4a1ef-1f69-4346-bdec-ee742d908ace.png">

- Now choose the file by clicking on "Choose File" input, enter the required format, and click on the "Execute" button.
<img width="919" alt="image" src="https://user-images.githubusercontent.com/63895917/183115627-d92891e1-92f7-4afb-80a0-536b99d1b34f.png">

- As soon as you click on the "Execute" button, the program will start its execution and return you a destination file path as the response.
<img width="915" alt="image" src="https://user-images.githubusercontent.com/63895917/183116362-9043bc2f-ff4e-49ab-bcfd-975245e8c2ff.png">

- Go to the URL provided in the response body as above and you will get your converted file. Url is like:
```
127.0.0.1:8000/output_files/sample05082022_212849.pdf
```


### Finally, your file has been converted.
## Cheers!
