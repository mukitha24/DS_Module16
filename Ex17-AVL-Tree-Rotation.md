# Ex.No:4(B) AVL Tree – Rotation
## DATE:29-03-25
## AIM:
To write a C function to perform right rotation in an AVL Tree.

## Algorithm
1. Start
2. Set y to the left child of x.
3. Set the left child of x to be the right child of y.
4. Set the right child of y to be x.
5. Update the height of x and y.
6. Return y as the new root after rotation.
7. End   
## Program:
```
/*
Program to perform right rotation in AVL Tree
Developed by:MUKITHA V  
RegisterNumber:212223040119  
*/
```
```
/*
typedefstruct node
{
int data;
struct node*left,*right;
int ht;
}node;
node *insert(node *,int);
//node*Delete(node*,int);
void preorder(node*);
//void inorder(node*);
int height( node *);
node*rotateright(node*);
node *rotateleft(node *);
node *RR(node *);
node *LL(node *);
node *LR(node *);
node *RL(node*);
*/
node *rotateright(node*x)
{
node *y;
y=x->left;
x->left=y->right;
y->right=x;
x->ht=height(x);
y->ht=height(y);
return(y);
}
```
## Output:
![Screenshot 2025-04-26 200100](https://github.com/user-attachments/assets/c6d4569c-5d1b-4e62-88a5-340ec93e9903)

## Result:
Thus, the function to perform right rotation in an AVL Tree is implemented successfully.
