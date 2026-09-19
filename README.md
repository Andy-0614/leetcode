# leetcode

C++ LeetCode solutions, managed with [leetgo](https://github.com/j178/leetgo).

Each problem lives in `cpp/<id>.<slug>/` with `solution.cpp`, `question.md` and `testcases.txt`.

## Workflow

```powershell
leetgo pick 1        # generate cpp/0001.two-sum/ and open it in VSCode
leetgo test last -L  # run testcases locally with g++
lcs                  # leetgo submit last; on Accepted, git commit + push
```

`lcs` is a PowerShell function from [DotFile](https://github.com/Andy-0614/DotFile); in VSCode press `Ctrl+Alt+S`.
