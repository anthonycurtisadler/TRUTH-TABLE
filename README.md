# TRUTH-TABLE
TRUTH TABLE GENERATOR 

GENERATES A TRUTH TABLE ANALYSIS OF A PHRASE IN CONVENTIONAL LOGICAL NOTATION, WITH THE FOLLOWING OPERATORS:
PARANTHESES, AND, OR, LOGICAL IMPLICATION, LOGICAL EQUIVALENCE

A VARIABLE CAN BE ANY WORD CONSISTING OF NON-RESERVED SYMBOLS, e.g:
A,B,1,2,3,P,Q,Hippo,HIPPO,elephant1,elephant* 

FOR EXAMPLE: 

TRUTH TABLE FOR A&A>B
_____________________
(0):  A  B  | True   
(1):  A ~B  | False  
(2): ~A  B  | False  
(3): ~A ~B  | False  

TRUTH TABLE FOR (A|B)&~B
________________________
(0):  A  B  | False     
(1):  A ~B  | True      
(2): ~A  B  | False     
(3): ~A ~B  | False     

TRUTH TABLE FOR A>B&B>C&C>(D|E|F)&(E>~A)&(F>~A)&(D>A)
_____________________________________________________
(0) :  A  B  C  D  E  F  | False                     
(1) :  A  B  C  D  E ~F  | False                     
(2) :  A ~B  C  D  E  F  | False                     
(3) :  A ~B  C  D  E ~F  | False                     
(4) :  A  B  C ~D  E  F  | False                     
(5) :  A  B  C ~D  E ~F  | False                     
(6) :  A ~B  C ~D  E  F  | False                     
(7) :  A ~B  C ~D  E ~F  | False                     
(8) : ~A  B  C  D  E  F  | True                      
(9) : ~A  B  C  D  E ~F  | True                      
(10): ~A ~B  C  D  E  F  | True                      
(11): ~A ~B  C  D  E ~F  | True                      
(12): ~A  B  C ~D  E  F  | True                      
(13): ~A  B  C ~D  E ~F  | True                      
(14): ~A ~B  C ~D  E  F  | True                      
(15): ~A ~B  C ~D  E ~F  | True                      
(16):  A  B  C  D ~E  F  | False                     
(17):  A  B  C  D ~E ~F  | True                      
(18):  A ~B  C  D ~E  F  | False                     
(19):  A ~B  C  D ~E ~F  | False                     
(20):  A  B  C ~D ~E  F  | False                     
(21):  A  B  C ~D ~E ~F  | False                     
(22):  A ~B  C ~D ~E  F  | False                     
(23):  A ~B  C ~D ~E ~F  | False                     
(24): ~A  B  C  D ~E  F  | True                      
(25): ~A  B  C  D ~E ~F  | True                      
(26): ~A ~B  C  D ~E  F  | True                      
(27): ~A ~B  C  D ~E ~F  | True                      
(28): ~A  B  C ~D ~E  F  | True                      
(29): ~A  B  C ~D ~E ~F  | True                      
(30): ~A ~B  C ~D ~E  F  | True                      
(31): ~A ~B  C ~D ~E ~F  | True                      
(32):  A  B ~C  D  E  F  | False                     
(33):  A  B ~C  D  E ~F  | False                     
(34):  A ~B ~C  D  E  F  | False                     
(35):  A ~B ~C  D  E ~F  | False                     
(36):  A  B ~C ~D  E  F  | False                     
(37):  A  B ~C ~D  E ~F  | False                     
(38):  A ~B ~C ~D  E  F  | False                     
(39):  A ~B ~C ~D  E ~F  | False                     
(40): ~A  B ~C  D  E  F  | True                      
(41): ~A  B ~C  D  E ~F  | True                      
(42): ~A ~B ~C  D  E  F  | True                      
(43): ~A ~B ~C  D  E ~F  | True                      
(44): ~A  B ~C ~D  E  F  | True                      
(45): ~A  B ~C ~D  E ~F  | True                      
(46): ~A ~B ~C ~D  E  F  | True                      
(47): ~A ~B ~C ~D  E ~F  | True                      
(48):  A  B ~C  D ~E  F  | False                     
(49):  A  B ~C  D ~E ~F  | False                     
(50):  A ~B ~C  D ~E  F  | False                     
(51):  A ~B ~C  D ~E ~F  | False                     
(52):  A  B ~C ~D ~E  F  | False                     
(53):  A  B ~C ~D ~E ~F  | False                     
(54):  A ~B ~C ~D ~E  F  | False                     
(55):  A ~B ~C ~D ~E ~F  | False                     
(56): ~A  B ~C  D ~E  F  | True                      
(57): ~A  B ~C  D ~E ~F  | True                      
(58): ~A ~B ~C  D ~E  F  | True                      
(59): ~A ~B ~C  D ~E ~F  | True                      
(60): ~A  B ~C ~D ~E  F  | True                      
(61): ~A  B ~C ~D ~E ~F  | True                      
(62): ~A ~B ~C ~D ~E  F  | True                      
(63): ~A ~B ~C ~D ~E ~F  | True            

I wrote this program mainly to see if I could write a simple recursive parsing function. Hence no eval, and no libraries. 
Needless to say, this could be done much more simply.
