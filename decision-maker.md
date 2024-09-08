# Decision maker
tool for making decision in cumbersome cases - when you have a lot of emotions ( or/and a lot of people )

## collect all factors that make (even potentially ) influence on your decision
during this "mind storm" think about:
* risks
* opportunities
* what you want to achieve directly ( goals ), indirectly ?
* what you will obtain after the achievement ?
* who also will be affected ?
* ...
   |  item   |
   |---------|
   | item A  |
   | item B  |
   | item C  |
   | item D  |
   | item E  |
   | item F  |
   | item G  |
   | item H  |
   | item I  |
   | item J  |
   | item K  |
   | item L  |
  

## probability 
1. Create second list with all the items from previous step.  
2. Sort them out from high probability ( on top ) to less probability ( on bottom ).  
   |  item   |
   |---------|
   | item A  |
   | item B  |
   | item G  |
   | item K  |
   | item H  |
   | item J  |
   | item E  |
   | item I  |
   | item C  |
   | item F  |
   | item D  |
   | item L  |

3. Detect "waterline" for the probability - rid off items below it, what is not gonna happen from your point of view.
   |  item   |
   |---------|
   | item A  |
   | item B  |
   | item G  |
   | item K  |
   | item H  |
   |-w--w--w-|
   | item J  |
   | item E  |
   | item I  |
   | item C  |
   | item F  |
   | item D  |
   | item L  |

4. Set likelihood [0.25, 0.5, 0.75, 1]
   where 1 - will be for sure and 0.25 - low possibility.
   |  item   | likelihood |
   |---------|------------|
   | item A  |     1      |
   | item B  |     1      |
   | item G  |     0.5    |
   | item K  |     0.5    |
   | item H  |     0.25   |

## importancy
1. Take list from previous step and sort them out from most influenced to less influenced items ( what will affect your decision ).
2. Detect equal item from influence on decision point of view.
   |  item   |   diff   |
   |---------|----------|
   | item B  |          |
   | item A  |          |
   | item G  |    x     |
   | item H  |    x     |
   | item K  |          |

3. Next, just image that you have possibility to set between elements diff-value as [1,2,3]
   |  item   |   diff   |
   |---------|----------|
   | item B  |    3     |
   | item A  |    1     |
   | item G  |    2     |
   | item H  |    2     |
   | item K  |          |

4. Try to detect elements, where 3 is not enough, mark all of them.
   |  item   |   diff   |
   |---------|----------|
   | item B  |    3 x   |
   | item A  |    1     |
   | item G  |    2     |
   | item H  |    2     |
   | item K  |          |
5. Read all marked elements again and try to evaluate one maximal biase between previous element and marked element.
   |  item   |   diff   |
   |---------|----------|
   | item B  |    5     |
   | item A  |    1     |
   | item G  |    2     |
   | item H  |    2     |
   | item K  |          |

6. Set proper value for your maximal marked element and set corresponding values agains rest of marked elements.

7. For each item calculate importancy to summarize all previous values, start from 1
   |  item   |   diff   |  influence    |
   |---------|----------|---------------|
   | item B  |    5     |       9       |
   | item A  |    1     |       4       |
   | item G  |    2     |       3       |
   | item H  |    2     |       3       |
   | item K  |          |       1       |
   

## calculate factor
1. multiply influence on likelihood for all the elements 
   |  item   |     factor      |
   |---------|-----------------|
   | item B  |       9*1       |
   | item A  |       4*1       |
   | item G  |       3*0.5     |
   | item H  |       3*0.5     |
   | item K  |       1*0.25    |

2. sort them out according to factor value 
   |  item   |     factor    |
   |---------|---------------|
   | item B  |       9       |
   | item A  |       4       |
   | item G  |       1.5     |
   | item H  |       1.5     |
   | item K  |       0.25    |


## positive/negative
1. for each of the item detect influence on the process
   |  positive  |   neutral   |  negative   |
   |------------|-------------|-------------|
   |    +       |     %       |     -       |
2. and set for each item 
   |  item   |     factor    |
   |---------|---------------|
   | item B  |      +9       |
   | item A  |      -4       |
   | item G  |      %1.5     |
   | item H  |      %1.5     |
   | item K  |      +0.25    |

## evaluation
evaluate each of your options with set of item from previous list 
and calculate factor 
YES: B, G, H, K =  6.25  ( winner )
 NO: A, G, H    = -4
