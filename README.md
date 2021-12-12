# hacker
Let's learn about list comprehensions! You are given three integers x,y and z representing the dimensions of a cuboid along with an integer . Print a list of all possible coordinates given by (i,j,k) on a 3D grid where the sum of i+j+k  is not equal to n . Here,0<=i<=x,0<=j<=y,0<=k<=z . Please use list comprehensions rather than multiple loops, as a learning exercise.

Example
x=1
y=1
z=1

All permutations of [i,j,k] are:
[0,0,0],[0,0,1],[0,1,0],[1,0,0],[1,1,1]



if __name__ == '__main__':
    x = int(raw_input())
    y = int(raw_input())
    z = int(raw_input())
    n = int(raw_input())
    
  
x, y, z, n = (int(input()) for _ in range(4))
print[[x,y,z] for x in range(0,x+1) for y in range(0,y+1) for z in range(0,z+1) if( x + y + z )!= n ]
