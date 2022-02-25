# Operating Systems Capstone 2022

This repository is homework submission for students

## Submission details

- GitHub account name: xdavidwu
- Student ID: 0716022
- Your name: 吳秉澔

### Build instructions

Requires meson, ninja/samurai, aarch64 GCC toolchain

Cross compiling target definition at arch/aarch64/cross.ini assumes toolchain
available under $PATH with triplet prefix `aarch64-none-elf-`, create another
definition base on it if that does not suit you.

```
cd src
meson build --cross-file arch/aarch64/cross.ini
ninja -C build
# kernel8.img will be at (src/)build/kernel8.img
```

## How to submit homework

1. Fork [this repository](https://github.com/oscapstone/osc2022) on GitHub 
    ![](images/fork_button.png)
2. Write down following info in your `README.md`
    - GitHub account name
    - Student ID
    - Your name
3. Design and implement your kernel in forked repository
4. Create a GitHub pull request
    - Choose `oscapstone/osc2022` as base repository and `{your student ID}` as base branch
    - Choose branch in your forked repository as compare branch
    - Name it with student ID and which lab e.g. `0856085 lab0`
    ![](images/pull_request.png)
5. We will accept pull request when lab due date

repeat 3-5 to submit later homework/lab.

## Happy Coding ~
