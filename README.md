# rock-scissor-paper-game


import 'dart:math';
import 'dart:io';
void main() {
print("welcome to the game");
Map rules={
"rock":"scissor",
"scissor":"paper",
"paper":"rock",};
List computerChoice=["rock","paper","scissor"];
var random=Random();
String c=computerChoice[random.nextInt(3)];
//print(c);
print("Enter Your Choice");
var userChoice=stdin.readLineSync()!;
if(rules[userChoice]==c){
print("User Win");}
else if(rules[c]==userChoice){
print("Computer Win");
}
else if(rules[c]==rules[userChoice]){
print("drawww");
}
else{
print("Invalid Choice");
}

}
