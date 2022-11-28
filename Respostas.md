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
