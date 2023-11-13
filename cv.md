## Nikitina Darya

<img src="https://github.com/Dakvalion/rsschool-cv/assets/105875517/ade00dfc-77c3-416e-81af-6db68d186271" width="320px" align='right'>

### Contacts:

---

- Telegram: @Dakvalion
- Email: dnikitina26@gmail.com

---

### About Me

---

I am a friendly and open person, and I also treat the tasks assigned to me responsibly. Nowadays I'm on my way to become a frontend developer and I'll do my best to achive my goals

### Skills:

---

#### Programming languages:

- JavaScript
- TypeScript
- C#
- Python

#### Frameworks:

- django

#### Methodologies:

- OOP
  ***

### English: B1

---

### Code Example:

```C#
 public static int FindPivot(int N_op, Queue numbers, int minIndex, int maxIndex)
{
    N_op += 4;
    int pivot = minIndex -1;
    int temp1 = 0;
    int temp2 = 0;
    N_op += 3;
    for (int i = minIndex; i < maxIndex; i++)
    {
        N_op += 4;
        if (numbers.Get(i) < numbers.Get(maxIndex))
        {
            N_op+=3;
            pivot++; //+1
            temp1 = numbers.Get(pivot);
            temp2 = numbers.Get(i);
            numbers.Set(i, temp1);
            numbers.Set(pivot, temp2);

        }
    }

    N_op += 3;
    pivot++;
    temp1 = numbers.Get(pivot);
    temp2 = numbers.Get(maxIndex);
    numbers.Set(maxIndex, temp1);
    numbers.Set(pivot, temp2);

    return pivot;
}

public static Queue QuickSort(int N_op, Queue numbers, int minIndex, int maxIndex)
{
    N_op++;
    if (minIndex >= maxIndex)
    {
        return numbers;
    }

    N_op++;
    int pivot = FindPivot( N_op, numbers, minIndex, maxIndex);
    QuickSort(N_op, numbers, minIndex, pivot - 1);
    QuickSort(N_op,numbers, pivot + 1, maxIndex);

    return numbers;
}
```
