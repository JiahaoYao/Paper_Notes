# Linear Discriminant Generative Adversarial Networks

It is probably the combination of GAN and LDA. The paper proposes a kind of unsupervised learning and class conditional GAN. DIscriminator of LD-GAN is trying to maximize the linear separabillity of generated image and targeted image, while generator is updated by the decision hyperplane by LDA. It compromise the learning rate between G and D. The LDA learn a linear projection matrix, whose objective is to maximize between-class distance and minimize within-class distance. 

### Structure 

discriminator is end-to-end combination of LDA with a extractor.

Maybe the best way to understand is just to implement such a fantastic idea.

Dynamic balance is to balance update frequency between G and D.

Nice idea, can not wait to implement it but I will give a talk first.