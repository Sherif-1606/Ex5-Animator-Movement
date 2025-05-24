# Ex5-Animator-Movement

## Aim :

To develop a animator movement for a player using unity.

## Algorithm :

## Step 1 : 

Import necessary models.

## Step 2 : 

 Right-click -> Create -> Animator Controller.

## Step 3 : 

Open Animator window, define states (Idle, Run, Jump, etc.).

## Step 4 : 

Use keyframes or Unity's Animation tools to animate transitions between states.

## Step 5 : 

Drag Animator Controller to the GameObject in the Inspector.

## Program :

### DEVELOPED BY : A.Abdul Rehman Sheriff 
### REG NO : 212222220002

## PlayerController:


```
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class Movement : MonoBehaviour
{
    public Animator animator;
    public float InputX;
    public float InputY;
    // Start is called before the first frame update
    void Start()
    {
        animator = this.gameObject.GetComponent <Animator>();
    }

    // Update is called once per frame
    void Update()
    {
        InputX = Input.GetAxis("Horizontal");
        animator.SetFloat("InputX", InputX);
        InputY = Input.GetAxis("Vertical");
        animator.SetFloat("InputY", InputY);
    }
}


```
## Output :
![AR OUTPUT](https://github.com/user-attachments/assets/7e4786a6-c970-4a04-b7c0-ee2b218aa903)
![AR OUTPUT 2](https://github.com/user-attachments/assets/ec09fee2-06a5-4dff-8a34-e2334aa262da)
![AR OUTPUT 3](https://github.com/user-attachments/assets/95b12b66-a37c-49ce-8d2c-a02dc095921d)



## Result :

Thus, An animator movement for a player using unity is developed successfully.
