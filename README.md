# pandasquad
termux banner
// C++ program to implement a queue using an array

#include <bits/stdc++.h>

using namespace std;

 

struct Queue {

    int front, rear, capacity;

    int* queue;

    Queue(int c)

    {

        front = rear = 0;

        capacity = c;

        queue = new int;

    }

 

    ~Queue() { delete[] queue; }

 

    // function to insert an element

    // at the rear of the queue

    void queueEnqueue(int data)

    {

        // check queue is full or not

        if (capacity == rear) {
