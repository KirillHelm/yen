# YEN Project

This project helps to manage shell tools in an organized manner.

> These tools are called **modules** in the terms of this project.

The project provides access to all these tools via a single entry point.
This helps to configure, deploy and navigate over them.

## Post-clone steps

1. Set the git message template:
`git config --local commit.template .gitmessage`
2. Set GPG signature:
`git config --local commit.gpgsign true`
`git config --local user.signingkey XXXXXXXXXX`

> Usefull links:
> [Git Tools - Signing Your Work](https://git-scm.com/book/en/v2/Git-Tools-Signing-Your-Work)
> [GPG Keys Cheatsheet](https://rtcamp.com/tutorials/linux/gpg-keys/)

## Build

### Docker

1. Build docker image:
`docker build -t yen-builder .`
2. Create & run a container with mounted sources:
`docker run -it --rm -v $(pwd):/host yen-builder`
3. Configure the project:
`mkdir /host/build && cmake -S /host -B /host/build`
4. Build the project:
`cmake --build /host/build`

### Host (Unix)

The following dependencies, should be installed:

| Name | Version | Comment |
| :- | :-: | :- |
| cmake | 3.22 | |
| gcc | 11.2 | Or compiler of your choice |
| clang | 13.1 | Or compiler of your choice |

1. Configure the project:
`mkdir build && cmake -S . -B build/`
2. Build the project:
`cmake --build build`

