# serverless-file-test

# Case 1

Check `serverless.yml` file:
In the first case, line 8 is uncommented `package: ${file(./dependences.yml)}`
In this case we use the file import

- run `sls print` you will see the package corretly
- run `sls package`
    - Unzip the file
    - You will see the `file-to-exclude.md` file there

# Case 2

Check `serverless.yml` file:
You should comment line 8
You should uncomment lines 11, 12 and 13

In this case we put everything inside the `serverless.yml` file

- run `sls print` you will see the package corretly
- run `sls package`
    - Unzip the file
    - You will NOT see the `file-to-exclude.md` file there