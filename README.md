# ethtps.utils

## Global utils and other useful stuff for ethtps (but not limited to)

I don't know who will use this, but here are some things that helped me during development:

1. Regexes (or "reg*i*?") I use in VSCode:

    1. `(.")(\^)\d(.*)(.")` matches `^1.2.3.4`

    2. `^(.*)IEnumerable<(.*)>(.*)\n(.*)\n(.*)Empty<>`, `\tpublic IEnumerable<$2> $3\n\t{\n\t\treturn Enumerable.Empty<$2>` replaces `public IEnumerable<INavigation> GetDeclaredNavigations\n\t{\n\t\tpublic IEnumerable<>}` with `public IEnumerable<INavigation> GetDeclaredNavigations\n\t{\n\t\tpublic IEnumerable<INavigation>`. I use this in `EmptyDbSet.cs` (in the [backend](https://github.com/ethtps/ethtps.backend/tree/main/ETHTPS.Configuration/Database/EmptyDBSet.cs))
