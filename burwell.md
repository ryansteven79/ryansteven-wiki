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

```html
<div class= MECC-NLsignup>
<div id="wrapper" class="divided">
		<section class="banner style1 orient-left content-align-left image-position-right fullscreen onload-image-fade-in onload-content-fade-right">
			<div class="content">
				<h3><strong>WELCOME TO MARGOT ELENA</strong></h3>
				<p class="major">The official site of Lollia, TokyoMilk, Library of Flowers, The Cottage Greenhouse, and Love & Toast.</p>

				<h3><strong>KEEP IN TOUCH</strong></h3>
				<p class="major">Subscribe to our Tribe for exclusive offers, special events and behind the scenes action! Sign up today to receive an exclusive offer,&nbsp;just&nbsp;for&nbsp;you.</p>


				<!-- Begin MailChimp Signup Form -->
				<style type="text/css">
					#mc_embed_signup {
						background: #fff;
						clear: left;
						font: 14px "Source Sans Pro", Helvetica, sans-serif;
						text-transform: uppercase;
						letter-spacing: .125rem;
					}

					#mc_embed_signup form {
						padding: 0;
					}

					/* Add your own MailChimp form style overrides in your site stylesheet or in this style block.
	   We recommend moving this block and the preceding CSS link to the HEAD of your HTML file. */
				</style>
				<div id="mc_embed_signup">
					<form action="https://margotelena.us13.list-manage.com/subscribe/post?u=36fcadbfa4d3283ccc7150a9b&amp;id=9f958942c4" method="post" id="mc-embedded-subscribe-form" name="mc-embedded-subscribe-form" class="validate" target="_blank" novalidate>
						<div id="mc_embed_signup_scroll">
							<div class="mc-field-group">
								<label for="mce-EMAIL">Email Address</label>
								<input type="email" value="" name="EMAIL" class="required email" id="mce-EMAIL">
							</div>
							<div id="mce-responses" class="clear">
								<div class="response" id="mce-error-response" style="display:none"></div>
								<div class="response" id="mce-success-response" style="display:none"></div>
							</div>
							<!-- real people should not fill this in and expect good things - do not remove this or risk form bot signups-->
							<div style="position: absolute; left: -5000px;" aria-hidden="true"><input type="text" name="b_36fcadbfa4d3283ccc7150a9b_15ac58c4ee" tabindex="-1" value=""></div>
							<div class="clear"><input type="submit" value="Subscribe" name="subscribe" id="mc-embedded-subscribe" class="button"></div>
						</div>
					</form>

				</div>
				<script type='text/javascript' src='//s3.amazonaws.com/downloads.mailchimp.com/js/mc-validate.js'></script>
				<script type='text/javascript'>
					(function($) {
						window.fnames = new Array();
						window.ftypes = new Array();
						fnames[0] = 'EMAIL';
						ftypes[0] = 'email';
						fnames[1] = 'FNAME';
						ftypes[1] = 'text';
						fnames[2] = 'LNAME';
						ftypes[2] = 'text';
					}(jQuery));
					var $mcj = jQuery.noConflict(true);
				</script>
				<!--End mc_embed_signup-->
			</div>

			<div class="image">
				<img src="{{ 'Margot_1_of_1.jpg' | asset_img_url: '250x', scale: 3,crop: ‘center’, format: 'pjpg' }}" />              
			</div>


		</section>

	</div>
</div>
```
