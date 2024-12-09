Preview Link: https://mira-dev-test.myshopify.com

Password: cheeld

Sample Product URL: https://mira-dev-test.myshopify.com/products/red-t-shirt

# Steps for displaying different Colored Products as variants of a Single Product

## 1. Creating the Collection
Go to the Collections Tab in the Shopify Admin under Products

![image](https://github.com/user-attachments/assets/de8bc1f7-17a6-441c-b229-467056c2bb5b)

Next step is to create a collection, click on the Create collection button

![image](https://github.com/user-attachments/assets/29118a96-91a2-4b91-a610-c02b5d055149)

Give a suitable title to your collection, I have called it Plain T-Shirts

![image](https://github.com/user-attachments/assets/7c6fa7cf-9594-4fe8-9ed0-7e71ba5ba405)

Great job! Let's add the products next, select the Smart radio option and then we'll add the conditions to add the products that will appear as variants on the frontend

![image](https://github.com/user-attachments/assets/8023edaf-e9b0-4f1b-b310-5cd73d7773ba)

For the condition, I have matched the Product Title of the T-Shirts but you can even use product tags or any other suitable condition that Shopify offers. You can also add
more than one condition.

![image](https://github.com/user-attachments/assets/5fe3621f-49b7-4d81-b058-c3f718d7547a)

We're almost there! Scroll to the bottom of the collection creation page and once you click on the pencil icon next to Search engine listing, it will reveal additional information
we can change. 

![image](https://github.com/user-attachments/assets/9b9c4b57-770f-403a-8472-c1059acca54f)

Under the URL Handle field, copy the collection handle, it is the text after the 'collection/'. We will use this in the last step

![image](https://github.com/user-attachments/assets/870d6ee7-f4a3-45bb-b057-9e85a1ea3813)

## 2. Creating the Product
Got to the Products tab and click on Add product

![image](https://github.com/user-attachments/assets/7cf327ca-bcf1-4ec1-b793-fdd793c43abf)

Add the product title and fill in the necessary details, then scroll down until you see the Add Variants button, click on it

![image](https://github.com/user-attachments/assets/914c52ad-83fe-4117-a1b4-a5ab609ed1cc)

Click on the Color option, and then select a size

![image](https://github.com/user-attachments/assets/0c4c0c0e-413d-482a-96d4-5b61b64c5bec)![image](https://github.com/user-attachments/assets/ffdef7f2-8201-472b-801f-19e52cd34919)

Then click on the Add another option and follow the same steps for adding Size variants. Once you're done with adding the inventories to your variants, scroll down to the 
metfields section and click on the field next to **Product Collection Handle**

![image](https://github.com/user-attachments/assets/470bf37e-5851-43ef-a0ca-1245ce824324)

Inside this, paste the Collection Handle we copied in the last step of the Collection Creation Step.
![image](https://github.com/user-attachments/assets/b629bc81-82f2-4e37-bb2c-b003024e04f4)

That's it, Well done! You can now preview the product on the fron end by clicking this button at the top 

![image](https://github.com/user-attachments/assets/9a7f2e5a-5255-40cf-bb70-2f47375a86dd)


## Page Speed Insights Report: 
https://pagespeed.web.dev/analysis/https-mira-dev-test-myshopify-com-products-black-t-shirt/g61qwo23ku?use_original_url=true&form_factor=desktop

As you can see, both SEO and Accessibility have a 100 and 97 score respectively for mobile and desktop. But that is more of a Dawn thing, I didn't do much to improve the score but this also shows how my code doesn't negatively affect
SEO, accessibility and site performance.

I have done ADA projects for Voluspa.com so I am familiar with Accessibility as well.


> [!IMPORTANT]
> I have created 2 PRs for both my approaches, one utilizes Dawn's native HTMLUpdateUtility object that updates the entire main section based on the Product URL. I have stored the Product URL for
> each color swatch inside its input. The next approach that I have coded myself is based on prefetching URLs and the sections using the section rendering API to make the transition and > switching between variants seamless. Aftler replacing the old section with the new one, I update the URLs and make sure out of stock sizes aren't selected.
> The branch called Prefetching-Variants-Approach utilizes my custom approach and the branch called Dawn-HTMLUpdateUtility-Approach utilizes Dawn's native HTMLUpdateUtility object.

Hope you like the code and functionality.

Best,

Muhammad Malik
