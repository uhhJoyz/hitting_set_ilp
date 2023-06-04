write_from_sets(sets, filepath):
    
    A function that takes a list of sets and a name and writes the sets to 
    a text file in the form of an ILP. Use this to generate text files
    that represent the ILP formation of the Hitting Set Problem.
    
    :param sets: List<List<int>> : a list of sets 
    :param filepath: String : a path for a file without a file extension 
    :return: void

from_sets(sets):
    
    A function to calculate the minimum hitting set from a list of sets
    
    :param sets: List<List<int>> : the sets of the hitting set problem
    :return: List<int> : the minimum tags required to cover the sets

solve(filepath):
    
    The solver function. Takes in a hitting set problem as specified by the
    ILP reduction, outputs the minimum number of tags required to hit each
    of the sets at least once. Use this when solving the hitting set 

    :param filepath: string : the path to the corresponding 
    ILP formulation of the hitting set problem

    :return: List<int> : the minimum sets required to hit 
    all the elements in the universal set

hitting_set_ilp(n, t, B):
    
    A helper function that takes in the number of data items, followed by the 
    number of sets, followed by the resulting B matrix and returns the
    solution to the corresponding minimum hitting set problem

    :param n: int : the number of data items
    :param t: int : the number of sets
    :param B: List<List<int>> : the B matrix from the hitting set problem
    :return: List<int> : the minimum tags required to hit items in the universal set