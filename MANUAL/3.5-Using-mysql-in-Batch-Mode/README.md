### 3.5 Using mysql in Batch Mode

<strong>
You can also run mysql in batch mode. To do this, put the statements you want to run in a file, then tell mysql to read its input from the file:
</strong>

```
shell> mysql < batch-file
```


- If you have a query that produces a lot of output, you can run the output through a pager rather than watching it scroll off the top of your screen:
    ```
    shell> mysql < batch-file | more
    ```
- You can catch the output in a file for further processing:
    ```
    shell> mysql < batch-file > mysql.out
    ```