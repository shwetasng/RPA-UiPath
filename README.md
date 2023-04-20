# RPA-UiPath
This UiPath Studio project features an RPA Bot designed to create a personalized unicorn name for you, which will then be displayed on the screen.

## Steps to install UiPath Studio in your system 
- Step 1: Link: https://bit.ly/3rOHDkd >> option on the right side >> sign up for UiPath Automation Cloud for community 
- Step 2: Download UiPath Studio (not StudioX):
Once inside the Automation Cloud click on the first blue button Download UiPath Studio
- Step 3: Run the UiPath Studio installer
- Step 4: Sign into UiPath Automation Cloud from UiPath Studio

## RESOURCES:
https://docs.uipath.com/installation-and-upgrade/docs/studio-install-studio

## STEPS TO MAKE YOUR FIRST BOT

1. First open your UiPath studio Community app, then to create a new bot we select Process from New Project
<img width="600" alt="image" src="https://user-images.githubusercontent.com/103261868/233266256-5262fd2a-d60f-4f43-b14f-4d3afbf3a0b8.png">
2. Give name to the process and change the location according to you then create.
<img width="332" alt="image" src="https://user-images.githubusercontent.com/103261868/233266446-58f14ffe-e21e-4c4b-85e4-76bfdb7be6a1.png">
3. Design window for the bot will then open and we can give instructions to the bot in the main sequence.
<img width="600" alt="image" src="https://user-images.githubusercontent.com/103261868/233266648-0f712045-309f-4efc-98fc-f48ef2c34e5b.png">
4. In the left search bar of Activities search for input dialog.
<img width="230" alt="image" src="https://user-images.githubusercontent.com/103261868/233266793-932dff10-8c5b-49cd-9629-35ceb58889e3.png">
5. Drag and Drop the input dialog in main sequence.
<img width="500" alt="image" src="https://user-images.githubusercontent.com/103261868/233266880-62a72b33-eff7-4885-8020-c7b1daab1742.png">
6. input values in the dialog box as given in the picture below and in the field 'value entered' using Ctrl+K put str_name
<img width="242" alt="image" src="https://user-images.githubusercontent.com/103261868/233267070-47cc912d-46ae-4310-b2e9-0d4a9fba4b4c.png">
7. Drag and drop one more input dialog just below the previous one.
<img width="240" alt="image" src="https://user-images.githubusercontent.com/103261868/233267174-89e2e2a1-02ad-4ebe-99f7-da077f3696da.png">
8. Enter the values in this as well just like in the previous one.
<img width="242" alt="image" src="https://user-images.githubusercontent.com/103261868/233267526-44b71c48-f641-4205-9afd-6e6d44930cb9.png">
9. Now search for open browser.
<img width="227" alt="image" src="https://user-images.githubusercontent.com/103261868/233267368-f606927e-d22c-4a1f-8619-f4c5283d46d2.png">
10. Drag and drop the open browser below the input dialog.
<img width="290" alt="image" src="https://user-images.githubusercontent.com/103261868/233267621-1c2c3119-ff5a-4a1f-ba78-973bc21d9bbf.png">
11. In the open browser insert the url of website https://www.rpasamples.com/unicornname
<img width="260" alt="image" src="https://user-images.githubusercontent.com/103261868/233267926-6c9662ca-ad3b-4fe6-b276-5c3e25754d34.png">
12. Search for type into
<img width="227" alt="image" src="https://user-images.githubusercontent.com/103261868/233268090-8a96a407-97da-4a96-9a7f-e742d609f176.png">
13. Drag and drop type into in the do section of open browser.
<img width="290" alt="image" src="https://user-images.githubusercontent.com/103261868/233268603-eb1ba217-5de1-46da-94f9-6a1c572a32d1.png">
14. select enter your name as screenshot for type into and put variable as str_name
<img width="600" alt="image" src="https://user-images.githubusercontent.com/103261868/233268668-4aa4104a-dc4f-41b9-b7cc-12175c29d596.png">
15. Search for 'click'.
<img width="230" alt="image" src="https://user-images.githubusercontent.com/103261868/233268794-dcd03d9e-1092-446f-8b87-a951e321925a.png">
16. Drag and drop 'search just below 'type into' in the do section of open browser.
<img width="500" alt="image" src="https://user-images.githubusercontent.com/103261868/233268933-69d873d6-6832-4fa7-ad85-6c397e6123ec.png">
17. Choose 'get name' from the website.
<img width="206" alt="image" src="https://user-images.githubusercontent.com/103261868/233269079-17a3c936-b3ee-4848-b37e-a1142304723a.png">
18. Search for 'get text'
<img width="228" alt="image" src="https://user-images.githubusercontent.com/103261868/233269196-0d0dfbd7-5607-491c-bfe0-20fdc50ae41f.png">
19. Drag and drop 'get text' below the get name and select 'unicorn name' from the website on browser.
<img width="202" alt="image" src="https://user-images.githubusercontent.com/103261868/233269239-1a65bda0-1cc6-42c4-959f-6d83347181d1.png">
<img width="188" alt="image" src="https://user-images.githubusercontent.com/103261868/233269556-59dec66f-f049-4577-8126-c9d58154e68b.png">
20. For the 'get text' on the right side enter the OUTPUT Value, using Ctrl+K give it's value as str_unicornname
<img width="500" alt="image" src="https://user-images.githubusercontent.com/103261868/233269726-ff51d929-e620-4291-9055-63026f1ce6eb.png">
21. Search for 'message'.
<img width="229" alt="image" src="https://user-images.githubusercontent.com/103261868/233269867-a13063cd-b8e2-4efe-9c00-087303bae3d3.png">
22. Drag and drop it outside 'Open Browser'.
<img width="293" alt="image" src="https://user-images.githubusercontent.com/103261868/233269952-378c9fe4-246e-4d55-bd0d-8dd8e2bf4b51.png">
23. In the text section put the desired message you want to print for eg: "Hello"+str_name+"Your Unicorn Name Is"+str_unicornname   you might see some error in this this is because the variable str_unicornname is not in global scope and it can be done so by changing its scope to Main Sequence from the variables section.
<img width="494" alt="image" src="https://user-images.githubusercontent.com/103261868/233270374-3cb389cd-5db4-4e83-8e09-2b249973f839.png">
24. Now we can run the file from Debug File drop down on left side on top of screen.
<img width="226" alt="image" src="https://user-images.githubusercontent.com/103261868/233270710-6ad49417-724b-4367-9db2-e7a88580e973.png">
25. Enter your name and then required password length as we specified in the input dialog box
<img width="248" alt="image" src="https://user-images.githubusercontent.com/103261868/233270565-166b5e48-aab8-4911-9f49-c4243c45cfa3.png">
26. You will then see a message box will be automatically generated having your username and your unicornname.
<img width="500" alt="image" src="https://user-images.githubusercontent.com/103261868/233272177-6ab28c8d-3828-4ac5-b338-c7eb88263b1e.png">

## "YAYY!!😃 YOU'VE FINALLY MADE YOUR FIRST BOT WHICH GENERATES A MESSAGE BOX WITH YOUR USERNAME AND YOUR UNICORN NAME"




