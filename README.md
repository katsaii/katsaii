```prolog
% pairs:    [-katsaii,k-atsaii,ka-tsaii,kat-saii,kats-aii,katsa-ii,katsai-i,katsaii-]
% prefixes: [,k,ka,kat,kats,katsa,katsai,katsaii]
% suffixes: [katsaii,atsaii,tsaii,saii,aii,ii,i,]
```

<p align="center">
  <img width="40%" src="https://www.katsaii.com/image/works/fire.png" />
</p>

```prolog
name("katsaii").

?-
  name(Name),
  findall(Prefix-Suffix, string_concat(Prefix, Suffix, Name), Pairs),
  pairs_keys_values(Pairs, Prefixes, Suffixes),

  write("pairs:    "), write(Pairs), nl,
  write("prefixes: "), write(Prefixes), nl,
  write("suffixes: "), write(Suffixes).
```
