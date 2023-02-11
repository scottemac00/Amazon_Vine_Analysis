# Overview: #
        The purpose of this analysis was to assess bias in Amazon reviews; whether the 'Vine' reviews written by paid members 
        of the program are more favorable than those submitted by non-paid individuals. I used Google Colaboraty Notebooks, 
        Apache Spark (PySpark), Amazon Web Services, and pgAdmin to extract the data from an Amazon US Reviews database.
        
        I selected a dataset that included musical instruments and associated items. Upon extraction, I cleaned and transformed 
        the data using PySpark, then loaded the data into pgAdmin for further analysis.

# Results: #
        There is a bulleted list that addresses the three questions for unpaid and paid program reviews
        
    * How many Vine reviews and non-Vine reviews were there?
        * Vine reviews: 59
        * non-Vine reviews: 13480    
    * How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
        * 5-star Vine reviews: 34
        * 5-star non-Vine reviews: 7678
    * What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
        * 5-star Vine reviews: 57.63%
        * 5-star non-Vine reviews: 56.96%


# Summary: #
        The data above shows that Vine reviews were significantly **LESS** than non-Vine reviews. Proportionally, though, of the 
        paid reviews, more than **HALF** were 5-Star. What this tells decision makers is that, according to this sample set, 
        paid reviewers give 5-star ratings about the same amount as non-paid reviewers. This could mean that those purchasing musical 
        instruments and music products tend to be more accepting of what they buy, or more inclined to write a positive review due to 
        <insert factor/reasons here>.
             
        This rather small sample set would best be compared against more of the 50 Amazon US Review datasets available. Applying a 
        regression might better illuminate any bias in reviews and also might bring other correlations to light. Perhaps certain types 
        of items (datasets) are more similar than others, and thus might better represent conclusions on the broader population.
        
        Another aspect of the data worthy of further analaysis is the *'verified_purchase'* column:
        !(Resources/Images/verified_purchase.png)
        If a review is high, regardless of paid or non-paid status, does this call the review's integrity into question? 
        This information might inform updates to review accepted practices and policies, and ultimately the Vine program itself.

