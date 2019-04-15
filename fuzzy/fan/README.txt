%fan fuzzy uses ../membership/fan json data
%and K is the plant model dc gain

u(k) = fuzzy(e(k), de(k)); %no model
u(k) = (r(k)/K - 50) + fuzzy(e(k), de(k)); %with model

Gz =
 
    0.07751 z^-1 + 0.1716 z^-2
  ------------------------------
  1 - 0.8539 z^-1 - 0.02473 z^-2
 
Sample time: 0.1 seconds
Discrete-time transfer function.