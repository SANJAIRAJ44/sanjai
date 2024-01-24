// Code your testbench here
// or browse Examples
module tb;
  reg a,b;
  wire c,s;
  HA halfadd(a,b,s,c);
  initial begin
  a=1'b0;
  b=1'b0;
  end
  initial
    begin 
      #20 a=0;b=0;
      #20 a=0;b=1;
      #20 a=1;b=0;
      #20 a=1;b=1;
    end
  initial begin 
    $monitor("sum is %b and Carry is %b",s,c);
  end
  initial begin 
    $dumpfile("tb.vcd");
    $dumpvars();
  end
endmodule

// Code your testbench here
// or browse Examples
module tb;
  reg a,b;
  wire c,s;
  HA halfadd(a,b,s,c);
  initial begin
  a=1'b0;
  b=1'b0;
  end
  initial
    begin 
      #20 a=0;b=0;
      #20 a=0;b=1;
      #20 a=1;b=0;
      #20 a=1;b=1;
    end
  initial begin 
    $monitor("sum is %b and Carry is %b",s,c);
  end
  initial begin 
    $dumpfile("tb.vcd");
    $dumpvars();
  end
endmodule
