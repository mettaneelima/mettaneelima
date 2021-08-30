- 👋 Hi, I’m @mettaneelima
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
mettaneelima/mettaneelima is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
 cart = []
def addItem(item):
      cart.append(item)
      print("{] has been added to your cart".format(item))
def removeItem(item):
       try:
           cart.remove(item)
           print("{} has been removed from cart".format(item))
       exceppt:
           print("Sorry, we could not remove that item")
def showcart():
       if cart:
           for item in cart:
                print("=>{}".format(item))
       else:
                print("Sorry,your cart is empty.")
def clearcart():
         cart.clear()
         print("your cart has been emptied")
def main():
        done=False
        while not done:
                print("what action would you like to perform?")
                ans = input(\n**Quit\n**Add\n**Remove\n**Shhown\n**Clear:\n).title()
                if ans == "Quit":
                        if not cart:
                               print("Thanks for shopping with us")
                        else:
                               print("Thanks for shopping with us")
                               print("\n here are the items in your cart")
                               showcart()
                        done = True
                elif ans =="Add":
                     item = input("what item would uyou like to add?").title()
                     addItem(item)
                elif ans =="Remove":
                     showcart()
                     item = input("what would you like to remove?").title()
                     removeItem(item)
                elif ans == "Show":
                     print("Here is your cart:")
                     show cart()
                elif ans == "Clear":
                     print("Are you sure you want to clear your cart?")
                     surety=input("Yes/No:").upper()
                     if surety == "Yes":
                           clearCart()
                     else:
                           continue
