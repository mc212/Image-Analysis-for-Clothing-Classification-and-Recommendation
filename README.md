# Image-Analysis-for-Clothing-Classification-and-Recommendation

Clothing classification and recommendation have been demonstrated as essential supporting tools and techniques in the fashion e-commerce industry. These applications encourage customers to buy more products and made a huge contribution to the yearly revenue of this industry. Most of the existing efforts have considered classification and recommendation tasks separately. In [1] [2], the clothing item images can be classified into categories and attributes, while many recommendation techniques assume the input data labelled already [3] [4]. Therefore, in this paper, we propose an approach to combine these tasks to build an end-to-end predictive system. The workflow can be seen in Figure 1. Two main stages are building clothing image classification models, outfit compatibility learning and recommendation. Clothing images are annotated automatically with higher-level categories (top/bottom clothing items), lower-level categories (e.g. jean/shirt/tank) and attributes (e.g. floral, cotton, tight) by the models trained in the first stage.
Please note that the terms top clothing items and upper body items are used interchangeably in this paper. Similarly, the terms bottom clothing items and lower body items refer to the same class of clothing items. Then these annotations are used for the outfit compatibility learning and recommendation in the second stage.

Overall, our research aims to address the main research question: Can classification models support compatibility learning in the context of matching clothing items?. Along
with the main question, two sub-questions are as follows:
SubRQ1. Which does the Convolutional Neural Network (CNN)-based model (i.e. VGG16/InceptionV3/Resnet50-based models) bring the best performance in the clothing image classification task? and 
SubRQ2. How does the outfit compatibility depend on the accuracy of the classification models?

The research has been carried out using DeepFashion [5] and Polyvore [6] datasets. While Deepfashion has a diverse fashion images range and rich annotation that’s suitable for training models to classify images into categories and attributes, Polyvore contains a wide range of combinations mostly used for outfit compatibility learning. Our main contribution can be summarized in fourfold:
• Developing a complete pipeline for suggesting bottom clothing images with a given top clothing item.
• Implementing experiments on different CNN approaches (transfer learning with pre-trained models - Resnet50, Inceptionv3, VGG16) on clothing image classification task and identifying the best performing approach.
• Implement Bayesian Personalized Ranking on modelling the compatibility between clothing items.
• Investigating the dependency of the outfit compatibility learning on the accuracy of classification models


In this repository, I uploaded the source code for data preparation and modelling for compatibility learning - which is my main responsibility in the project.


[1] J. P. A. Madulid and P. E. Mayol, “Clothing classification using the convolutional neural network inception model,” in Proceedings of the 2019 2nd International Conference on Information Science and Systems, 2019, pp. 3–7.
[2] T.-R. Tzikas, A.-C. Kyprianidis, M. T. Kotouza, S.-F. Tsarouchis, A. C. Chrysopoulos, and P. A. Mitkas, “Towards fashion image annotation: A clothing category recognition procedure.” in SETN Workshops, 2020, pp. 42–47.
[3] T. Iwata, S. Watanabe, and H. Sawada, “Fashion coordinates recommender system using photographs from fashion magazines,” in TwentySecond International Joint Conference on Artificial Intelligence, 2011.
[4] X. Song, X. Han, Y. Li, J. Chen, X.-S. Xu, and L. Nie, “Gp-bpr: Personalized compatibility modeling for clothing matching,” in Proceedings of the 27th ACM International Conference on Multimedia, 2019, pp. 320– 328.
[5] Z. Liu, P. Luo, S. Qiu, X. Wang, and X. Tang, “Deepfashion: Powering robust clothes recognition and retrieval with rich annotations,” in
Proceedings of the IEEE conference on computer vision and pattern recognition, 2016, pp. 1096–1104. https://mmlab.ie.cuhk.edu.hk/projects/DeepFashion.html
[6] Z. Cui, Z. Li, S. Wu, X.-Y. Zhang, and L. Wang, “Dressing as a whole: Outfit compatibility learning based on node-wise graph neural 
networks,” in The World Wide Web Conference, 2019, pp. 307–317 https://github.com/CRIPAC-DIG/NGNN/tree/master/data

