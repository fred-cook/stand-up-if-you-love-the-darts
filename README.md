# [stand-up-if-you-love-the-darts](https://www.youtube.com/watch?v=TfwnO3T5TY8)

Two programs for calculating darts checkouts given a total to achieve and a number of darts to achieve it, bearing in mind you have to finish on a double or the bull.

The programs are almost identical except one is written in Python and one is written in C, and one takes an hour to find all of the nine dart checkouts and one takes less than a minute.

They both have one small optimisation to reduce the number of darts you have to search for by calculating the minimum possible dart to reach a score, assuming all of the other darts scored their maximums.

## C program

Compile using your compiler of choice. I used GCC with the following command:
`gcc -o check_me_out check_me_out.c -O3`

The program can then be run with
`./check_me_out [target_score] [number_of_darts]`

I don't do any checking on inputs so don't put any naughty values in.

When I run it with a target score of 501 and 9 darts I get the expected 3944 possible cominations in a time of just over 30 seconds.

## Python Program

Run using `python check_me_out.py [target_score] [number_of_darts]`, again I've done no error checking so no naughty inputs please.

## Graph of possible checkouts

For fun here is a graph of how many combinations there are for each possible 3 dart checkout.

![checkouts](https://github.com/fred-cook/stand-up-if-you-love-the-darts/assets/135046797/1d3ec348-187c-4848-a4b4-1379cefbf7b5)
