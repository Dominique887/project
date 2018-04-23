## Project database 

## By: Dominique, Austin

#### This will create a database for the virtual closet application





create table Users (

userID int  primary key,

password text not null, 
);



create table Gallery (

CategoryID int not null,

userID int not null,

primary key (CategoryID),

foreign key (userID) references Users(userID)

);



create table Category (

shirtID text not null,

pantsID text not null,

sock text not null,

shoes text not null,

primary key (shirtID),

foreign key (pantsID) references Category(CategoryID),

);

insert into dbo.users
valus (1,'pa$$word','Dom');

Insert into dbo.Category
values(1,'Shirts',1),
                (2,'Red',1),
                (3,'blue with stripes',1),
                (4,'pink',1),
                (5,'green',1);

