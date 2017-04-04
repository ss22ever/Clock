# clock
In this program we have designed an analogue clock which tells the current time on the systems clock using graphics in c programming language.

We start the code by include the header files “stdio.h” “conio.h” “dos.h” “graphics.h” and “process.h”.

In the beginning we will make three functions namely:-

“calculatehrs(int h)”
“calculatemin(int m)”
“changehrs( int m, int a)”
In first function, hour’s value is received by the formal parameters and then check and whichever case it satisfies and x stores the value of the certain angle where it has to point on the clock. For example

        int calculatehrs(int h)
       {int x;
         switch(h)
         {case 0: x=90;                       
          break;
          case 1:
          case 13: x=60;
          break;
          case 2:
          case 14: x=30;
          break;
          case 3:
          case 15: x=0;
          .
 
         
Second function, minute’s value is received by the formal parameters and then check and whichever case it satisfies “x” is assigned some value, but in this case minutes are first divided by 5. For example

    int calculatemin(int m)
     {int x;
      if(m%5==0)
       {switch(m)
       {case 0: x=90;
         break;
        case 5: x=60;
         break;
        case 10: x=30;
         break;
        case 15: x=360;
         break;
        case 20: x=330;
        
Its code is same as the code of hours as it marks that the minutes are either 5, 10, 15, 20, etc so it is either on 1,2,3 till 12.

If it is not a multiple of 5 then again it is checked if it is more than 0 and less than 15 then x is assigned the value according to the graphics screen.



