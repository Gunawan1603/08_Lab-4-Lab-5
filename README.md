# 08_Lab 4, Lab 5

BAHASA PEMROGRAMAN

TEKNIK INFORMATIKA

UNIVERSITAS PELITA BANGSA

NAMA : GUNAWAN

NIM     : 312010191

KELAS   : TI.20.B1

DOSEN   : Agung Nugroho,S.Kom.,M.Kom

Tugas : Pertemuan 9

**List, Tuple dan Dictionary**

- **List**

• Python menawarkan berbagai tipe data
majemuk yang sering disebut sebagai
sequence.<br>
• List (Daftar) adalah salah satu datatype
yang paling sering digunakan dan
sangat serbaguna yang digunakan
dengan Python.<br>
• Pada pemrograman Python, List dibuat
dengan menempatkan semua item
(elemen) di dalam kurung siku [],
dipisahkan dengan tanda koma.<br>

- **How to access elements from a list?**

• To access values in lists, use the square brackets for slicing along with the
index or indices to obtain value available at that index.<br>
• Index starts from 0. So, a list having 5 elements will have index from 0
to 4.<br>
• The index must be an integer.<br>
Example:<br>
> list1 = [ ' physics' , ' chemistry' , 1997, 2000] ;<br>
list2 = [ 1, 2, 3, 4, 5, 6, 7 ] ;<br>
print ("list1[ 0] : ", list1[ 0] )<br>
print ("list2[ 1: 5] : ", list2[ 1: 5] )<br>

- Syntax Program Python List :

![08_Lab 4, Lab 5](Gambar/01_List1.jpg)

- Run Program Python :

![08_Lab 4, Lab 5](Gambar/02_RunList1.jpg)

- **Negative indexing**

• Python allows negative indexing for its sequences.<br>
• The index of -1 refers to the last item, -2 to the second last item and so on.<br>
Example:<br>

> my_list = [ ' p' , ' r' , ' o' , ' b' , ' e' ]<br>
print(my_list[ -1] ) # Output: e<br>
print(my_list[ -5] ) # Output: p<br>

- Syntax Program Python Negative indexing :

![08_Lab 4, Lab 5](Gambar/03_List2.jpg)

- Run Program Python :

![08_Lab 4, Lab 5](Gambar/04_RunList2.jpg)

- **How to slice lists in Python?**

• We can access a range of items in a list by using the slicing operator
(colon).<br>
> my_list = [ ' p' , ' r' , ' o' , ' g' , ' r' , ' a' , ' m' , ' i' , ' z' ]<br>
> #elements 3rd to 5th<br>
> print(my_list[ 2: 5] )<br>
> #elements beginning to 4th<br>
> print(my_list[ : -5] )<br>
> #elements 6th to end<br>
> print(my_list[ 5: ] )<br>
> #elements beginning to end<br>
> print(my_list[ : ] )<br>

- Syntax Program Python slice lists :

![08_Lab 4, Lab 5](Gambar/05_List3.jpg)

- Run Program Python :

![08_Lab 4, Lab 5](Gambar/06_RunList3.jpg)

- **Change or add elements in List**

• List are mutable, meaning, their elements can be changed unlike string or tuple.<br>
• We can use assignment operator (=) to change an item or a range of items.<br>

- **Change Element**

> #mistake values<br>
odd = [ 2, 4, 6, 8]<br>
#change the 1st item<br>
odd[ 0] = 1<br>
#Output: [ 1, 4, 6, 8]<br>
print(odd)<br>
#change 2nd to 4th items<br>
odd[ 1: 4] = [ 3, 5, 7]<br>
#Output: [ 1, 3, 5, 7]<br>
print(odd)<br>

- Syntax Program Python Change Element :

![08_Lab 4, Lab 5](Gambar/07_List4.jpg)

- Run Program Python :

![08_Lab 4, Lab 5](Gambar/08_RunList4.jpg)

- **Add Element**

• We can add one item to a list using append() method or add several items using extend() method.<br>

> odd = [ 1, 3, 5]<br>
odd. append(7)<br>
#Output: [ 1, 3, 5, 7]<br>
print(odd)<br>
odd. extend([ 9, 11, 13] )<br>
#Output: [ 1, 3, 5, 7, 9, 11, 13]<br>
print(odd)<br>

- Syntax Program Python Add Element :

![08_Lab 4, Lab 5](Gambar/09_List5.jpg)

- Run Program Python :

![08_Lab 4, Lab 5](Gambar/10_RunList5.jpg)

- **Remove elements**

