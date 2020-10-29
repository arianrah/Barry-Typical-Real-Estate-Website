model/db fields

### listing

id: int
realtor: int (foreign key [realtor])
title: str
address: str
city: str
province: str
postal: str
description: text
price: int
bedrooms: int
bathrooms: int
garage: int [0]
list_date: date
sqft: int
lot_size: float
is_published: bool [true]
photo_main: str
photo_1: str
photo_2: str
photo_3: str
photo_4: str
photo_5: str
photo_6: str

### realtor

id: int
name: str
photo: str
description: text
email: str
phone: str
is_mvp: bool [0]
hire_date: date

### contact

id: int
user_id: int
listing: int
listing_id: int
name: str
email: str
phone: str
message: str
contact_date: date
