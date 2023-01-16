```prolog
% pairs:    [-katsaii,k-atsaii,ka-tsaii,kat-saii,kats-aii,katsa-ii,katsai-i,katsaii-]
% prefixes: [,k,ka,kat,kats,katsa,katsai,katsaii]
% suffixes: [katsaii,atsaii,tsaii,saii,aii,ii,i,]
```

<p align="center">
  <img width="40%" style="min-width : 300px" src="./img.png" />
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

<p align="center">
  <code><a href="https://tio.run/##XY5NCoMwEIX3nmJwpRA9gJveoAg9gAw2ymAaJRNre/p0TGORZpGf9773JoubzTxWvFEIFh@6yCf0jER5WWfZpcoAonyVrVTyGsje0ZiidXqgV3VbBzkUsHdkx66fbY8@mQoO95uGFslxbFn2WzfpN3dPNKvmInqCxKTmI6t3XgKbIy@fi7kGZOXS9xVTK1ijTmDqac5g0v5ZTpPO7G96HcIH" title="Prolog (SWI) – Try It Online">Try it online!</a></code>
</p>
