# Circuitos-Digitais1
<br>

##Exercício 1:
=

<br>
module mux2x1(a,b,sel,y);
<br>
  intput a,b,sel;
  <br>
  output y;
  <br>

  assign y = sel ? a:b;
  <br>

endmodule
<br>
module circ_mux(e0,e1,e2,e3,s0,s1,y);
<br>
input e0,e1,e2,e3,s0,s1;
<br>
output y;
<br>

wire e01, e23;
<br>

mux2x1 m1 (e0,e1,s0,e01);
<br>
mux2x1 m2 (e2,e3,s0,e23);
<br>
mux2x1 m3 (e01,e23,s1,y);
<br>
endmodule

##Exercício 2:
=
<br>
module soma4x1(a,b,s);
<br>
  input [3:0] a,b;
  <br>
  output [3:0] s;
  <br>

  assign s = (a + b);
  <br>

endmodule

module subtracao4x1(a,b,s);
<br>
  input [3:0] a,b;
  <br>
  output [3:0] s;
  <br>

  assign s = (a - b);
  <br>

endmodule

module and4x1(a,b,s);
<br>
  input [3:0] a,b;
  <br>
  output [3:0] s;
  <br>

  assign s = (a & b);
  <br>

endmodule

module or4x1(a,b,s);
<br>
  input [3:0] a,b;
  <br>
  output [3:0] s;
  <br>

  assign s = (a | b);
  <br>

endmodule

module exor4x1(a,b,s);
<br>
  input [3:0] a,b;
  <br>
  output [3:0] s;
  <br>

  assign s = (a ~| b);
  <br>

endmodule

module circ(op,a,dado,s,sel);
<br>
input [3:0] a,dado;
<br>
input [2:0] op;
<br>
output [3:0] s;
<br>


endmodule
