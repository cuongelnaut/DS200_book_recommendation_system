# DS200_book_recommendation_system
Phong Lai Bao Minh1*, Bui Nguyen Phuong Linh1† and Le
Tuan Cuong1†
1*VNUHCM - University of Information Technology,VietNam.
*Corresponding author(s). E-mail(s): 20522217@gm.uit.edu.vn;
Contributing authors: 20521527@gm.uit.edu.vn;
20520146@gm.uit.edu.vn;
†These authors contributed equally to this work.

Abstract
This study focuses on exploring methods for building a book recom-
mendation system based on large-scale data from Amazon Review Data,
including content-based filtering, collaborative filtering, and keyword-
based recommendation approach. The main objective is to under-
stand the workings of book recommendation systems and propose
improvements and techniques to enhance the performance and qual-
ity of recommendations. The research aims to improve the reading
experience for users and contribute to the advancement of the field
of book recommendation systems in the current era of technology.
Keywords: content-based filtering, collaborative filtering, keyword-based
recommendation approach

1 Introduction
Technology nowadays has a powerful impact on how we access information
and cultural content, including the way we approach reading books. Gradu-
ally, in various ways, technology is replacing or influencing individual reading
preferences. One of the main trends is the explosion of e-books and e-readers.
Readers now have more choices and convenience in accessing books without
the need for traditional printed copies. Additionally, online book platforms and
services like Amazon Kindle, Google Books, and Apple Books have become
increasingly popular, allowing readers to easily purchase and download their
favorite books with just a few clicks or taps on the screen. This way, readers
can own hundreds or even thousands of books in a compact device, saving costs
and space, and providing a more diverse and enjoyable reading experience.
However, amidst the abundance of data available on the internet, find-
ing works that match one’s personal preferences can be quite challenging. To
address this issue, the development of recommendation systems has become
increasingly prevalent in recent years. Recommendation systems help users
discover relevant items, products, or content based on their interests and his-
torical interactions. These systems have revolutionized how readers explore and
interact with books, creating a personalized and engaging reading experience.
Moreover, recommendation systems play a significant role for online retailers,
libraries, and book platforms, enabling them to offer personalized book lists
tailored to each individual’s specific preferences and reading habits.
In this study, our team will explore methods to build a book recommen-
dation system based on large-scale data from Amazon Review Data - a vast
dataset containing user reviews about books and information about various
book titles. The methods include content-based filtering, collaborative filter-
ing, and the development of a keyword-based recommendation approach, where
users can input keywords from their keyboards to receive customized and more
accurate book recommendations. The main objective of this research is to gain
a deeper understanding of data processing and handling in the context of big
data, as well as to comprehend the workings of book recommendation systems.
From this understanding, we aim to propose improvements and techniques
to enhance the performance and quality of the recommendation system. We
hope that this research will contribute to improving the reading experience for
users, allowing them to discover new literary works more efficiently, and fur-
ther advancing the field of book recommendation systems in the current era
of technology.

2 Data
For this project, we utilized the Book Dataset from Amazon Review Data
(2018)Amazon Review Data (2018), which includes various aspects of reviews
such as ratings, text, and helpful votes, as well as product metadata containing
descriptions, category information, prices, brands, and image features. The
book dataset we used consists of two data files: ”reviews” containing 51,311,621
reviews from users and ”metadata” containing information about 2,935,525
products.
The ”reviews” file comprises 12 attributes, with specific focus on attributes
such as ”reviewerID” (ID of the reviewer), ”asin” (ID of the product), ”review-
Text” (text of the review), and ”overall” (rating of the product). As for the
”metadata” file, we are interested in three attributes out of 14: ”asin” (ID
of the product), ”title” (name of the product), and ”categories” - a list of
categories the product belongs to.
To build the book recommendation system based on these two data files, we
conducted extensive data preprocessing using Spark. The main steps included
merging the two data files based on the ”asin” attribute. We also performed
checks for null values, removed unnecessary attributes for the recommendation
task, balanced the data, and carried out several specific data processing steps
to adapt the data to different recommendation methods
