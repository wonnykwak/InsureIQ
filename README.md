# InsureIQ
5C Hackathon - Health & Equity Track Winner

Team Members: Nannapas Wonghirundacha, Wonny Kwak, Elly Rokeach

During an emergency at Pomona College, an international student hesitated to call an ambulance due to uncertainty about their health insurance coverage. Many students at Pomona, including all international students, are enrolled in the Student Health Insurance Program (SHIP). However, accessing and understanding the specific coverage details can be challenging. Contributing factors include the complexity of insurance plans, the confusing format of data in the PDF documents, and limited guidance provided by the college. As a result, students may struggle to determine what is and isn't covered, particularly in high-stress emergency situations.

For these reasons, we chose to approach the Health Equity track, and we built a platform that takes a user’s question as input, searches through the data in the PDFs, and finds the most relevant information, and then returns and displays this information in a simplified format to the user. This will help students have more efficient access to information about what SHIP actually covers, which will be especially useful in emergency situations. Our project applies to the Data & Analytics and Beginner overlays.

Since the SHIP information and coverage is standardized across all students, there are no ethical implications of our project that could potentially jeopardize student safety or privacy. All we are attempting to do is make information about insurance coverage more accessible. While we were developing, we noticed that there was a potential for harm when the AI model was generating its own relevant categories based on the user input. We addressed this issue by ensuring that the model continues to run and produce outputs until they are in the correct format.

We used Adobe Acrobat to convert the PDFs into Microsoft Excel spreadsheets. Then, we manipulated the data into tables, removing unnecessary information. We then loaded this data from the excel spreadsheets into a Python script using the pandas library. We also used the OpenAI API to perform a search for the most relevant categories based on the user’s inputted prompt. Then we generate extracted data of all the rows underneath each relevant category. We used Django to build the backend of our webpage, and React to create the front-end. We then combined our data extraction algorithm with the webpage. We don’t have a fully functional web-page yet, but ideally, the user would be able to input a question into the search bar, and then the relevant information will be displayed underneath.
