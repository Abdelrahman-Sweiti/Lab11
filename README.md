## Explaination 

The "Hotel" table represents a hotel in the system.
It has attributes such as HotelID (primary key), Name, City, State, Address, and Phone Number.
The HotelID is a unique identifier for each hotel.
Each hotel can have multiple rooms associated with it.
Room:

The "Room" table represents individual rooms within a hotel.
It has attributes such as RoomID (primary key), HotelID (foreign key referencing Hotel), RoomNumber, Layout, Nickname, Price, and IsPetFriendly.
The RoomID is a unique identifier for each room.
The HotelID is a foreign key referencing the corresponding hotel to which the room belongs.
Each room can have various properties like RoomNumber (room identifier), Layout (room layout type), Nickname (room nickname), Price (room price), and IsPetFriendly (indicating if the room is pet-friendly).
Amenity:

The "Amenity" table represents amenities that can be associated with rooms.
It has attributes such as AmenityID (primary key) and Name.
The AmenityID is a unique identifier for each amenity.
Each amenity has a Name, which represents the specific feature or service provided by the hotel.
RoomAmenity:

The "RoomAmenity" table represents the many-to-many relationship between rooms and amenities.
It serves as a junction table to associate specific amenities with specific rooms.
It has attributes such as RoomAmenityID (primary key), RoomID (foreign key referencing Room), and AmenityID (foreign key referencing Amenity).
The RoomAmenityID is a unique identifier for each entry in the junction table.
The RoomID is a foreign key referencing the room to which the amenity is associated.
The AmenityID is a foreign key referencing the amenity associated with the room.
The relationships between the tables are as follows:

One Hotel can have multiple Rooms (one-to-many relationship between Hotel and Room).
Each Room belongs to one Hotel (many-to-one relationship between Room and Hotel).
Each Room can have multiple Amenities (many-to-many relationship between Room and Amenity).
Each Amenity can be associated with multiple Rooms (many-to-many relationship between Amenity and Room).


## WhiteBoard
![image](https://github.com/Abdelrahman-Sweiti/Lab11/assets/102755704/752b8011-cbb4-4d79-b789-95163cb6b112)
