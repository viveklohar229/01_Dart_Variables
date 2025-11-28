# Chapter 1: Variables 

Flutter aur Dart seekhne ka sabse pehla kadam. Agar aap data store karna nahi jante, toh aap app nahi bana sakte.

---

## 1.  What is a Variable? (Variable kya hai?)

**Definition:**
A variable is a named storage location in the computer's memory used to hold a value.

**Hindi Mein Samjhein:**
Variable ek **"Dabba" (Container)** ki tarah hota hai.
* Jaise Kitchen mein "Cheeni" rakhne ke liye dabba hota hai.
* Jaise Wallet mein "Paise" rakhne ke liye pocket hoti hai.
* Waise hi Coding mein "Data" rakhne ke liye Variable hota hai.

---

## 2.  Why do we use it? (Kyun use karte hain?)

Sochiye aap ek App bana rahe hain jisme user ka naam "Vivek" 100 jagah dikhana hai (Profile, Home, Settings, Chat).

* **Bina Variable ke:** Aapko 100 jagah haath se "Vivek" likhna padega. Agar kal ko user ne naam badal kar "Rahul" kar diya, toh aapko 100 jagah jakar code change karna padega. ❌
* **Variable ke saath:** Aap bas ek jagah `String name = "Vivek";` likhenge. Agar naam badla, toh bas us ek line mein change karo, poore app mein apne aap change ho jayega. ✅

**Faayde:**
1.  **Reusability:** Ek baar banao, baar-baar use karo.
2.  **Maintenance:** Changes karna aasaan hota hai.

---

## 3.How to write? (Syntax)

Dart mein variable banane ka ek fixed formula hai:
```dart
DataType variableName = Value;

DataType: Batana padta hai dabba kis cheez ka hai (Text hai? Number hai?).

variableName: Dabbe par kya label lagana hai (e.g., userName, age).

Value: Asli maal jo andar rakhna hai.

 Core Data Types (Isme kya kya rakh sakte hain?)
Dart mein 4 sabse zaroori types hote hain:

A. String (Text ke liye)
Jab bhi koi naam, address, ya message store karna ho. Humesha Quotes (" ") mein likhein.

Dart

String name = "Vivek Kumar";
String city = 'Mumbai';
String message = "Hello, kaise ho?";
B. int (Poore Number ke liye)
Integer (int) matlab bina point wale number. Jaise umar, saal, quantity.

Dart

int age = 24;
int year = 2025;
int quantity = 5;
C. double (Point wale Number ke liye)
Jab precision chahiye ho. Jaise price, percentage, weight.

Dart

double price = 99.50;
double percentage = 85.5;
double temperature = 36.6;
D. bool (Haan ya Na ke liye)
Boolean (bool) sirf do value leta hai: true (sahi) ya false (galat). Logic lagane ke liye sabse zaroori.

Dart

bool isLogin = true;
bool isDarkTheme = false;
 Advanced Concepts (Zero to Hero Section)
Sirf basic types kaafi nahi hain. Professional developers inka bhi use karte hain:

 var (Smart Variable)
Agar aapko type nahi pata, ya aap Dart par chhodna chahte hain, toh var use karein. Dart khud samajh jayega.

Dart

var college = "BCA College"; // Dart samajh gaya ye String hai
var marks = 90;              // Dart samajh gaya ye int hai
B. final vs const (Fixed Variables)
Kabhi-kabhi hum chahte hain ki ek baar value set ho gayi toh wo Change na ho.

final: Iski value code run hone par set hoti hai, par uske baad change nahi hoti. (Jaise: Aaj ka Date/Time).

const: Ye pathar ki lakeer hai. Code run hone se pehle hi fix honi chahiye. (Jaise: Pi ki value 3.14).

Dart

final String today = "Friday"; 
// today = "Saturday"; //Error aayega! Change nahi kar sakte.

const double pi = 3.14;
 Real Life Example (Zomato Food Order)
Chaliye dekhte hain ek real app mein ye sab ek saath kaise use hote hain.

Scenario: Ek user ne Zomato par Burger order kiya hai.

Dart

void main() {
  // 1. String: Khane ka naam
  String dishName = "Chicken Burger";
  
  // 2. String: Restaurant ka naam
  String restaurant = "Burger King";
  
  // 3. double: Price (Point mein ho sakta hai)
  double price = 149.50;
  
  // 4. int: Quantity (Kitne burger mangaye)
  int quantity = 2;
  
  // 5. bool: Kya Veg hai? (Chicken hai toh false hoga)
  bool isVeg = false;
  
  // 6. final: Order ID (Ye kabhi change nahi honi chahiye)
  final String orderId = "ZOM12345";

  // --- Printing the Receipt ---
  print("Order ID: $orderId");
  print("Dish: $dishName");
  print("From: $restaurant");
  print("Is Veg: $isVeg");
  
  // Calculation Logic (Chota sa)
  double totalBill = price * quantity;
  print("Total Bill: ₹$totalBill");
}
Output:

Order ID: ZOM12345
Dish: Chicken Burger
From: Burger King
Is Veg: false
Total Bill: ₹299.0

```dart
DataType variableName = Value;
