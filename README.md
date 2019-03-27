# Project: Can you unscramble a blurry image? 
![image](figs/example.png)

### [Full Project Description](doc/project3_desc.md)

Term: Spring 2019

+ Team ##2
+ Team members
	+ Andy Huang
	+ Haiqing Xu
	+ Wensong Qiao
	+ Zongbo Cai
	+ HuiChiang Tay

+ Project summary: In this project, we created predictive models for enhance the resolution of images. The goal is to create a high-resolution image that is twice as big as the test image. Basically, for each pixel in the test image, we need to predict 4 corresponding pixels in the high-resolution image. For each point, we select surrouding 8 pixels as our features, vectorize them and fir a predictive model. We used Gradient Boosting Method as the baseline method and proposed three possible improvements: XGBoost, LightGBM and Random Forest. For each model, we used grid search to find the best parameters and used cross validation to prevent overfitting. Our final model is LightGBM because it produces higher PSNR and needs less training time.
	
**Contribution statement**: Andy Huang prepared functions, implemented the basline method and the XGBoost model. Haiqing Xu proposed and implemented the Random Forest model. Zongbo Cai proposed and implemented the LightGBM Model. Wensong Qiao proposed and implemented SRCNN. (Due to time limit, the model is not fully tuned so we did not include it in the final report.) All memebers contributed to the presentation and brainstorming of the project.

Following [suggestions](http://nicercode.github.io/blog/2013-04-05-projects/) by [RICH FITZJOHN](http://nicercode.github.io/about/#Team) (@richfitz). This folder is orgarnized as follows.

```
proj/
├── lib/
├── data/
├── doc/
├── figs/
└── output/
```

Please see each subfolder for a README file.
