# ApartmentListInterview2013 Solution

*Contains the problem statement and dictionary file for the interview question posed at the Fall 2013 UC Berkeley Startup Fair*

Your task is to count the size of the social network of the word "LISTY" in the dictionary provided.
We define two words as being friends if the edit distance between them is 1.  For this problem, we will
be using Levenshtein distance (http://en.wikipedia.org/wiki/Levenshtein_distance) as our edit distance.
The size of a word's social network is equal to the number of nodes who are within edit distance 1 from
that word, plus the number of words that are edit distance 1 from all of those words, and so on.  A word
is in its own social network, so if our dictionary is simply [HI] then the size of the social network
for HI is 1.

*For example:*

With dictionary `[HI HERE THERE HER HE SHE HEAR HALLOW]`
The size of the social network for HI is 7.  We calculate this as follows: HE is edit
distance 1 from HI, SHE and HER are edit distance 1 from HE, HERE and HEAR are edit 
distance 1 from HER, and THERE is edit distance 1 from HERE. As before, HI is in its 
own social network.

` 1 + (1+1) +  (1 + 1) +  1 + 1 = 7`
`HE  SHE HER  HEAR HERE THERE HI`
 
Please note that we want to see production quality code! Be sure to include any and all tests and
comments in addition to the logic behind your solution. We want to see code that you feel proud of 
and would check in to source control and push to production for use in a professional environment.
 
This readme and the dictionary you will be using is available at http://tiny.cc/LISTY (case sensitive!)
We have included the entire dictionary in dictionary.txt, as well as a few smaller dictionaries for you
to test your code on as you are developing a solution.  For your final answer, we want the size of the 
social network for LISTY given the entire 178,692 word dictionary in dictionary.txt
 
To submit your solution, please send your code and resume to:
solutions@apartmentlist.com 
and put the size of the social network for LISTY in the subject.
 
Good luck!
