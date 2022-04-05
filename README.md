# NuxiiGit

NuxiiGit contains the source code to "Kat," a command-line application that periodically produces [open-source projects](https://github.com/NuxiiGit?tab=repositories) and [art works](https://nuxiigit.github.io/content/works). 

## Examples

Creating a canonical instance of Kat in Haskell

```hs
{-# LANGUAGE TypeOperators #-}

import Data.List (intercalate)

-- |Represents instances of Kat.
data (🙀)
    = Katsaii
    | Nuxii
    deriving (Show)

main = putStrLn $ let katsaii = show Katsaii
                      nuxii   = show Nuxii
                      in intercalate " ✨ " ["Kat is either", katsaii, "or", nuxii, ""]
```
