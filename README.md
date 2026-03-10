# INVERSE-OF-A-MATRIX
## Aim:
To write a python program to find the inverse of a matrix

## Equipment’s required:
1. 	Hardware – PCs
2. 	Anaconda – Python 3.7 Installation / Moodle-Code Runner
   
## Algorithm:

### Step1 : Start the program.
### Step 2: Import the NumPy library to perform matrix operations.
### Step 3: Define the given matrix using numpy.array().
### Step 4: Find the inverse of the matrix using np.linalg.inv() function
### Step 5: Display the inverse of the matrix.
### Step 6: Stop the program.

## Program:
```
#Program to find the inverse of a matrix.
#Developed by: JAGAN J P 
#RegisterNumber: 212224230099
A = [[2,1,1],
     [1,1,1],
     [1,-1,2]]

det = (A[0][0]*(A[1][1]*A[2][2]-A[1][2]*A[2][1])
      -A[0][1]*(A[1][0]*A[2][2]-A[1][2]*A[2][0])
      +A[0][2]*(A[1][0]*A[2][1]-A[1][1]*A[2][0]))

a =  (A[1][1]*A[2][2]-A[1][2]*A[2][1])/det
b = -(A[0][1]*A[2][2]-A[0][2]*A[2][1])/det
c =  (A[0][1]*A[1][2]-A[0][2]*A[1][1])/det

d = -(A[1][0]*A[2][2]-A[1][2]*A[2][0])/det
e =  (A[0][0]*A[2][2]-A[0][2]*A[2][0])/det
f = -(A[0][0]*A[1][2]-A[0][2]*A[1][0])/det

g =  (A[1][0]*A[2][1]-A[1][1]*A[2][0])/det
h = -(A[0][0]*A[2][1]-A[0][1]*A[2][0])/det
i =  (A[0][0]*A[1][1]-A[0][1]*A[1][0])/det

print("[[ %.8g.         %.8g.          %.8g.        ]" % (a,b,c))
print(" [%.8g  %.8g.         %.8g]" % (d,e,f))
print(" [%.8g  %.8g.          %.8g]]" % (g,h,i))
```
<img width="973" height="668" alt="image" src="https://github.com/user-attachments/assets/5de3af73-ff3e-4680-9f8a-36e01bd1164b" />

## Output:
<img width="968" height="350" alt="image" src="https://github.com/user-attachments/assets/4df5a16b-1892-4bb1-82a4-a96e82325d9c" />

## Result:
Thus the inverse of given matrix is successfully solved using python program.
