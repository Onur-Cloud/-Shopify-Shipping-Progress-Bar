# Shopify Shipping Progress Bar

# Shopify Shipping Progress Bar

This Shopify snippet provides a dynamic shipping progress bar that enhances the user experience by visually indicating how close a customer is to achieving free shipping. The progress bar fills as the cart total increases, and a package icon at the end of the bar changes color once the free shipping threshold is reached. Additionally, when free shipping is achieved, the original shipping cost is crossed out, and a "0,00 €" in green is displayed next to it.

## Features

- **Dynamic Progress Bar:** The progress bar fills based on the current cart total relative to the free shipping threshold.
- **Package Icon:** A package icon is positioned at the end of the progress bar and changes color when free shipping is reached.
- **Free Shipping Notification:** Once the cart total meets or exceeds the free shipping threshold, a congratulatory message is displayed.
- **Strikethrough Shipping Costs:** The original shipping cost is crossed out and replaced with "0,00 €" in green when free shipping is achieved.
- **Customizable Colors:** Easily customize the progress bar color, icon color, and other UI elements through the snippet code.

## Installation

1. **Navigate to the Theme Code Editor:**
   - In your Shopify Admin, go to `Online Store` > `Themes`.
   - Click on `Actions` > `Edit code` to open the Theme Code Editor.

2. **Find the Correct File:**
   - In the Theme Code Editor, look for the `Snippets` folder.
   - Open the relevant snippet file, typically named `cart-drawer.liquid` or something similar. If you're unsure of the file, you can use `Ctrl + F` (or `Cmd + F` on Mac) to search for the code.

3. **Locate the Correct Position:**
   - Search for `</cart-drawer-items>` in the file using `Ctrl + F`.
   - Insert the provided code snippet directly **below** the `</cart-drawer-items>` line and **above** the `<div class="drawer__footer">` line.

   ```
   </cart-drawer-items>
   <!-- Insert the Shipping Progress Bar code here -->
   <div class="drawer__footer">

## Usage

- **Free Shipping Threshold:** Set the `free_shipping_threshold` variable in the code to define the amount required for free shipping.
- **Shipping Cost:** Set the `shipping_cost` variable to reflect the normal shipping cost before free shipping is applied.
- **Progress Bar Color:** Customize the `progress_bar_color` variable to change the color of the progress bar.
- **Remaining Amount Color:** Customize the `remaining_amount_color` variable to change the color of the remaining amount text.

## Preview

### Before Free Shipping Threshold is Met
![Before Free Shipping](https://i.postimg.cc/9FqXHRGm/image.png)

### After Free Shipping Threshold is Met
![After Free Shipping](https://i.postimg.cc/SRh2Y6LG/image.png)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contributions

Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.