• We can delete one or more items from a list using the keyword del. It
can even delete the list entirely.<br>

> my_list = [ ' p' , ' r' , ' o' , ' b' , ' l' , ' e' , ' m' ]<br>
#delete one item<br>
del my_list[ 2]<br>
#Output: [ ' p' , ' r' , ' b' , ' l' , ' e' , ' m' ]<br>
print(my_list)<br>

- **Add Element**

• We can also use + operator to combine two lists. This is also called
concatenation.<br>
• The * operator repeats a list for the given number of times.<br>

> odd = [1, 3, 5]<br>
#Output: [1, 3, 5, 9, 7, 5]<br>
print(odd + [9, 7, 5])<br>
#Output: ["re", "re", "re"]<br>
print(["re"] * 3)<br>

- Syntax Program Python Add Element :

![08_Lab 4, Lab 5](Gambar/11_List6.jpg)

- Run Program Python :

![08_Lab 4, Lab 5](Gambar/12_RunList6.jpg)

- **Remove elements**
- 
• We can delete one or more items from a list using the keyword del. It
can even delete the list entirely.<br>

> my_list = [ ' p' , ' r' , ' o' , ' b' , ' l' , ' e' , ' m' ]<br>
#delete one item<br>
del my_list[ 2]<br>
#Output: [ ' p' , ' r' , ' b' , ' l' , ' e' , ' m' ]<br>
print(my_list)<br>

- **Basic List Operations**
- 
• Lists respond to the + and * operators much like strings; they mean
concatenation and repetition here too, except that the result is a
new list, not a string.<br>

**Tuple**

• Tuple sama seperti List, hanya saja pada tuple datanya bersifat tetap
atau tidak dapat diubah-ubah.<br>
• Karena berbentuk sequences maka operasi-operasi di atas dapat
diterapkanterhadap tuples.<br>

> #! /usr/bin/python<br>
tup1 = (' physics' , ' chemistry' , 1997,2000) ;<br>
tup2 = (1, 2, 3, 4, 5, 6, 7 ) ;<br>
print ("tup1[ 0] : ", tup1[ 0] ) ;<br>
print ("tup2[ 1: 5] : ", tup2[ 1: 5] ) ;<br>

**Dictionary**

• Dictionaries adalah koleksi pasangan item-item berasosiasi dimana
setiap pasangan terdiri dari suatu key dan value.<br>
• Pasangan key-value ini ditulis seabagai key:value.<br>
• Dictionaries ditulis dipisahkan koma dalam kurung kurawal.<br>

> #! /usr/bin/python
dict = {' Name' : ' Zara' , ' Age' : 7, ' Class' : ' First' }<br>
print ("dict[ ' Name' ] : ", dict[ ' Name' ] )<br>
print ("dict[ ' Age' ] : ", dict[ ' Age' ] )<br>

**Accessing Values in Dictionary**

• To access dictionary elements, you can use the familiar square
brackets along with the key to obtain its value.<br>

> #! /usr/bin/python<br>
dict = {' Name' : ' Zara' , ' Age' : 7, ' Class' : ' First' }<br>
name = dict[ "Name"]<br>
age = dict[ "Age"]<br>
class= dict. get("Class")<br>
class= dict. get("Class", "Alternate value")<br>

**Updating Dictionary**

• You can update a dictionary by adding a new entry or a key-value pair,
modifying an existing entry<br>

> #! /usr/bin/python<br>
dict = {' Name' : ' Zara' , ' Age' : 7, ' Class' : ' First' }<br>
dict[ ' Age' ] = 8; # update existing entry<br>
dict[ ' School' ] = "DPS School"; # Add new entry<br>
print "dict[ ' Age' ] : ", dict[ ' Age' ]<br>
print "dict[ ' School' ] : ", dict[ ' School' ]<br>

**Delete Dictionary Elements**

• You can either remove individual dictionary elements or clear the
entire contents of a dictionary.<br>
• You can also delete entire dictionary in a single operation.<br>

> #! /usr/bin/python<br>
dict = {' Name' : ' Zara' , ' Age' : 7, ' Class' : ' First' }<br>
del dict[ ' Name' ] ; # remove entry with key ' Name'<br>
dict. clear() ; # remove all entries in dict<br>
del dict ; # delete entire dictionary<br>
print "dict[ ' Age' ] : ", dict[ ' Age' ]<br>
print "dict[ ' School' ] : ", dict[ ' School' ]<br>


Cukup sekian latihan materi yang di berikan oleh dosen pembimbing.

**Terimakasih**




