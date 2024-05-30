# Free Shipping Bar V1

This snippet provides a dynamic Free Shipping Bar component for Shopify storefronts. It informs customers of their progress towards qualifying for free shipping, enhancing their shopping experience and potentially increasing the average order value. This guide details the component's features, ideal use cases, and step-by-step implementation instructions.

**Live Preview Link**: [Free Shipping Bar Preview](https://dark-development-store.myshopify.com/?preview_theme_id=136011317410)

## Features

- **Feature 1**:
  - Option to add a Free Shipping Heading.
  - Option to add a Free Shipping Threshold.
  - Option to add a Free Shipping Success Message.
  - Option to add a Free Shipping Progress Message.

- **Feature 2**:
  - Option to change the Background Color.
  - Option to change the Progress Bar Color.

## Implementation Steps

### Step 1: 
	Navigate to the `cart-drawer.liquid` or `cart.liquid` file in the `sections` folder of your Shopify theme.

### Step 2: 
	Render the `free-shipping-bar-v1.liquid` snippet in the `cart-drawer.liquid` or `cart.liquid` file:
	
	{% render 'free-shipping-bar-v1' %}

### Step 3: 
	Add the Free Shipping Heading, Free Shipping Threshold, Free Shipping Success Message, and Free Shipping Progress Message:
	
	{% render "free-shipping-bar-v1" , 
 		cart: cart,free_shipping_heading: settings.free_shipping_heading, 
   		free_shipping_success_message: settings.free_shipping_success_message , 
     		free_shipping_messsage: settings.free_shipping_messsage , 
       		free_shipping_threshold: settings.free_shipping_threshold 
	 %}
### step 4:
     Navigate to the `free-shipping-bar-v1.css` file in the `Assets` folder of your Shopify theme.

### step 5: 
    Add the `free-shipping-bar-v1.css` file in `cart-drawer.liquid` or `cart.liquid` 

### step 6:
    To change the settings Navigate to `Global cart Theme setting` under cart section will have option to change Free shipping settings


## Important Notes

> - The component employs its own styling for the grid system. For further optimization, consider using the classes provided by the theme.

By following these steps, you can effectively integrate the Free Shipping Bar into your Shopify storefront, providing customers with real-time feedback on how close they are to qualifying for free shipping. This can enhance the shopping experience and potentially increase the average order value.
