# Motivation:
Generative AI is currently being applied to creative fields, but AI art faces numerous ethical controversies. As a fan who has envolved in Chinese fandom for a long time, I obeserved debates about AI fan arts, and concerns about the future of human creativity in respect of originality protection, human automy and fan idenitity under this impact of generative AI technology. Through this project, I hope to understand the most common characteristics of AI fan art and its popularity, and to envision its potential position and development within the fandom in the future.

# Data Source:
This dataset is a collection of data from the tag "ai绘画(ai drawings)" in Chinese fan platform Lofter. It is collected works data from the rankings from March 2024 - April 2024. By analyzing this dataset, I hope to explore the relationship between the number of likes, recommendations, and comments received by AI fan art and independent variables such as style, illustration scale, affiliated fandom, and original work type of the fandom.

# Data Processing: 
The data was collected by hand from the platform Lofter. For fandom and characters, I read from the tags of the posts and translated those fandom and characters' names in English. For style and scale, I have compiled tags based on the consensus of Chinese fans and the stylistic classifications in digital painting, and I use these tags as predictors. For example, the style that frequently appears in Japanese games and animation is classified as "ACGN" style, while the style that lacks accurate outlines and relies on color to create the sense of volume of characters is classified as "Impasto" style.

# Visualization:

## The Most Popular Style
<img width="875" height="540" alt="image" src="https://github.com/user-attachments/assets/83663f94-7512-4647-8f70-72ff94609015" />
The first bar plot is a visualization counting different styles. In the original dataset, style is a predictor defining the artistic style the AI fan art imnitating. From the visualization, we can see that ACGN style is the most popular among all the collected data, and the 3D Model, Water Color and Original Work Imnitating are the least welcomed. Impasto is the second popular one, and realistic is the third popular one. The ACGN style is closely related to ACGN culture, and this culture is very dominate in fandoms, and ACGN fandoms are the most flourished fandom in China; therefore, the popularity of ACGN style is propobably related to the popularity of ACGN culture in Chinese fandom.

## The Most Popular Fandom
<img width="875" height="540" alt="image" src="https://github.com/user-attachments/assets/a1cc800c-419b-425a-b293-b8d46bdebf16" />

## The Most Popular Illustration Scale
<img width="875" height="540" alt="image" src="https://github.com/user-attachments/assets/a566c732-ae47-4b9e-8be9-00565ec8c979" />

## The Most Popular Orignal Work Type
<img width="875" height="540" alt="image" src="https://github.com/user-attachments/assets/e682714e-5152-4acd-9dcc-879be7fa7716" />
Same as the first bar visualization, I visualized the number of works based on fandom, illustration scale and orginal work type (genre) in these three plots. Although there are various fandoms, Genshin (Chinese game) is most popular among all of the fandoms in the dataset. This could propably a result of the fandom itself's popularity, and also because it is a very new work.
The most popular illustration scale is bust, this is probably because of it could show more details of the character. On contrast, the large illustration with landscape is less popular.
The third plot visualized the popularity based on the original work type. The most popular type is game, and the second popular one is anime.
In later analysis, I will analyze in each original work type, which kind of style is the most welcomed.

## Relationship Between Scale and Likes
<img width="875" height="540" alt="image" src="https://github.com/user-attachments/assets/32d3a6a6-4891-495a-b943-106d4aa5af15" />
This bar plot shows the relationship between Scale and Likes. Here, the “Scale” indicates in what size of character body the illustration draws. I firstly calculated the means of likes among each scale, and then drew a plot to demonstrate the relationship. We can see that the Portrait scale is the most welcomed, and the Bust is the second. Comparing to larger scale, portrait and bust scale can more directly display facial features, and although it contains less information, it is very eye-catching. Small-scale illustrations also avoid errors that AI may make during the generation process. In addition, because AI art has lower information density and lacks emotional expression compared to human art, those who choose to support AI art may be more concerned with the direct visual impact than with the information in the illustration.

## Likes vs Recommendations Linear Regression
<img width="865" height="534" alt="image" src="https://github.com/user-attachments/assets/f873a7cc-ac8a-441c-a38a-fb1f203d9cdc" />
This visualization shows a linear regression relationship between the number of likes and recommendations. The visualization reveals a strong positive correlation between likes and recommendations, with Impasto-style viewers being most likely to provide a recommendation after a like. An extreme value in the upper right corner of the visualization influences the regression performance of ACGN style. Most works have low numbers of likes and recommendations, indicating that only a small number of works achieve high popularity.

## Popularity of Styles in Each Original Work Type

<img width="875" height="540" alt="image" src="https://github.com/user-attachments/assets/560c4d4a-f277-457d-8ebb-ce2a1296e184" />
This visualization is a heatmap showing the popularity of styles in different original work types. However, since there is an extreme value in the style "Original Work Imnitating" (there is only one work for this style) and it has a extreme high like, I redraw a heatmap after remove this style.
<img width="875" height="540" alt="image" src="https://github.com/user-attachments/assets/7daa7b29-be2e-404b-a47c-4968179cdc9d" />
This visualization shows that the "Game" genre has the most diverse styles. Analyzing from the perspective original work types of fan art which each has more than one style, I found that the most popular style in both Anime and Game genere is impasto, while the most popular style in Novel genres is realistic.
