'''
Problem statement:

Write a program that display the following menu: 

1.) Calcualte Circumference

2.) Calculate Area

 Enter 1, 2 or 0 to exit

 In the case of option 1 and 2, the program should then prompt the user for the
 radius of the circle, perform calculation, and output the result. Then the program
 should re-display the menu. When option 0 is choosen the program should exit.

 Author: Nikesh Sapkota

 Date: 09/11/2021

 '''
            
            import sys

            def main():
                while (True):
                    #displaying option to the user
                    option = input("Please choose one of the option from here \n\n Enter 1 to Calculate the circumference of a circle \n Enter 2 to Calculate th Area of circle \n                              Enter 0 for Exit: \n\n Your Option: ")
                    option= float(option)
                    # selecting the values from users
                    if option == 1:
                        radius = input(" Enter the radius of circle: ")

                        #converting Str radius into float radius
                        radius= float(radius)
                        Circumference = 2* 3.14159* radius
                        print("The circumference of circle is: " , Circumference, "\n\n")

                    #Generating the condition and printing the values here    
                    elif option == 2:
                        radius = input("Enter the radius of circle: ")   
                        #converting Str radius into float radius
                        radius= float(radius)    
                        Area = 3.14159* (radius **2)
                        print("The Area of circle is: ", Area, "\n\n")

                    elif option ==0:
                        sys.exit()

            main()






