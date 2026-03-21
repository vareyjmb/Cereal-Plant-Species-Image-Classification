Laboratory Work 2-A Activity — Plant Species Image Classification

Using Teachable Machine

Activity Overview
In this activity, you will design, train, evaluate, and document an image classification model that
recognizes 20 related plant species using Google Teachable Machine. You will also document your
entire process and results using GitHub, following proper dataset handling, model evaluation, and accuracy
practices.

Learning Objectives
By the end of this activity, you should be able to:
● Organize and classify an image dataset for machine learning
● Train an image classification model using Teachable Machine
● Analyze model performance using confusion matrices and accuracy metrics
● Test and export a trained ML model
● Document an ML project using GitHub and Markdown

Tools & Platforms
● Google Teachable Machine (Image Project)
● Google Drive
● GitHub (with README.md)
● Screenshot tool (Snipping Tool / Screenshot / Print Screen)

-------

Plant Species
Below are the plant species used in this project.
-------
1.Wheat
Common Name: Wheat
Scientific Name: Triticum aestivum

Description: Wheat is one of the most widely cultivated cereal crops. It is used to produce flour for bread, pasta, and other food products.
![wheat](https://github.com/user-attachments/assets/170459cb-b9ec-4f42-bd04-6927350a457f)
-------
2.Triticale
Common Name: Triticale
Scientific Name: Triticosecale

Description: Triticale is a hybrid of wheat and rye, combining the yield of wheat with the hardiness of rye. It is mainly used for animal feed.
![Triticale](https://github.com/user-attachments/assets/a1db7f17-bdc9-4cc4-8615-230f870c069a)
-------
3.Teff
Common Name: Teff
Scientific Name: Eragrostis tef

Description: Teff is a tiny-grained cereal crop native to Ethiopia. It is used to make traditional flatbread and is rich in nutrients.
![000270](https://github.com/user-attachments/assets/deb162eb-007d-47a7-b7f2-d8a453f01dbb)

--------
4.Spelt
Common Name: Spelt
Scientific Name: Triticum spelta

Description: Spelt is an ancient wheat species with a nutty flavor. It is used in baking and is valued for its nutritional properties.
![000291](https://github.com/user-attachments/assets/702e77a4-e28e-4aae-97fb-25fe59ae82e7)

-----------

5.Sorghum
Common Name: Sorghum
Scientific Name: Sorghum bicolor

Description: Sorghum is a drought-tolerant cereal crop used for food, fodder, and biofuel production. It produces tall stalks and grain heads.
![000283](https://github.com/user-attachments/assets/a716020f-a83b-4eb5-bb36-4d8cb18a965e)

----------
6.Rye
Common Name: Rye
Scientific Name: Secale cereale
Description: Rye is a hardy cereal grain that grows in cold climates. It is commonly used for bread, whiskey, and animal feed..
![000253](https://github.com/user-attachments/assets/c3590c40-d520-4be1-bbd2-275397cbd2b7)

-----------
7.Rice
Common Name: Rice
Scientific Name: Oryza sativa

Description: Rice is a staple cereal crop grown in flooded fields. It is a primary food source for a large portion of the global population.
![000156](https://github.com/user-attachments/assets/d1d09c30-52a2-470a-b220-753b9ba31e95)

--------
8.Amaranth
Common Name: Amaranth
Scientific Name: Amaranthus cruentus

Description: Amaranth is a fast-growing cereal-like plant cultivated for its nutrient-rich seeds and edible leaves. It thrives in warm climates and is valued as both a grain and leafy vegetable.
![000006](https://github.com/user-attachments/assets/21f1c183-ef3b-457a-b3b8-45a0c5fee2a9)

-------
9.Barley
Common Name: Barley
Scientific Name: Hordeum vulgare

Description: Barley is a major cereal grain used for food, animal feed, and brewing. It grows in temperate regions and produces long, slender spikes of grain.
![000005](https://github.com/user-attachments/assets/80f09970-03dc-4e21-922e-a08781b1d3d2)

---------
10. Buckwheat
Common Name: Buckwheat
Scientific Name: Fagopyrum esculentum

Description: Buckwheat is a pseudocereal known for its triangular seeds and white flowers. It grows quickly and is commonly used for flour and health foods.
![000017](https://github.com/user-attachments/assets/4324d338-1e4d-4e0f-bcf9-129a6790d616)

----------
11 Durum Wheat
Common Name: Durum Wheat
Scientific Name: Triticum durum

Description: Durum wheat is a hard variety of wheat used primarily for pasta production. It has high protein content and grows well in dry climates.
![000275](https://github.com/user-attachments/assets/7ea42989-7bd7-41a7-af42-4f48262e7708)

--------
12 Einkorn
Common Name: Einkorn Wheat
Scientific Name: Triticum monococcum

Description: Einkorn is one of the oldest cultivated wheat species. It produces small grains and is valued for its nutritional content and resistance to poor soil conditions.
![000092](https://github.com/user-attachments/assets/1a1dde00-4d65-453e-ab79-55f1841498b6)

-----------
13 Emmer
Common Name: Emmer Wheat
Scientific Name: Triticum dicoccum

Description: Emmer is an ancient wheat variety, also known as farro. It is hardy and commonly grown in traditional farming systems.
![000279](https://github.com/user-attachments/assets/e8c004a5-8879-4b47-9694-8e6f3add1cb2)

-----------
14 Maize (Corn)
Common Name: Maize / Corn
Scientific Name: Zea mays

Description: Maize is a widely cultivated cereal crop producing large ears of grain. It is used for food, animal feed, and industrial products.
![000288](https://github.com/user-attachments/assets/b3d05965-56f9-4880-b38d-b4ee9fb23d34)

----------
15 Finger Millet
Common Name: Finger Millet
Scientific Name: Eleusine coracana

Description: Finger millet is a drought-resistant cereal crop with small seeds. It is commonly grown in Africa and Asia for its high nutritional value.
![000295](https://github.com/user-attachments/assets/e1137111-c988-49f2-9027-e3174faed63f)

----------
16 Foxtail Millet
Common Name: Foxtail Millet
Scientific Name: Setaria italica

Description: Foxtail millet is a small-seeded cereal known for its adaptability to dry conditions. It is used as food and animal feed.
![000292](https://github.com/user-attachments/assets/b3268e6f-70fd-4c9c-9ad0-6fc8cd886ae7)

---------
17 Pearl Millet
Common Name: Pearl Millet
Scientific Name: Pennisetum glaucum

Description: Pearl millet is a heat-tolerant grain crop widely grown in arid regions. It produces dense grain heads and is a staple food in some areas.
![000286](https://github.com/user-attachments/assets/bf51737e-882e-42e7-9360-f5b0fde7be17)

-----------
18 Proso Millet
Common Name: Proso Millet
Scientific Name: Panicum miliaceum

Description: Proso millet is a fast-maturing cereal crop used for food and birdseed. It grows well in dry environments with minimal water.
![000267](https://github.com/user-attachments/assets/2e6e5092-43d5-4e3a-964a-a0908eac7ee3)

----------
19 Oats
Common Name: Oats
Scientific Name: Avena sativa

Description: Oats are a cereal grain known for their nutritional benefits. They are commonly used for breakfast foods and animal feed.
![000020](https://github.com/user-attachments/assets/59ee2461-6637-429c-a63a-a9322e0a9a2a)

----------
20 Quinoa
Common Name: Quinoa
Scientific Name: Chenopodium quinoa

Description: Quinoa is a pseudocereal grown for its edible seeds. It is rich in protein and adapted to high-altitude environments.
![000064](https://github.com/user-attachments/assets/936a3da0-f9d3-45b8-97cc-47ad14ebd6d3)

--------------
 Model Training

Epochs: 50  
Batch Size: 16  
Learning Rate: 0.0001  

Reason:
Epochs set to 50 to allow sufficient learning cycles without overfitting.  
Batch size set to 16 for stable updates and manageable resource usage.  
Learning rate set to 0.0001 to ensure gradual and stable convergence.

<img width="1523" height="1036" alt="image" src="https://github.com/user-attachments/assets/03ee6ec2-a7a7-4b7d-a3c9-670ef4d560f5" />
--------------------

Model Evaluation
-----
<img width="402" height="796" alt="accuracy-per-class" src="https://github.com/user-attachments/assets/e2d47ca0-7fda-444c-9f7f-480dc5a8349e" />
<img width="403" height="308" alt="accuracy-per-epoch" src="https://github.com/user-attachments/assets/5773ad4b-33fc-4f38-b8c2-099c5f357ece" />
<img width="411" height="748" alt="confusion-matrix" src="https://github.com/user-attachments/assets/cd936ad8-7b42-40b8-94aa-77f333c864e0" />
<img width="404" height="778" alt="confusion-matrix2" src="https://github.com/user-attachments/assets/4ea846cf-e0d7-475f-beec-7d3f661330aa" />
<img width="394" height="309" alt="loss-per-epoch" src="https://github.com/user-attachments/assets/8f96756a-685c-4efa-b432-5474d1792dc2" />

---------------
Model Testing
-------------
test1-test10
------------




<img width="388" height="930" alt="test1" src="https://github.com/user-attachments/assets/23a1f1a8-74f6-436d-8a7c-d0310f6c14f2" />

<img width="302" height="860" alt="test2" src="https://github.com/user-attachments/assets/6ab75e1f-f2fc-4670-9e22-dfb8508699aa" />

<img width="380" height="756" alt="test3" src="https://github.com/user-attachments/assets/3506e544-9d68-4494-aabc-23be315a5f74" />

<img width="246" height="904" alt="test4" src="https://github.com/user-attachments/assets/6bde1f2e-da6d-4e59-9b5f-0bc5aebc37c4" />

<img width="298" height="874" alt="test6" src="https://github.com/user-attachments/assets/ab121ca2-3b04-4b1d-976f-c822b63c9fd0" />

<img width="361" height="839" alt="test7" src="https://github.com/user-attachments/assets/992eef6d-77ea-4ab4-aa1d-4265e240a94f" />

<img width="293" height="858" alt="test8" src="https://github.com/user-attachments/assets/ea723242-bcbc-4168-95ab-92b78b65e8aa" />

<img width="306" height="884" alt="test9" src="https://github.com/user-attachments/assets/168acf24-576b-4091-971d-344f81f7c9ed" />

<img width="297" height="878" alt="test10" src="https://github.com/user-attachments/assets/ba1f04c1-4490-4b2e-90eb-3147dbd70d83" />




























