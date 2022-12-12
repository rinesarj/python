def orderPizza(size, pepperoni=False, cheese=False):
    total = 0
    size = size.lower()

    # Pizza Order
    if size == 's':
        total += 15
    elif size == 'm':
        total += 20
    elif size == 'l':
        total += 25

    # Pepperoni   
    if pepperoni and size == 's':
        total += 2
    elif pepperoni:
        total += 3
    
    # Extra cheese
    if cheese:
        total += 1

    with open('pizzaOrder.txt','w') as f:
        f.write(f"{size.upper()} pizza\n")
        if pepperoni:
            f.write("extra pepperoni\n")
        if cheese:
            f.write("extra cheese\n")
        f.write("-"*10)
        f.write(f'\nprice: {total}')

orderPizza("M", True)
