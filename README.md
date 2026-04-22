# diarynotes

Utility for taking notes using markdown and git

The `./today` script creates a new .md file you can use to take notes for your current day's work.

When you run the `./today` script it will create a folder for the current year, within the year folder it will create a folder for the current month. Within the month folder it will create a .MD file with the following name format `day-month-year.md`. As an example if you run the script on 5 March 2025 your folder structure will look like so:
- `2025`
    - `March`
        - `05-03-2025.md`

Running the script on subsequent days would cause the following folder structure to exist:

- `2025`
    - `March`
        - `05-03-2025.md`
        - `06-03-2025.md`
        - `07-03-2025.md`
        - `08-03-2025.md`
        - etc
     
## Generating a file for a different day than the current date

If you need to generate a file for a different date than the current date, you can pass a negative or a positve offset to the script like so:

```bash
# passing -1 will generate a file for the previous day
./today -1
```

```bash
# passing +1 will generate a file for the next day
./today +1
```


## How to use this script.
Create a new repo and copy the `__template__.md` and the `./today` script.

You can modify the `__template__.md` file to be in a different format.
