# Related-Blog-Posts

RelatedBlog Posts on Product Page

The "Related Blog Posts" section is designed to enhance product pages by displaying relevant blog articles. It leverages Shopify's Liquid templating language to fetch and display related blog posts based on metafield values associated with the products. If no related metafields are present, the section defaults to displaying globally defined blog posts.

Step 1: Define the Metafield
Go to Settings in your Shopify admin.
Navigate to Metafields and select "Products."
Click on "Add definition" to create a new metafield for products.
Set the Namespace and Key to custom.related_post_handles
Choose the Content Type. For this purpose, "Single line text" type “List” is appropriate, as you'll be storing multiple blog post handles.
Give it a name and description that makes it easy to recognize, like "Related Blog Post Handles."
Save the metafield definition.

Step 2: Populate the Metafield for a Product
Go to the Products section of your Shopify admin and select a product you want to edit.
Scroll down to the Metafields section and find the "Related Blog Post Handles" metafield you created.
Enter the blog post handles you wish to relate to this product. A handle is the last part of the URL for a blog post. For example, if the blog post URL is https://yourstore.com/blogs/news/awesome-post, the handle is ‘awesome-post’.
Save the product to store these metafield values.

Step 3: Create menu ‘blogs’ in Navigation, where add links to all blogs in shop.

Step 4: Creating the Section
Access Your Theme Files: Go to your Shopify Admin, click on "Online Store," then "Themes." Find the theme you want to edit, and click "Actions" > "Edit code."

Create a New Section: In the Sections folder, click "Add a new section." Name it RelatedBlogPosts.liquid or similar, ensuring it reflects the purpose of the section.

Copy code and paste code from RelatedBlogPosts.liquid that is on https://github.com/HelgJet/Related-Blog-Posts

Step 5: Configuring the Section Settings
After creating the section with the appropriate Liquid and schema, you can configure its settings to control how it appears on the product page.

Navigate to Customize Theme: From the Shopify Admin, go to "Online Store" > "Themes." Find the theme you're working on, click "Customize."

Select a Product Page to Edit: In the theme editor, navigate to a product page from the page selector dropdown to bring up sections that can be added or configured on product pages.

Add the Related Blog Posts Section: Click "Add section" and look for your newly created "Related Blog Posts" section. Add it to your page.

Configure the Section: Use the settings defined in your schema to customize the section. This can include:

Page Width: Adjust the maximum page width for the related posts section.
Use Section Width: Decide whether the section should span the full width of the page or be constrained.
Title: Set a title for the section, such as "Related Posts."
Choose Default Blog: Select a blog from which posts will be pulled, if a product has no metafields filled out.
Posts Limit: Choose how many posts to display at maximum.
Padding: Adjust the top and bottom padding for the section to fit the overall design of your product pages.
Preview and Save: As you adjust these settings, preview the changes in real-time in the theme editor. Once satisfied, make sure to save your changes.
