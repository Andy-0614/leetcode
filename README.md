# leetcode

C++ LeetCode solutions, managed with [leetgo](https://github.com/j178/leetgo).

Each problem lives in `cpp/<id>.<slug>/` with `solution.cpp`, `question.md` and `testcases.txt`.

## Workflow

```powershell
lc-login             # once, and again when cookies expire: paste LeetCode cookies from Brave
leetgo pick 1        # generate cpp/0001.two-sum/ and open it in VSCode
leetgo test last -L  # run testcases locally with g++
lcs                  # leetgo submit last; on Accepted, git commit + push
```

`lc-login` and `lcs` are PowerShell functions from [DotFile](https://github.com/Andy-0614/DotFile).
In VSCode: `Ctrl+Alt+P` = pick, `Ctrl+Alt+S` = submit + push; `Tasks: Run Task` also lists `leetgo login` and `leetgo test last`.

## Cookies

leetgo cannot read Chromium (Brave) cookies on Windows, so `lc-login` stores
`LEETCODE_SESSION`, `csrftoken` and `cf_clearance` as user environment variables.
Get them from Brave: log in to leetcode.com, F12 -> Application -> Cookies -> https://leetcode.com.
