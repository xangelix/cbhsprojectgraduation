# cbhsprojectgraduation

## Build

```hugo -F -d docs```

```parallel -eta cwebp -q 85 -m 6 {} -o {}.webp ::: *.JPG```

```find . -printf "%T@ %Tc %p\n" | sort -n | egrep '*.webp' | cut -c57- | sed -e 's;^;- image : ;' > files.txt```

## Serve

```hugo -F serve```
