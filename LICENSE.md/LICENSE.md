  
  // Task 1
  
  type runway = string;;
type runway = string

# type kind = Domestic | International;;
type kind = Domestic | International

# type planeSize = Medium | Large;;
type planeSize = Medium | Large

# type gate = int * planeSize;;
type gate = int * planeSize

# type accMethod = Car | Bus | Train;;
type accMethod = Car | Bus | Train

# type terminal = string * gate * kind * accMethod;;
type terminal = string * gate * kind * accMethod

# type airport = string * runway * terminal;;
type airport = string * runway * terminal 


# let arlanda = ("Arlanda", ["One", "Two"], ["Terminal 5", [(1, Large), (2, Medium)], International, [Car, Bus]]);;

//Output:

val arlanda :
  string * (string * string) list *
  (string * ((int * planeSize) * (int * planeSize)) list * kind *
   (accMethod * accMethod) list)
  list =
  ("Arlanda", [("One", "Two")],
   [("Terminal 5", [((1, Large), (2, Medium))], International, [(Car, Bus)])])

