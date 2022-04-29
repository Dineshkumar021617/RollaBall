# RollaBall

## Aim:
To Roll a Ball using C# program in unity .

## Algorithm:

## Program:
```python
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class Object1 : MonoBehaviour
{
    // Start is called before the first frame update
    public float xmove = 7.0f;
    public float zmove = 5.0f;
    public float ymove = 150.0f;
    void Start()
    {
        
    }

    // Update is called once per frame
    void Update()
    {
        float x = 0.0f;
        if(Input.GetKey(KeyCode.UpArrow))
        {
            x += xmove;
        }
        if(Input.GetKey(KeyCode.DownArrow))
        {
            x -= xmove;
        }
        float z = 0.0f;
        if(Input.GetKey(KeyCode.RightArrow))
        {
            z -= zmove;
        }
        if(Input.GetKey(KeyCode.LeftArrow))
        {
            z += zmove;
        }
        float y = 0.0f;
        if(Input.GetKeyDown(KeyCode.Space))
        {
            y = ymove;
        }
        GetComponent<Rigidbody>().AddForce(x, y, z);
    }
}
```

## Output:
![Screenshot (78)](https://user-images.githubusercontent.com/75234807/165896244-94ada6c5-63da-4597-b95a-cc6b911d9a08.png)

## Result:
