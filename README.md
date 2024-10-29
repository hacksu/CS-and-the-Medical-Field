# CS-and-the-Medical-Field

## What is the role of technology in the health field?
Health and technology have always been involving since the beginning of the human race. Early on, paper, the wheel, and even glue were created and we still use today.
The medical field is the same way. The first civilizations used medicnial plants in order to relieve pain, and now those plants are the basis for a ton of different medicines. 
As the years went on technology and the medical field influenced each other. When paper was created, case studies and diseases were documents and we can still see some of those documents today.
Now technology and medicine are progressing more rapidly now than ever. With the creation of the computer and the internet the medical field exploded. 
Now it is easy to share research and ideas and collaborate with others all over the world. Currently there's been some interesting intersections between biology and technology.
### Bread and Cancer???
Back in 2017 a Japanese bakery would bake a million different pastries and to someone who is not a pastry expert I have no clue what anything is. So during checkout you would place whatever pastry into 
a rectangluar box and you would look at a screen and there would be a bunch of different little green lines and it would tell you want you got and the price. 
This greatly helped the cashiers and allowed the bakery to produce a wider variety of pastries. Well you know what a bunch of pastries apparently looks like?
Cancer cells... A partnership between a bakery and medical research began. Now this same program is being used for a wide variety of issues in the medical field 
and is still in use at that bakery. 
### There's a computer made of human brain cells? 
More recently, back in June, a biocomputer was created. A swiss startup called FinalSpark created a biocomputer with 16 mini-brains. So the human brain is actually 
super efficient. We have over 86 billion neurons and it's amazing what they are capable of. For this to be used as a computer is an interesting idea. 
This consumes a million times less power than a traditional computer. This could greatly reduce the environmental impact of classical computers. They are
currently training this computer to handle large language models and it will be interesting to see how it performs. 

## Robotic Surgery
How many of you would feel comforatable having surgery done by a robot? 
Advancements in robotics has improved healthcare greatly. Robotics can improve surgical outcomes, improve bedside care, and can even help in therapy. 
### Intuitive da Vinci
It's rated as one of the best surgical systems for minimally invasive surgery. It allows the surgeon to control the instruments with more accuracy and to be able to give a magnified view.
There's more than 1,700 of these systems worldwide and this number keeps growing.It is primarily used for heart surgeries, general surgeries, and gynecologolical procedures and over 7 million procedures have been done.
This robot has many benefits like less blood loss, smaller incisions, less pain, and fewer surgical complications. 
### CyberKnife
The CyberKnife is a non-invasive tumor treatment. It is a robot that can deliver percision radiation therapy which allows it to focus on the tumor while keeping the surrounding 
tissue safe. It can account for someone breathing or a patient turning their head. It can determine where the tumor is and then focus on it while it is giving treatment. Treatment takes 
around 45 minutes of 1-5 visits which is an improvement over current radiation therapies. 
### Paro Therapeutic Robot
Ok this thing is honestly kinda cute (minus the fact that it's a robot). Do this little thing has been proven to reduce stress, improves relaxation, and is certified by Guinness World Records
as the most therapeutic robot. It's capable of sensing light, voice, and touch. It acts like a pet pretty much. It's currently being used for those who have dementia and Alzheimer's. It will also 
learn the patient's behavior and adjust accordingly. I don't know how I feel about that part but overall it's pretty cute and I like the idea. Well if you want one of these be ready to spend over $6,000.
It also has been tested on a mars mission simulation to reduce stress. 

## Brain Tumor Analysis: Notebook by: Zeeshan Latif https://www.kaggle.com/code/zeeshanlatif/brain-tumor-segmentation-using-u-net/notebook
So now into the actual lesson. I am going to need everyone to create a kaggle account. https://www.kaggle.com/ Kaggle is one of the largest AI and machine learning 
communities and they host their own challenges and even some courses related to data science. So pretty much with the advancements of technology the medical Field
is now adopting AI, ML, and quantum computing methods in order to solve different medical and scientific issues. So in this case we will be using U-net.
It's a convolutional neural network which is primarily used for image segmentation. So we are using this since it requires fewer training images. 
This is actually used quite a bit in medical research since it can be useful in identifying brain tumors. So first we need to pre-process the data. It's a bunch of brain MRI scans. So I'm not going to cover the data pre-processing steps. So as we go through this analysis I want you to keep in mind 
4 different modulalities that help us identify brain tumors. T1 is used to find tissue structure. T1ce is used to help identify abnormalities. T2 helps visualize
fluid content and FLAIR makes it easier to find lesions specifically in the white matter. In this case we are only interested in T1ce and FLAIR. 

So in the brain we need to keep in mind the 3 planes. Transverse, Coronal, and Sagittal planes. Tranverse divides the brain horizontally. Coronal divides it into front and back.
Sagittal divides the brain into left and right. Each plane can give us a different insight into the brain and it's functions. So the next part will show the brain in each of these views. 
We can see where the tumor is. We will look at the sagittal view first. We can see an entire range of the brain in quite a few different slices. Well that's a lot of slices, we can reduce this so we only keep the 
ones that we are interested in. From this we can identify where the tumor is, what it looks like, how the surrounding tissue is impacted. From this we can isolate the tumor. 
We can categorize the different parts into classes. class 0 which is not a tumor, class 1 which is a non-enhancing tumor (lacks iodine), class 2 which is an edema (swelling due to fluid buildup), class 4 which is an enhancing tumor (the actual tumor).

So now we need to split the data set. So 70ish percent will be used for training, about 15 percent for the validation set and another 15 percent for the final testing set. So now we can get started on training the neural network. We will need the raw data and 
the ground truth which is what the model is attempting to simulate. So again I'm gonna skip over the preprocessing. Let's say there's a ton of steps but pretty much we wanted to avoid overloading the neural network, narrowed down our training data and shaped it so
it can be used in our analysis. So we wanted to select a single slice and be able to view it using the FLAIR, T1ce, and the colored segmentation views. So while we are training the model we need to keep in mind the loss function. This is pretty much a formula that allows us to 
see how well a model is performing. So more specifically we will be using the Dice loss function which allows us to see the overlap of the predicted and actual segmentation. So back to the U-net stuff. We want to be able to segment small regions and this is perfect for what we are doing. 
We will be using the 2D version since it's faster and easier to work with for larger datasets. Now we can train our model. After it's done running we can see the different metrics in order to see how it's doing. the 1st graph shows that accuracy increases over time which is what we hope to see.
The second graph is the loss graph which shows the loss decreases over time. I don't personally care about the right 2 graphs. Now we can use our model to analyze the rest of the brain scans. We can see the different classes being predicted and I think it did a good job. 
Let's try another slice. Still fairly good. 


## Resources
The History of Technology: https://en.wikipedia.org/wiki/History_of_technology#:~:text=In%20navigation%2C%20the%20foundation%20to,armour%2C%20steel%20crossbows%20and%20cannon.
The History of Medicine: https://en.wikipedia.org/wiki/History_of_medicine
Bread AI: https://www.newyorker.com/tech/annals-of-technology/the-pastry-ai-that-learned-to-fight-cancer
Biocomputer: https://www.sciencealert.com/swiss-startup-connects-16-human-mini-brains-to-create-low-energy-biocomputer and https://www.frontiersin.org/journals/artificial-intelligence/articles/10.3389/frai.2024.1376042/full
Intuitive Da Vinci Robot: https://www.intuitive.com/en-us/products-and-services/da-vinci
Paro: http://www.parorobots.com/
CyberKnife: https://cyberknife.com/



