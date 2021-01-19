import time
from yahoo_fin import stock_info

brands=input("enter the company")
while True:
    current_time=time.strftime("%H:%M:%S")
    price=stock_info.get_live_price(brands)
    print(price)   
    if price<3104:
        print("sell selll")
    elif price<3304:
        print("invest investtt")
    elif price<3804:
        print("profit")
    else:
        pass
     