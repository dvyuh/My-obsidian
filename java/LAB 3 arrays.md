
taking input of array
```
        // Read the size of the array
        if (!scanner.hasNextInt()) {
            return;
        }
        int n = scanner.nextInt();
        
        int[] arr = new int[n];
        
        // Read array elements
        for (int i = 0; i < n; i++) {
            arr[i] = scanner.nextInt();
        }
```

