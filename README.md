Download Link: https://assignmentchef.com/product/solved-c-programming-language-project-1
<br>
Professor Oak who is known as Pokémon creator, lost his laboratory on a explosion because of an mischievous fire Pokémon. After so much effort, Prof. Oak rebuild his own lab but he couldn’t activate Pokémon creating machine because storage of the machine has broken. Professor can do wonders with Pokémon’s but he doesn’t know anything about software developing. Therefore, he asked students of Gebze Technical University for help to make the machine functional again. Professor send an image of the old machine’s control panel that is shown below:<sub>       </sub>










You are expected to code a function for each menu option. Write the code of the functions that

are shown below by obeying given function prototypes.




<strong>Part 1. </strong>Write a function that takes shape of the Pokémon as an input and calculates area of the shape and returns it. Parameters that are used to calculate the area of the shape must be taken from the user in the function. Number of the parameters can be changed according to the shape of the Pokémon. The shapes could be rectangular, square or circular and all the shape types must be pre-defined on the program like: Square is 1, rectangular is 2 and circular is 3. The function prototype is:




double CreateBody (int shape)




<strong>Part 2. </strong>Write a function that takes a color code as an integer input to paint the Pokémon and returns revised color code. If the color code is between 0<sub>     </sub>

Page <strong>1</strong> of <strong>3 </strong>







and 1000 then the function returns modulo five of the code, otherwise, it always returns 1 as the revised color code. The colors could be red, yellow, blue, black or white and all the colors must be pre- defined on the program like: red is 0, yellow is 1, blue is 2, black is 3 and white is

<ol start="4">

 <li>The function prototype is:</li>

</ol>

int SetColor (int color)




<strong>Part 3. </strong>Write a function that takes shape and size of the body as an input and calculates length of one move of the Pokémon and returns the length. The length of one move is equal to perimeter of the body (Assume that the shorter edge is 5 if the shape is rectangular). The function prototype is:

double LoadMoves(int shape, double body_size)




<strong>Part 4. </strong>Write a function that specifies attack power of the Pokémon. It takes lower and upper bound of the attack power and generates a random integer attack power between the bounds and returns the power. The function prototype is:

int SetAtackPower(int lower_bound, int upper_bound)




<strong>Part 5. </strong>Write a function that prints created Pokémon with its wonderful specifications like the figure that is shown below:




(Rectangular Pokémon example)




XXXXXXX<sub>           </sub>

XXXXXXX<sub>           </sub>

XXXXXXX<sub>           </sub>

XXXXXXX<sub>           </sub>

XXXXXXX<sub>           </sub>

Name: Rectangular Pokémon<sub>       </sub>

Size: 35<sub>        </sub>

Color: Red<sub>   </sub>

Move: 24<sub>        </sub>

Attack Power: 78




(Circular Pokémon example)




X

X               X

X

Name: Circular Pokémon<sub>               </sub>

Size: 28.26<sub>               </sub>

Color: Blue<sub>               </sub>

Move: 18.84<sub>               </sub>

Attack Power: 102







As you notice, the shapes of the Pokémon’s are dynamic and that means you should print them according to their size. On the figure that is shown above, the function prints X’s by the length of the edges on vertical and horizontal direction (Assume that the shorter edge is 5 if the shape is rectangular). If the shape is




Page <strong>2</strong> of <strong>3 </strong>




circular then put tabs between two X’s which are on the middle of the shape as much as minus one of the radius of the shape, and align the other rows as expected by using the middle row. The function prototype is:




void ShowPokemon(int shape, double body_size, int color,

double move_length, int attack_power)




The main function must be li ke as shown above:

…




int main ()<sub>               </sub>

{

<sub> </sub>int shape, color, attack_power; <sub> </sub>double size_of_body, move_length; shape = RECTENGULAR / CIRCULAR / SQUARE // Pick one of them size_of_ body = CreateBody (shape) color = 798




<sub> </sub>color = SetColor(color) <sub> </sub>move_length = LoadMoves(shape, size_of_body) <sub> </sub>attack_power = SetAttackPower (0, 150)

<sub> </sub>ShowPokemon(shape, size_of_body, color, move_length, attack_power)

}


