# Predict-Subscriptions-of-a-music-listening-website
Predict a music-listening social networking website, follows the “freemium”
business model. The website offers basic services for free, and provides a number of additional premium capabilities
for a monthly subscription fee. This project is focused on predicting which people would be likely to convert from free
users to premium subscribers in the next 6-month period, if they are targeted by promotional campaign. The dataset contains data from the previous marketing campaign which targeted a number of non-subscribers.

The general overall task is to build the best predictive model for the next marketing campaign, i.e., for
predicting likely adopters (that is, which current non-subscribers are likely to respond to the marketing campaign
and sign up for the premium service within 6 months after the campaign). 

Data Description:
 The training dataset contains approx. 86,700 records, each record representing a different user of the
XYZ website who was targeted in the previous marketing campaign. Each record is described with 25 attributes.
Here is a brief description of the attributes (attribute name/type/explanation):
1. adopter / binominal (0 or 1) / whether a user became a subscriber within the 6-month period after the marketing campaign (this is an outcome variable!)
2. user_id / integer / unique user id
3. age / integer / age in years
4. male / integer (0 or 1) / 1 – male, 0 – female
5. friend_cnt / integer / numbers of friends that the current user has
6. avg_friend_age / real / average age of friends (in years)
7. avg_friend_male / real (between 0 and 1) / percentage of males among friends
8. friend_country_cnt / integer / number of different countries among friends of the current user
9. subscriber_friend_cnt / integer / number of friends who are subscribers of the premium service
10. songsListened / integer / total number of tracks this user listened (or reported as listened)
11. lovedTracks / integer / total number of different songs that the user “liked”
12. posts / integer / number of forum or discussion board posts made by the user
13. playlists / integer / number of playlists created by the user
14. shouts / integer / number of wall posts received by the user
15. good_country / integer (0 or 1) / country type of the user: 0 – countries where free usage is more limited, 1 –less limited.
16. tenure / integer / number of months since the user has registered on the website.
17. There are also a number of attributes with the following names: delta_<attr-name>, where <attr-name> is one of the attributes mentioned in the above list. Such attributes refer not to the overall number, but the change to the corresponding number over the 3- month period before the marketing campaign. For example, consider attribute delta_friend_cnt. If, for some user, friend_cnt = 50, and delta_friend_cnt = –5, it means that the user had 50 friends at the time of the previous marketing campaign, but this number reduced by 5
during the 3 months before the campaign (i.e., user had 55 friends 3 months ago).
