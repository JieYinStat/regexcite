# side-by-side diffs work

    Code
      waldo::compare(c(
        "X", letters), c(
        letters, "X"))
    Output
          old | new    
      [1] "X" -        
      [2] "a" | "a" [1]
      [3] "b" | "b" [2]
      [4] "c" | "c" [3]
      
           old | new     
      [25] "x" | "x" [24]
      [26] "y" | "y" [25]
      [27] "z" | "z" [26]
               - "X" [27]

---

    Code
      str_dup(1:2, 1:3)
    Condition
      [1m[33mError[39m in `str_dup()`:[22m
      [33m![39m could not find function "str_dup"

