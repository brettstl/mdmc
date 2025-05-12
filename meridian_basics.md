**Site**  
[https://developers.google.com/meridian](https://developers.google.com/meridian)  
[https://developers.google.com/meridian/docs/user-guide/collect-data](https://developers.google.com/meridian/docs/user-guide/collect-data)

**What is MMM**  
A Mixed Media Model\* estimates how each of your marketing channels, combined with market factors, affect our revenue.

(aka media mix modeling, aka MMM, aka Marketing mix modeling)

**Appeal to authority**   
“MMM is the most  promising measurement type for identifying drivers of business value,  
...61% of US marketers are aiming to improve their MMM in the future.”   
\- [emarketer.com](http://emarketer.com/)

**Meridian according to Google**  
Marketing mix modeling (MMM) is a statistical analysis technique that measures the impact of marketing campaigns and activities to guide budget planning decisions and improve overall media effectiveness. MMM uses aggregated data to measure impact across marketing channels and account for non-marketing factors that impact revenue and other key performance indicators (KPIs). MMM is privacy-safe and does not use any cookie or user-level information.  
Meridian is an MMM framework that enables advertisers to set up and run their own in-house models. Meridian helps you answer key questions such as:

* How did the marketing channels drive my revenue or other KPI?  
* What was my marketing return on investment (ROI[1](https://developers.google.com/meridian/docs/basics/about-the-project#fn1))?  
* How do I optimize my marketing budget allocation for the future?

**Pros and Cons of a MMM**  
Advantages

* Privacy-compliant measurements  
* Improve media ROI  
* Guide budget planning

Areas of concern

* Requires a lot of data  
* Less effective with big market changes  
* Very difficult to build…

**Features of Meridian**  
was released Free and open-source this year (2025). 

Meridian provides…

* Google Search Volumes as a control  
* Media saturation and Adstock decay models  
* Evaluation of the model’s quality  
* Media budget optimization recommendations  
* Estimation using what-if scenarios

**Things to do in order.**  
Sign up for the “Stay Connected” emails

Sign up for Google Search Query Volume (GQV)  
[https://developers.google.com/meridian/docs/basics/using-mmm-data-platform](https://developers.google.com/meridian/docs/basics/using-mmm-data-platform)

Use the free Colab demo to get the basics. 

Prepare your own data

Run in Colab, Vertex, or another type of notebook. 

Last, get involved with the community [https://developers.google.com/meridian/support](https://developers.google.com/meridian/support)

Notebooks are documents that can contain a mix of live code, equations, narrative text, visualizations, and other rich media (like images, videos, and interactive plots). It's not just a static document; the code within it can be executed, and the results (output, plots, etc.) are displayed directly within the notebook.

Generally, you can back these up in tools like Github, or even Google Drive so you can reference them later, or even work in the same one with another person. 

**About Colab**  
This is a free python environment that leverages Google’s cloud computers. It has a lot of libraries already installed, so it is pretty easy to setup (but there are always hiccups\!)  
The biggest issue is that Meridian takes a lot of computing resources, and Colab can time out if you push it too hard. 

**About Colab pro**  
The next step up for you might be Colab pro, and I like it. First, you can do all of the same things you can do in the free version (save to Drive, work with other people, use the exact same code\!)

But, it can do a lot more. It gives you access to a lot more computing power, you can use terminal access to install and control things better. It is part of GPC, so you have better control of who in your organization can access notebooks. 

It does cost money, but there are low cost options to try it out including a pay-as-go option of a one time $9.99 option.

The biggest disadvantage is that unless you go with an Entreprise plan, you can’t schedule your notebooks. To get around that, you would need to use something like Google Cloud Composer to kick off your python code as needed.

   
**FAQs**  
Is this Free to use: 100% free\!  
Is your data safe: yes, Google can’t access your data

**How Meridian works**

**How Meridian Works (Simplified):**

1. **Looks at Historical Data:** Meridian analyzes your past marketing spending across different channels alongside your business results (like sales, website visits, or leads) over time. It also considers other factors that might influence your results, such as seasonality (like more sales during holidays) or significant events (like a product launch).

2. **Identifies Patterns:** Using statistical techniques, Meridian tries to find patterns and relationships in this data. For example, it might identify that increases in spending on a specific type of online ad tend to correlate with increases in sales a little while later.

3. **Quantifies Impact:** The key output of Meridian is understanding *how much* each marketing channel contributes to your desired business outcome. It estimates things like:    
   * **Return on Investment (ROI):** For every dollar you spend on a particular marketing channel, how many dollars in revenue (or other valuable outcomes) do you get back? For instance, Meridian might tell you that for every $1 spent on search engine ads, you generate $3 in revenue.  
   * **Channel Effectiveness:** Which marketing channels are the most effective at driving results, and which might be underperforming?

**Meridian is based on Bayesian Inference**

Imagine you're trying to guess if it will rain tomorrow.

Prior Belief (the "Prior"): Before looking at any weather data, you might have a general idea based on the time of year or the typical climate in your area. This is your "prior belief" or just "prior." For example, you might think there's a 30% chance of rain.

Evidence (the "Likelihood"): Now you check the weather forecast and see dark clouds. This new information is the "likelihood" – how likely is it to see dark clouds if it's actually going to rain?

Updated Belief (the "Posterior"): Bayesian inference is the process of combining your prior belief with the new evidence to arrive at a more informed belief, called the "posterior belief" or "posterior." Seeing dark clouds likely increases your belief that it will rain tomorrow, maybe now you think there's an 80% chance.

The Key Idea: Bayesian methods don't give you a definitive "yes" or "no." Instead, they provide a probability – a degree of certainty – that something is true, and this probability gets updated as more data becomes available.

**Bayesian For Meridian.**  
Prior knowledge can be based on your internal and external research. For example, you know that Paid Search is more effective dollar-for-dollar than banner advertising, so you bake that into your priors. You may not know exactly how much, but you think Paid Search might have an ROI of 2 vs 0.9 for banner ads. 

Bayesian methods naturally quantify uncertainty by providing a range of possible ROI values along with their probabilities. Instead of saying "SEM ROI is $3," Meridian might say, "There's a 90% probability that the ROI for SEM is between $2.50 and $3.50." This gives you a much better understanding of the potential variability.

Bayesian is always willing to adjust to new data. The initial prior beliefs are either strengthened or adjusted based on new evidence, leading to more accurate and reliable insights over time. More data over time is almost always better, but strong priors can help you when you don’t have  a lot of data (like for a product you just launched this year\!)

At the end of the day, Bayesian methods can help distinguish between channels that are consistently high performers and those whose apparent success might be due to random fluctuations in the data.

