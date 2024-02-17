name = "Lovely Loveseats for Neat Suites on Fleet Street"

address = "3201 Greenway Rd." 
address_part_2 = "Salem, MA 01970"
phone_number = "(978) 822-7543"

lovely_loveseat_description = "Lovely Loveseat. Tufted polyester blend on wood. 32 inches high x 40 inches wide x 30 inches deep. Red or white. $254.00"

lovely_loveseat_price = 254.00 

stylish_settee_description = "Stylish Settee. Faux leather on birch. 29.50 inches high x 54.75 inches wide x 28 inches deep. Black. $180.50"

stylish_settee_price = 180.50 

luxurious_lamp_description = "Luxurious Lamp. Glass and iron. 36 inches tall. Brown with cream shade. $52.15"

luxurious_lamp_price = 52.15 

sales_tax = .088

customer_one_total = 0

customer_one_total += lovely_loveseat_price

customer_one_itemization = ""

customer_one_itemization += lovely_loveseat_description

customer_one_total += luxurious_lamp_price

customer_one_itemization += "\n"

customer_one_itemization += "\n"

customer_one_itemization += ""

customer_one_itemization += luxurious_lamp_description

customer_one_tax = customer_one_total * sales_tax 

customer_one_total += customer_one_tax

print(name)
print(address)
print(address_part_2)
print(phone_number) 
print("\n")
print("Customer One Items:\n")
print(customer_one_itemization)

print("\n" + "Subtotal: $" + str(lovely_loveseat_price + luxurious_lamp_price))
print("Sales Tax: ${:,.2f}".format (customer_one_tax))

print("\nCustomer One Total: ${:,.2f}".format(customer_one_total))
print("\n02/16/2024")
print("--------------------------------------")
print("Refund policy: We offer a 30-day refund window for your purchase. If you're not satisfied, return the product within 30 days of purchase to request a refund with original receipt!")
