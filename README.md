# cbhsprojectgraduation

## Build

```hugo -F -d docs```

```parallel -eta cwebp -q 85 -m 6 {} -o {}.webp ::: *.JPG```

```find | egrep '*.webp' > files.txt```

## Serve

```hugo -F serve```
