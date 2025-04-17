# **Email Campaign Optimization**

The marketing team of an e-commerce site has launched an email campaign. This site has the email addresses of all users who created an account in the past.
They have chosen a random sample of users and emailed them. The email informs the user about a new feature implemented on the site. From the marketing team's perspective, success is if the user clicks on the link inside of the email. This link takes the user to the company site.

We are tasked to analyze the success rate of the campaign given by the data, and answer the following:
- What percentage of users opened the email, and what percentage clicked on the link within the email?
- Based on all the information you have about the emails sent, can you build a model to optimize how to send emails in the future to maximize the probability of users clicking on the link inside the email?
- How can you test your proposed model?
- Any different patterns found?

## **User Activity**

![Email_engagement](https://github.com/user-attachments/assets/92fb02b5-9015-42d0-b4be-d30d4f84a4b1)

The total percentage of users who opened the mail is **`10.39%`**

The total percentage of users who clicked the link is **`2.12%`**

The conversion rate from opened emails to clicked links is **`20.38%`**

## **Optimization of Email Campaign**

To optimize our email campaign, let's refine our targeting approach with these strategic elements:

- **Timing optimization** - Analyze user activity patterns to identify peak engagement periods across different days and hours, allowing us to schedule deliveries when recipients are most likely to be active.
- **Geographic targeting** - Leverage location data to map regional engagement patterns and customize delivery schedules according to time zone differences and local behavioral trends.
- **Content refinement** - Evaluate performance metrics across different email types and versions to determine which content elements drive the highest engagement, then adapt our messaging accordingly.

### Timing Optimization
To highlight the most significant engagement opportunities, a threshold value at the 90th percentile (top 10) of all open counts is calculated, and cells exceeding this threshold are marked with red rectangles.
Analyze user activity patterns to identify peak engagement periods across different days and hours, allowing us to schedule deliveries when recipients are most likely to be active.

Below is the heat map of the number of users engaged across different days of the week and hours of the day, who opened the email

![Timing_email_heatmap](https://github.com/user-attachments/assets/25174c43-f7a9-4823-abc7-31a554f153e8)

Below is the heat map of the number of users engaged across different days of the week and hours of the day, who clicked the link

![Timing_link_heatmap](https://github.com/user-attachments/assets/61614f2c-923a-41e6-be96-b3548ff6a35f)

From the above heatmaps, the following are the observations:
- The emails clicked and opened are mostly on weekdays from `Monday` to `Wednesday`
- The majority opened and clicked during the time interval of `9 AM`-`12 PM`.

### Geographic Targeting
Leverage location data to map regional engagement patterns and customize delivery schedules according to time zone differences and local behavioral trends.

![country_bar_chart](https://github.com/user-attachments/assets/a2abc559-dc4c-44dd-8306-9e14621ea907)

The majority of the users who opened the email and clicked the link are from the `US`, followed by the `UK`, `France`, and `Spain`.


### Content Refinement

Different email types and versions are being sent to the users. The different types and versions are as follows:
- Personalized
- Genric
- Long_text
- Short_text

Let us evaluate the performance metrics across different email types and versions to determine which content elements drive the highest engagement, then adapt our messaging accordingly.

The heatmaps depict the different segments across email opened and link-clicked across email types and versions

![email_type_opened](https://github.com/user-attachments/assets/def89181-e6c1-451c-8eea-83a9f45a0d89)

![email_type_clicked](https://github.com/user-attachments/assets/73b56e5a-f8af-43e1-a3dc-8d7bfc319894)

The conversion rate between different segments is depicted below:

![email_type_conversion](https://github.com/user-attachments/assets/74395577-58d5-42f7-ac97-61102951f598)

It is evident that the emails that are `personalized` and `short`, have higher rates of conversion.

# **Observations**

- It is evident that during the Weekdays, i.e., `Monday`, `Tuesday`, and `Wednesday`, in the time interval of `0900`-`1200` hrs, the users are actively viewing the emails and clicking the link.
- Geogrpahically, the citizens of the `US` are the majority of the population are opening the email and clicking the link.
- When the email type and email version is being into consideration, users who are sent a `personalized` and `short` email  are more likely to open the email and click on the link. The conversion rate for this is about `21.6%`.

# **Conclusions**

From the observations dereived from the dataset, it is evident that:

To perform the campaign successfully, it is advised that the emails are to be sent to the users:
- who are from the US
- in the weekdays from Monday to Wednesday
- in the time interval of 0900-1200 hrs
- emails must be personalized and short

