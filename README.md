int b= sizeof(arr)/sizeof(int)
 int i, j, min, temp;
   for (i = 0; i < b - 1; i++) {
      min = i;
      for (j = i + 1; j < b; j++)
      if (a[j] < a[min])
      min = j;
      temp = a[i];
      a[i] = a[min];
      a[min] = temp;
   }
