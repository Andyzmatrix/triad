# triad
A = float(input ('Enter Velocity A Radians/ unit of time_'))       #Rotational velocity of Vector A in Radians/unit of time
E = float(input ('Enter Length A unit length_'))                   #Length of vector A
print ('---------------------------------------------')
B = float(input ('Enter Velocity B Radians/ unit length_'))        ##Rotational velocity of Vector B in Radians/unit of time
D = float(input ('Enter Length B unit length_'))                   #Length of vector B
print('----------------------------------------------')
C = float(input ('Enter time T units of time, sec. or minutes_'))   #Desired time at which the observation occours
O = A*C            # angle vector A in radians makes with the x-axis
P = B*C            # angle vector B in radians makes with the x-ax
import math
print ('angle vector A in radians makes with the x-axis',O,'radians')
print ('angle vector B in radians makes with the x-axis',P,'radians')
G = math.pow(E,2)       # squares the length of vector A
print('O Radians in Degrees:',math.degrees(O),'degrees')
print('P Radians in Degrees:',math.degrees(P),'degrees')
O1 = math.cos(O)
O4 = math.sin(O)
O5 = math.atan2(O4,O1) 
O2 = math.acos(O1)
O3 = math.degrees(O5)
print('cos of angle of vector A is_',O1)
print('angle of vector A is_',O3,'degrees')
P1 = math.cos(P)
P4 = math.sin(P)
P5 = math.atan2(P4, P1) 
P2 = math.acos(P1)
P3 = math.degrees(P5)
print('cos of angle of vector B is_',P1)
print('angle of vector B is_',P3,'degrees') 
H = E*D             
I = math.cos(O-P)
J = math.pow(D,2)
K = G*A ; L1=A+B
L = I*H*L1
M = J*B
S = K+L+M
F = G+(2*H*I)+J
Y = S/F
print ('The angular velocity is:_',Y)
N = E*math.cos(O)
Q = D*math.cos(P)
R = N+Q
T = E*math.sin(O)
U = D*math.sin(P)
V = T+U
V1 = math.pow(V,2);R2 = math.pow(R,2)
W = math.pow(V1+R2,1/2)
math.hypot(R,V)
print ('hypot (',math.hypot(R,V),')')
E1=E*25      #multiplier of 25 for the number of pixels in vector A
D1=D*25      #multiplier of 25 for the number of pixels in vector B
import turtle
turtle.sety(0)
turtle.setx(0)
print (' turtle Angle Vector A at :_',math.degrees(O3),'degrees')
turtle.left(math.degrees(O))
turtle.forward(E1)      #Creates vector A at length of vector A
turtle.back(E1)
turtle.right(math.degrees(O))
print (' turtle Angle Vector B at :_',math.degrees(P3),'degrees')
turtle.left(math.degrees(P))
turtle.forward(D1)
turtle.home
print ('The length of the resultant vector is_:',W)
X = Y*W
print ('The tangential velocity is_',X)

