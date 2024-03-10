# XML_Assignment_2
In the orders.xsd created a schema that will validate the data entered into orders.xml


# The schema defined in the .xsd file specifies the structure and rules for valid XML documents.

# Root Element:
- The root element is <customers>, which represents a collection of
customer information.
- It contains multiple <customer> elements.

# Customer Element (<customer>):
- Each <customer> element represents an individual customer.
- It has the following child elements:
- <custID>: The ID number of the customer (formatted as cust where # is a digit).
- <name>: The name of the customer.
- <address>: The address for the customer.
- <phone>: The phone number for the customer.
- <orders>: A collection of information on individual orders.

# Order Element (<order>):
- Nested within each <customer> element, there can be multiple <order> elements.
- Each <order> element represents an order placed by the customer.
- It has the following attributes:
- orderID: An ID number for the order (formatted as ord### where is a digit).
- orderBy: The ID number of the customer who placed the order.
- Order Details (<orderDate> and <items>):
- <orderDate>: Represents the date when the order was placed.
- <items>: A collection of information on individual items within the order.

# Item Element (<item>):
- Nested within each <order> element, there can be multiple <item> elements.
- Each <item> element represents a specific item in the order.
- It has the following attributes:
- itemNumber: The item number ordered.
- saleItem: Indicates whether the price was a sale price (either “Y” or “N”).
- Child elements within <item>:
- <itemPrice>: The price paid for the item (as a decimal).
- <itemQty>: The quantity of the item ordered.

# Data Types:
- The schema defines data types such as xs:string, xs:date,
- xs:decimal, and xs:positiveInteger.

# This schema will validate the data structure in our orders.xml document.
