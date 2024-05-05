# BCD_7SEGMENT

![image](https://github.com/RESMIRNAIR/BCD_7SEGMENT/assets/154305926/804ab8db-8637-45ac-b10f-80e77d818d61)

# VERILOG CODE:
~~~
module segment7(

     bcd,

     seg
    
    );
    
     input [3:0] bcd;
    
     output [6:0] seg;
     
     reg [6:0] seg;

    always @(bcd)
    
    begin
    
        case (bcd)
        
            0 : seg = 7'b0000001;
            
            1 : seg = 7'b1001111;
            
            2 : seg = 7'b0010010;
            
            3 : seg = 7'b0000110;
            
            4 : seg = 7'b1001100;
            
            5 : seg = 7'b0100100;
            
            6 : seg = 7'b0100000;
            
            7 : seg = 7'b0001111;
            
            8 : seg = 7'b0000000;
            
            9 : seg = 7'b0000100;
            
            default : seg = 7'b1111111; 
        
        endcase
    
    end

    endmodule
    ~~~
    ** OUTPUT**:

    ![BCD](https://github.com/teja2134/BCD_7SEGMENT/assets/161149578/17d23b2d-1b69-4569-82be-4de11a4890fc)
