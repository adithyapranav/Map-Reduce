# DS-Project

## To run code

1. Open 4 terminals
2. On Terminal 1

```
cd main
go run wc.go master localhost:7777 data/pg*.txt
```

3. On Terminal 2

```
cd main
go run wc.go worker localhost:7777 localhost:7778 &
```

4. On Terminal 3

```
cd main
go run wc.go worker localhost:7777 localhost:7779 &
```

5. On Terminal 4

```
cd main
go run wc.go worker localhost:7777 localhost:7780 &
```

## Input

All the files in `data` directory

## Output

`mrtmp.wcseq`
