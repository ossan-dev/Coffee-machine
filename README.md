# Coffee-machine

## Fixes

1. keep decreasing the amount of the due money as long as we insert coins
1. add a check on the number of coins inserted by the user. Otherwise, the user can insert an endless number of coins (updated by asking if he wishes to continue or stop there)
1. if you do a second operation it won't manage the remainder correctly (such as I take another cappuccino)
1. the insert money function is not clear: it only asks me to `Enter your money:`. As mentioned above, you should keep asking for money and decrease the amount due. (updated this one. If you have enough money and you want to purchase again, it will not ask for any money)

<h1>Coffee Machine</h1>
<h3>Overview</h3>
<p>
This project implements a simple interactive coffee machine simulation. Users can select various coffee options, make payments, and receive their chosen beverages. The project is divided into modular files, each handling specific functionalities.
</p>

<h2>Files</h2>
<h4>1. main.py</h4>
<p><b>Description:</b> The main script that orchestrates the coffee machine simulation.<br>
<b>Responsibilities:</b><br>
User interface and menu interaction.<br>
Integration of Menu, MoneyMachine, and CoffeeMaker functionalities.</p>
<h4>2. menu.py</h4>
<p><b>Description:</b> Defines the menu and menu item classes for different coffee options.<br>
<b>Responsibilities:</b><br>
Menu item creation and initialization.<br>
Retrieving available menu items and finding a specific drink.</p>
<h4>3. money_machine.py</h4>
<p>
<b>Description:</b> Manages the financial aspects of the coffee machine, including payment and change calculation.<br>
<b>Responsibilities:</b><br>
Handling user input for money.<br>
Processing payments and making change.<br>
Keeping track of profits.
</p>
<h4>4. coffee_maker.py</h4>
<p><b>Description:</b> Simulates the coffee-making process.<br>
<b>Responsibilities:</b><br>
Deducting required ingredients from available resources.<br>
Displaying a message for the user when the coffee is ready.</p>

<h3>How to Run the Coffee Machine Project</h3>

<h4>1.  Clone the Repository:</h4>

```
git clone https://github.com/shohanR/Coffee-machine.git 
cd your-repository
```

<h4>2.  Run the Coffee Machine:</h4>

```
python main.py
```

<h4>3.  Interact with the Menu:</h4>
<ul>
  <li>Follow the on-screen instructions to choose a coffee option.</li>
  <li>Enter the corresponding number for your desired coffee.</li>
</ul>

<h4>4.  Make Payments:</h4>
<ul><li>Enter the required amount when prompted.</li></ul>

<h4>5. Repeat or Exit:</h4>
<ul><li>After making a purchase, choose to make another purchase or exit the program.</li></ul>

<h3>Dependencies</h3>
<ul><li>Python 3.x</li></ul>

<h3>Notes</h3>
<p>ANSI escape codes are used for colored output. Make sure your terminal supports ANSI escape codes for the best visual experience.</p>
