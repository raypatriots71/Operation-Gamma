# Operation_Gamma

----------------Contributors-------------------
  raypatriots71 - Rohan Ray
  Kavar814 - Kavin M. Govindarajan
  mjoy0210 - Joydeep Mukherjee
  ACSarma - Arun C. Sarma
  amsraman - Aditya Sundaram
  amirkhanaursrk - Manav Majumdar
  ravitejaaechan - Raviteja Aechan
----------------Purpose------------------------
To create a programming language in which everything is returnable.
----------------Syntax-----------------
Heres what I have so far  ( might need some tweaking )

. = Of
_ = to
, = Chain (useless)( don't really need it unless it's useful) ( )
{} = Conditional
= = Equal
; = Apply

X.(2,3).add //x=5

In add(a,b).construct( a + b) //function
In square(a).construct( a*a)
In mult( a b).construct(a*b)

Y.(X).Square //25
Y.(X).Square,mult // err mult needs 2 terms

Method.y.(X) //square
Y.method.y.(X) //25
Y.method.y.x //undefined

[A] //Meet true iterate
[0 to 3] // 0 false 1 false 2 false 3 true
{ [A] }( y.y.add) //loop a times within conditional []
Y.6 F.{ [ 0 to 3 ] }(y.(y).sqare) //F= 2,821,109,907,456


//Fibbonachi
In fibbonachi(length).construct(
start.0,c,next, second.1,
{ [0 to length] }(
{c lessthan 1 }(next.c);().construct(
next.(first second).add
first equal second
second equal next)
)

Fibresult.(6).fibboonachi


Some theory: () code resides in this automatically
{} Returns object
; Applies to previous object
heres what i ahve so far

{ condtional } ( true statement ) ;().construct( falsestatement)
^^ if else
yeah needs work
so every variable is an object
if its too confusing
then just remember this
it eliminates typecasting
not like javascript
that has typecasting
but like Y.(HELLO WORLD) // y's (hello world) is of type value
and Y.(8) would still exist as a property of Y
sort of like everything is a tree
to declare a variable
Y.(6) //y is set to 6
but if you add a contstructor
Y.(6).square // the .square returns (36) to the 6 property of Y
so everything binds to each other and can be used independtly
so Y.(6).constructor returns .square
to declare functions you use in  //input
{ conditional }
[ from one number to another ( its a loop ) ]
another thing is that the code can be written psuedo-english but still be back into a codable sort
ex. Y.(8).square   // Y of (8) of square constructor
the purpose of this programming language is to bind other languages together
the other purpose is to add interoperability to oop parents and children

yeah thats why i needed help
after writing all of that i realized that constructors are still enclosed in () so it would interfere with order of ops
and then theres the problem with javascript that i intend to fix   
1. javascript cant compute big numbers
2. javascript confuses async and sync
whatever
here is how functions would be declared
parent.(anything inside these is returned to the parent)
so
for functions
in randomFunctionName( a, b).construct(a + b )
it returns a + b to randomFunctionName method
so
Y.(7,6).randomFunctionName //13
and it would translate as
Variable Y of (7 6) of method randomFunctionName
so yeah
how do you want to get started on the language
and lets put it on git so we could have as much supporters as we can
