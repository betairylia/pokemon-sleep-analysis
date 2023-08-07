**tl;dr**:

- The true helping rate of pokemon seems significantly faster than said in there stats menu (`Frequency`), for passive play.
- Seems we have ~20% ingredient drops per help for berry specialists.
- For ingredient specialists however, this probability seems to be ~30%.

Only have used two sets of data and they do not agree on the true helping rates.  
Perhaps going to make some scripts for more calculation but idk when ;-;;  

## Data #1

Erayto @ 07/30/2023

<img src="./Pasted image 20230807171039.png" style="zoom:25%;" />
Metapod @ Lum berry (~31, +32, ++33)  
Lum berry x2 @ Snorlax  
Slept 34200s  

>Pichu 11 Berry / 1 apple   
>Squirtle 4 berry / 8 milk   
>Metapod+ : 70 pts 10 berries / 6 honey   
>Metapod++ : 66 pts 14 berries / 2 honey    
>Metapod~ : 61pts 16 berries / 0 honey (edited)  

>~: BER, 2b/1i, 4158s, 61, No nature  
>+: BER, 2b/1i, 4124s, 70, Helping bonus, Ingredient finding ++  
>++: BER, 2b/1i, 3727s, 66, Speed of help ++  
>Pichu: BER, 3b/1i, 3792s, berryS, Speed of help ++  
>Squirtle: ING, 1b/2i, 4419s, Skill Trigger M, Main skill chance++  

:~ 1612/31 = 52 (helped ~~26~~ 13 times) + 16 berries holding (8) = 21  
- 87318s (2.553x)

:+ 1120/32 = 35 (9?) + 10 berries (5) + 6 honey = 20  
- 82480s (2.412x)  

:++ 1848/33 = 56 (helped ~~28~~ 14 times) + 14 berries (7) + 2 honey (2) = 23  
- 85721 (2.506x)  

Serebii:  
Ingredient finding++ provides +20% on ingredient drop rates.  

### Ingredients correction  
Ingredient rate of above metapods: (average from ~ & ++):  
Pichu 4-1 (20%); ~ 8-0 (0%); ++ 7-2 (22.2%). => Approx. 14.06% (say, 15% is being used)  
- Likelihood: 39%, 27%, 26%  

If above was correct, then Metapod+ (5-6, 54.5%) => 35%?  
- Likelihood: 10%, so perhaps acceptable ig  

=> Sum LL of 15%: - 0.94 - 1.31 - 1.35 - 2.30 = -5.9  
=> Sum LL of 20%: - 0.89 - 1.78 - 1.20 - 1.92 = **-5.79**  

=> MLE: Ingredient has 20% chance for berry types?  

For squirtle: 4-4 (50%) => 23.2% likelihood. (Boosts for ING type?)  

With above correction of 20% ingredients, we can scale the corresponding # of helps in above data:  

:p 22.5 + 5 = 27.5 helps = 104280s (3.049x)  
:~ 16.25 + 8 = 24.25 helps = 100831.5s (2.948x)  
:+ 15 + 5 + 6 = 26 helps = 107224s (3.135x)  
:++ 17.5 + 7 + 2 = 26.5 helps = 98765.5s (2.887x)  

## Data #2

Soipask @ 08/06/2023  

<img src="Pasted image 20230807174932.png" style="zoom:25%;" />  
Slept for 9h15m (45000s)  

> Everyone 0% or low energy  
> Pikachu 16b-0i (8-0, 0%)  
> Raichu 22b-4i (11-4, 26.6%)  
> Larvitar 3b-6i (3-3, 50% ING)  
> Totodile 11b-0i (6-0, 0% --)  
> Charmander 8b-4i (8-2, 20% ING)  

Stats:  
> Pikachu 2646s, 2b/1i  
> Raichu 2169s, 2b/1i  
> Larvitar 4276s, 1b/2i Speed of help ++  
> Totodile 4455s, 2b/1i, Ingredient finding --  
> Charmander 3093s, 1b/2i  

Pikachu 1120 (32 berries (35p)?) -> 20 + 8 = 28 helps = 74088s (1.646x)  
Raichu 1088 (32 berries (34p)?) -> 20 + 15 = 35 helps = 75915s (1.687x)  
ING-Larvitar 280 (8 berries (35p)?) -> 10 + 6 = 16 helps? = 68416s (1.520x)  
Totodile 720 (20 berries (35p)?) -> 10 + 6 = 16 helps? = 71280s (1.584x)  

- Assuming nature makes ingredient% goes to 0%, which is unlikely.  
- will be 11.1 + 6 = 17.1 = 76229s if nature make ingredient% down by 10%. (seems more reasonable)  

ING-Charmander 324 (9 berries (36p)?) -> 11.25 + 10 = 21.25 helps = 65726.25s (1.461x)  

ING type mons seems having a significantly short amount of effective time.  
Hypothesis: ING-mons have more % to obtain ingredients per help. How much?  

Difference between 75000s:  
Larvitar 6584s = ~1.5 helps => Ingredient% should be 30%  
Charmander 9274s = ~3 helps => Ingredient% should be 35%  

### The Squirtle in data#1:  
Squirtle 4419s  
w/ 20% ingredient rate  
ING-Squirtle 462 (11 berries (42p)?) -> 13.75 + 8 = 21.75 helps = 96113.25s  
- (others got 104280, 100831, 107224, 98765.5 sec resp. (avg 102775), so squirtle is a bit shorter here)  

w/ 30%  
ING-Squirtle 462 (11 berries (42p)?) -> 15.71 + 8 = 23.71 helps = 104793.4s  

w/ 35%  
ING-Squirtle 462 (11 berries (42p)?) -> 16.92 + 8 = 24.92 helps = 110135.1s  

=> 30% seems benefical.
