
# Introduction 
Most people have heard of  Java, the programming language can also help to manage stores through an efficient cashier system. However, not many people know how one actually goes about creating a cashier system in this language. That is why I am writing this essay - to demonstrate the process and instructions for setting up a cashier system with Catshop Java. This essay will present what I did and how I went about completing this task so that readers can gain insight into how to create their own accurate cashier systems using Catshop Java and maybe even add a few creative touches to it.

# How does all the code work together?
The Main class is responsible for starting all the clients in the cashier application. It is designed as a single application, which is good for testing the system without using Remote Method Invocation (RMI). The class begins by creating an instance of the LocalMiddleFactory, which is used to create objects to access the stock list. The Main class then starts the different clients such as the customer, cashier, back door, pick, display, and collection clients. Each client is started using the Model-View-Controller (MVC) pattern, which separates the logic of the application into three interconnected components: the model, the view, and the controller (Kumar, 2021). The model contains the data and the logic of the application, the view displays the data, and the controller handles the interactions between the user and the model. The Main class uses the LocalMiddleFactory to start each client, and it sets the default close operation of each client's window to exit on close.

# Cashie package
To effectively build a computer application that simulates the role of a cashier in a retail store. In the frontend server or the client side there has to be a cashier class. In this case, the "Cashier" package is created that includes a CashierModel class that handles data and logic, a CashierView class that handles the graphical user interface, and a CashierController class that handles user input and communicates between the Model and View.  Which acts as the role of a cashier in a retail store. The class allows users to input product codes to check if they are in stock and if available, add it to the basket. Once added, items are ready for purchase by clicking on “check out” at the bottom-right corner of the Cashier window. The code also contains extra functionality such as sound effects playing when various buttons are clicked or hovered over and even change button color upon interaction with them. 

# Adding a remove item button
 Featured in figure 1, we can see what this application looks like when code is properly implemented. Starting with the remove button, this feature is coded within three main components: 1. CashierController; 2. CashierModel; and 3. CashierView-- all of which are necessary for smooth functionality. In essence, these parts work together to allow users to easily remove an item from their basket or shopping cart within seconds. In detail, firstly,the Cashier Controller has a method called ‘remove_Item’ embedded into it which takes product number as input and calls corresponding methods in both the CashierModel and CashierView. Secondly coming onto Cashier Model where there is another method called 'remove_Item' which basically receives a product number as argument and attempts to delete it from basket of purchased items if not null initialized already before removing an item via looping through basket and returning modified instance of new basket back to controller class finally updating view accordingly when done correctly . Last but not least ,in order to provide a user-friendly interface alongside simplify meaningful implementation in the CashierView, there is a button labeled "REMOVE" and an input field for the product number. When the "REMOVE" button is clicked, the product number entered in the input field is passed to the "remove_Item" method in the CashierController. 

# Figure 1 

