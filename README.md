**Idea:** <br />  
Climate change is one of the biggest issues that we as a human race face, and one of the biggest contributors to this problem is rubbish. Unfortunately, due to the lack of proper recycling, waste often gets piled up in landfills, leading to toxins and greenhouse gas emissions. One way that we can help curb this problem is making sure we dispose of our waste properly. 

In Victoria where I’m from rubbish is separated into three different bins: recyclables, waste, and organic. However, there are some countries such as Japan who have taken a far tougher stance on recycling, having to split their waste into 10 or more different categories. This is where my idea comes in, an AI that is able to visually detect and differentiate the different types of rubbish there are, and understand which bins they have to be placed in. This is handy, as learning how to properly differentiate your trash can be an arduous task, a task which instead could be automated easily using artificial intelligence. 
To keep it simple I am developing an AI that will just detect and sort rubbish into the three categories that are available in Victoria using just a picture of the trash. 

**Approach:**

As someone with minimal experience in coding, I am choosing to approach this problem using the Azure Custom Vision AI service. This service is extremely helpful in the fact that it enables users to create object detection models with minimal deep learning expertise and fewer training images. 

Data phase: The main data that I need to collect are various pictures of different types of rubbish so that the custom vision service is able to detect which bin they belong in. The way that the service is trained is by uploading pictures, and then tagging the classes and bounding box coordinates of each object. I decided to separate my objects into their bin types: recyclables, organic, and waste.  

Model phase: With enough pictures, the Azure Custom Vision AI service can then easily train the model and will then evaluate the images using the following metrics: precision, recall, and mean average precision. 

Deployment phase: For the time being the data would be deployed using Jupyter Notebooks. Of course, the AI could still miss out or make mistakes on specific objects, therefore it would be good to get manual feedback from the user where they specify the location and the type of object when something is wrong it is so that the model can continuously learn and grow as time goes on, continuing the machine learning life cycle. 

**Principiles:**
Privacy and security - The project will delete all images once taken
Reliability and safety - Product is very safe and reliable, only detects trash 
Transparency - Will be very clear on the purpose of project, and what is done with obatained information and data 


If I were to expand my idea, I would add a live camera feature similar to google translates’ way of translating language using the phone’s camera so that it is more accessible and usable.   
