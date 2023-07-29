# Gamer's Ticket Hub
## What's Gamer's Ticket Hub?
**Gamer's Ticket Hub** is a ticketing platform located in Riyadh's Gamer's Season that provides tickets for elite, community, and international/regional gaming tournaments.

### Ticket's Types
- Elite

  <img src="Elite_Tournaments.jpeg" width=450 height=450>
- Community

  <img src="Community.jpg" width=450 height=450>
- International/Regional

  <img src="Regional_Tournaments.jpeg" width=450 height=450>



| Elite | Community | International/Regional |
| ----------- | ----------- | ----------- |
| Elite tournaments are highly competitive gaming events for the best players in the world, offering large prizes and a chance to showcase their skills.| Community tournaments are open to players of all skill levels, offer a fun, social atmosphere, and are a great way to connect with other gamers. | International/regional tournaments are highly competitive gaming events that attract top players from around the world and offer significant prizes |
| Prices: 30-45 SR | Prices: 10-20 SR | Prices: 100-200 SR |



## Code Section

### Here is a summarized list of features related to the Gamer's Ticket Hub system. These snippets provide an overview of the key functionalities of the system and help users understand the purpose of the following code section.

***Cart Management***
```python
def cart_management():
    # It shows system available features to manage user cart
    print('Welcome to cart management section, please check the following options \n')
    print('1- Print cart elements\n')
    print('2- Add cart elements\n')
    print('3- delete cart elements\n')
    choice = int(input('Enter your choice'))
    if choice == 1:
        print_cart_elements(cart)     
    elif choice == 2:
        tournaments_options()
    elif choice == 3:
        delete_from_cart(cart)

```
***Print Cart Elements***
```python
def print_cart_elements(cart_elements):
    total_price = 0
    if(len(cart['Name']) == 0): #checks if cart is empty 
        choice = int(input('You have no items, write 1 to proceed to tournaments section or 0 to exit code'))
        if(choice == 1):
            tournaments_options()
        else:
            print('Thank you for your visit')
            return
    else:
        total_price = 0
        print('\nHere is your cart information\n')
        for name,date,price,Type in zip(cart_elements['Name'],cart_elements['Date'],cart_elements['Price'],cart_elements['Type']):
            print(f'Name : {name}')
            print(f'Date : {date}')
            print(f'price : {price}')
            print(f'Type: {Type}\n')
            total_price+=price
        choice = int(input("'What would you like to do next? Type '1' for Payment or '2' for Main Menu:'"))
        if(choice == 1 ):
            total = total_price
            return total
        else:
            cart_management()
```
***Delete Cart Elements***
```python
def delete_from_cart(cart_elements):
    
    #This feature displays the user's cart items and enables them to remove a specific ticket by entering its name."
    if(len(cart['Name']) == 0): #checks if cart is empty 
        choice = int(input('You have no items, write 1 to proceed to tournaments section or 0 to exit code'))
        if(choice == 1):
            tournaments_options()
        else:
            print('Thank you for your visit')
            return
    else:
        print('\nHere is your cart information\n')
        for name,date,price,Type in zip(cart_elements['Name'],cart_elements['Date'],cart_elements['Price'],cart_elements['Type']):
            print(f'Name : {name}')
            print(f'Date : {date}')
            print(f'price : {price}')
            print(f'Type: {Type}\n')
        print('To delete a ticket please enter ticket name')
        ticket_name = str(input('Ticket name : '))
        for name,date,price,Type in zip(cart_elements['Name'],cart_elements['Date'],cart_elements['Price'],cart_elements['Type']):
            if(name == ticket_name):
                cart['Name'].remove(name)
                cart['Price'].remove(price)
                cart['Date'].remove(date)
                cart['Type'].remove(Type)
        cart_management()
```
***Add Cart Elements***
```python
    choice = int(input('Would you like to book a ticket? please write 1 to yes and 0 to no'))
    while choice != 0:
        if(choice == 1):
            tournament_name = str(input('Please enter the name of tournament'))
            for name,date,price,Type in zip(cart_elements['Name'],cart_elements['Date'],cart_elements['Price'],cart_elements['Type']):
                if(tournament_name == name):
                    cart_choice = int(input('Add this ticket to your cart? Type 1 for Yes, 0 for No'))
                    if(cart_choice == 1):
                        cart['Name'].append(name)
                        cart['Date'].append(date)
                        cart['Price'].append(price)
                        cart['Type'].append(Type)
                        choice = int(input('Book another ticket? Type 1 for Yes, 0 for No:'))
                        if(choice == 1):
                            continue
                        else:
                            cart_management()
```

## Resources
- [Gamer's Season](https://gamers8.gg/?gclid=CjwKCAjw8ZKmBhArEiwAspcJ7pZ8nLiic469KQtv7tMpmjT0IWMNQ16Ls32qPzL-fWcogWIqmCDRdxoCawEQAvD_BwE)