## Cashier Control
![unnamed (3)](https://github.com/user-attachments/assets/d089833c-4281-461f-af56-123ac14c0591)

## Cashier Model

![unnamed](https://github.com/user-attachments/assets/eebb5b28-7f00-475e-bde4-ba16511e50f9)

## CashierView
![unnamed](https://github.com/user-attachments/assets/641ac360-0bba-4371-866b-2ce705f4399d)

# Enhancing GUI

Creating a retail cashier simulation using Java can be accomplished with some simple code and few GUI components. With the right coding techniques, the application can be built to resemble an actual retail store’s cashier experience. For example, the buttons used in this simulator should have a color animation when they are hovered over or clicked on by the user (Figure 3). To do this, we need to create a class called Mouse_Clicker_Colour_Changer which will act as MouseListener for all the JButtons in the CashierView class. In addition to this, One must also remember about attaching these MouseListeners directly to each JButton component in order for it work correctly; without forgetting resetting their color back when mouse exited from button area so click effect retention is achieved at runtime successfully in our program – something only possible through expert use of Java and its components alone(Ali).

# Figure 2

## Mouse_Clicker_Colour_Changer 

![unnamed](https://github.com/user-attachments/assets/eacae430-b885-4536-81fa-da3dcb2bbbbc)

# Adding sound effects

First, Figure 3 should be set up by creating “Sound_Clip” and “Music_Fx” classes; these provide methods for playing sound effects specific to certain buttons or actions within the simulation. The Sound Clip  class contains instructions such as when it should produce a beep or buzzer sound, while different music files names can also be stored using the Music FX class fields. objects must then be created from these two classes before their associated methods are called on according to specified conditions. To facilitate understanding of how this works, an example is given in which pressing on a Buy button will call up that contained within Sound Clip – namely its play Beep function – while clicking on Check will activate Music Fx through its play Music method instead with Button Music1 as passed parameter value (Kensoft PH, 2019). 

# Figure 3
## Music_FX
![unnamed](https://github.com/user-attachments/assets/f5c1b07b-ba87-4fb0-9b68-ec4e18fbd2f9)

# Better basket 

Creating a cashier system using Catshop Java is not as hard as it may initially seem. After gaining familiarity with the object-oriented programming language, breaking down the process class by class will prove to be quite simple. The basis of this type of code comes from an extension called “Basket” which allows for the adding and subtracting of products, keeping track of quantity and identifying any repeat purchases when complete. To take things further, “BetterBasket” extends on this existing basket in order to sort products based on their price in descending order (as shown in figure 4). This means that every product within Basket needs to have its own add method overridden according to BetterBasket specifications which include sorting them first before anything else. Once level one is reached within their own coding system a loop can then be started that looks at individual products found within the basket and checks if they are repeated or has a quantity value set at zero - such items must immediately be removed from those collected by customers. Additionally, items that may become repeated need merge functions built into them so when the next purchase is made there are no extras added but rather just an increase in sale numbers for that specific goods being bought more than once (a specific function better explained through figure 4). In effect if every step has been followed through correctly returns should come back differently as per how one wished their shopping cart/cashier system would look after completion prompting readers or users alike they know exactly what they are purchasing while sorting each item according their pricing order all stored under customized parameters determined during design phase completion prior.

# Figure 4
## Better basket
![unnamed](https://github.com/user-attachments/assets/39836c8b-c800-4201-8ad4-080d75ce1867)

# Critical Review: why the implementation of the project are good

When it comes to software development, a well-designed, well-managed and well-implemented project is crucial for success. The codebase for the Catshop Java cashier system is a prime example of a project that excels in all three of these areas. Firstly, the design of the project is top-notch. The use of the Observer pattern, as seen in Figure 5, allows for a clean and organized structure, making the code easy to read and understand. The Observer pattern allows for a clear separation of concerns, where the Model, View, and Controller all have their specific responsibilities. This makes it easy for developers to add new features or make changes without affecting the rest of the codebase. Secondly, the management of the project is also exemplary. The use of clear and consistent naming conventions makes it easy to navigate the codebase and understand the purpose of each class and method. This makes it easy for developers like myself to understand the codebase and make changes without introducing bugs. Lastly, the implementation of the project is also very well done. The use of Java, as seen in Figure 5, allows for efficient execution and a wide range of libraries that can be used for various functionality. Additionally, the use of the Model-View-Controller pattern and the Observer pattern in the codebase allows for a clear separation of concerns, making the code easy to read and understand. This makes it easy for developers to add new features or make changes without affecting the rest of the codebase.

# Figure 5 

## Cashier client
![unnamed](https://github.com/user-attachments/assets/d3829040-7075-4f3b-9321-576c55c44f2d)

## PickClient
![unnamed](https://github.com/user-attachments/assets/28d01c35-7cfb-458c-9cbd-fca9a3ddd1e3)

# Critical Review: Improvements

One of the ways to improve the Cashier application is by incorporating a search function that allows users to search for items by name instead of product number. This can be achieved by adding a search bar or input field in the CashierView class and implementing a search function in the CashierController class that queries the stock list using the item name as a search parameter. Another way to enhance the application is by introducing a feature that offers discounts to customers. This can be done by adding a new method in the CashierController class that calculates the discount based on certain criteria such as the total purchase amount or the number of items in the basket. Furthermore, the CashierModel and CashierView classes should be updated to reflect the changes in the final purchase amount and display the discount information correctly. Finally, another way to improve the application is by adding a feature that allows cashiers to process returns or exchanges. This can be achieved by implementing methods in the CashierController and CashierModel classes to handle the return or exchange process, and updating the CashierView to include the necessary buttons and input fields for the user to initiate a return or exchange. This feature would involve several steps such as confirming the customer's purchase, checking for the item's return policy, updating the inventory and updating the customer's account.

# Conclusion 

In conclusion, the main class CashierClient serves as the entry point for the cashier application, it creates an instance of RemoteMiddleFactory and sets the stockRWInfo and orderInfo for it. It also creates the MVC components: the CashierModel, CashierView, and CashierController and sets them up to work together. The remove button was added by creating a method called remove_Item in the CashierController, which calls the corresponding method in the CashierModel and CashierView. The colors and sound effects were added by creating classes such as Sound_Clip and Music_Fx which provide methods for playing sound effects specific to certain buttons or actions within the simulation. Furthermore, the code also includes the BetterBasket class which sorts the products in the basket and checks for repeat products in the basket and merges the product. It also sorts the products in the basket and makes sure that there are no products with zero quantity in the basket. Overall, this cashier system is designed to provide a smooth and efficient shopping experience for custom

# Additional pictures 

![unnamed (2)](https://github.com/user-attachments/assets/27dbe24f-3fa6-47fd-a484-df1178bbfeff)

![unnamed (1)](https://github.com/user-attachments/assets/43a9738c-aeaa-4c7b-8616-e95c9e9efba8)

![unnamed](https://github.com/user-attachments/assets/2eb2e436-6717-4234-a03b-7b3afccaf177)


