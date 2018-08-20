<!-- TITLE: Burwell -->
<!-- SUBTITLE: Things I've worked on here. -->

Wholesale site: Shopify doesn't provide "wholesale" templates. We had to find a standard template that we liked and modify the access to the site. Only botique store owners that sign a contract with us are able to have access to this website with private information.

* Created sub-menu navigation for each brand.
* Created a case pack for-loop.
* Generated "Brand" pages our product lines.
* Made a page for the Marketing Kit that includes cards with download links to our Dropbox account.
* Modified the template "featured collections" section. Changed from 3 to 4 features.
* Added a responsive video section to the homepage using existing code.
* Created "edit product" buttons for all the websites. When the admin is logged in, they can quickly jump to the backend and edit product details.

Brand sites:

* Created "Discover our Brands" top menu bar using SVG graphics.
* Replaced all CT brand logos with SVG logos.


MargotElena.com
* Started the subscription program from a Shopify app.
	* Lots of modifications were needed to get this to functin the way we run our subscription model.
* Improved the Google Page Speed for the site by modifiying the template using Liquid image filters. Went from 30-40 values to 85-95.
* Added social media buttons to the top navigation using FontAwesome.
* Added an auto-populate search feature to the site.
* Created a persistant footer bar about Free Shipping.
* Created "NEW" product badge for this theme. How to activate: tag the SKU with "NEW PRODUCT", then the SVG file will appear in the corner of the image.
* "High Volume" warning on the cart page when we have busy times of the year.
* "Hazmat Restrictions" warning on the cart page when a customer orders an alcohol-based product.


```liquid
{% if page.id == 846168083 %} <!-- /pages/subscribe-to-newsletter -->
	{% include 'newsletter-subscribe' %}
	{{ 'MECC-NLsignup.css' | asset_url | stylesheet_tag }}
{% endif %}
```
