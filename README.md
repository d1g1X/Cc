using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class Cc : MonoBehaviour
{
    int health = 5;
    int lvl = 1;
    float speed = 1.2f;
    // Start is called before the first frame update
    void Start()
    {
        health += lvl;
        print("Здоровье:" + health);
    }

    // Update is called once per frame
    void Update()
    {
        Vector3 pos = transform.position;
        pos.z += speed * Time.deltaTime;
        transform.position = pos;
    }
}
