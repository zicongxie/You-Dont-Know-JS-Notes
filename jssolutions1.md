***Still Incomplete***

```/* Write a program to calculate the total price of your phone purchase. You will keep purchasing phones (hint: loop!) until you run out of money in your bank account. You'll also buy accessories for each phone as long as your purchase amount is below your mental spending threshold.
After you've calculated your purchase amount, add in the tax, then print out the calculated purchase amount, properly formatted.
Finally, check the amount against your bank account balance to see if you can afford it or not.
You should set up some constants for the "tax rate," "phone price," "accessory price," and "spending threshold," as well as a variable for your "bank account balance.""
You should define functions for calculating the tax and for formatting the price with a "$" and rounding to two decimal places.
Bonus Challenge: Try to incorporate input into this program, perhaps with the prompt(..) covered in "Input" earlier. You may prompt the user for their bank account balance, for example. Have fun and be creative! */

const tax = 0.09;
const phonePrice = 80.00;
const accessory = 10.00;
const budget = 500.00;
var balance = 900.89;

function calculateTax(taxRate, phone) {
  return phone * taxRate;
}

function getPhone(amt, acc, priceWithTax) {
  return acc - (amt + priceWithTax);
}

function getAccessory(cover) { 
  getPhone() + cover;
}

function formatPrice(receipt) {
  return `${getPhone()}`;
}

const getTax = calculateTax(tax, phonePrice);
const phoneSale = getPhone(budget, getTax, phonePrice);
const addition = getAccessory(accessory);
const printPriceForPhone = formatPrice(phoneSale);
const printPriceWithAccessory = formatPrice(addition);


/* while (phonePurchase === 'Yes' && accesoryPurchase === 'Yes') {
  console.log(`Your total is ${printPriceWithAccessory}.`);
  if (balance === budget) {
    break;
    console.log(Prompt('My budget is below the mark. Should I buy more phones'?));
  };
  
};

if (phonePurchase === 'Yes') {
  while (budget > phonePrice) {
  console.log(`Your total is ${printPriceWithAccessory}.`);
  }
  console.log('My budget is below the mark. I should not buy anymore phones.');
} */```
