# Crackme Reverse Engineering Challenge

**Hinweis:**
Da ich aktuell keine Möglichkeit habe, das Programm auf einem Server laufen zu lassen, liegt die Flag-Datei (`flag`) direkt im Repository bei.
Der eigentliche Spaß und die Herausforderung bestehen darin, die Flag nicht einfach zu lesen, sondern sie durch das Ausnutzen einer Schwachstelle im Crackme-Programm zu erhalten!
Viel Erfolg beim Exploiten!

**Note:**
Since I currently do not have the possibility to run the program on a server, the flag file (`flag`) is included directly in the repository.
The real fun and challenge is not simply reading the flag, but obtaining it by exploiting a vulnerability in the crackme binary!
Good luck exploiting!

## Overview

Welcome to the crackme reverse engineering challenge! Your objective is simple:

> **Analyze the provided binary and discover the flag.**

This challenge is designed to test your skills in binary analysis, vulnerability discovery, and exploitation. The flag will be printed by the binary upon successful exploitation.

## Binary Information

- **File:** `crackme`
- **Architecture:** x86-64 (64-bit)
- **Platform:** Linux (ELF, dynamically linked)
- **Tested on:** Ubuntu 22.04 (amd64)

## Getting Started

Download or clone the repository and make the binary executable:

```bash
chmod +x crackme
./crackme
```


---

## Recommended Tools

You may find the following tools useful:

- **Disassemblers:**
	- [objdump](https://man7.org/linux/man-pages/man1/objdump.1.html)
	- [radare2](https://rada.re/n/)
	- [Ghidra](https://ghidra-sre.org/)
	- [IDA Pro](https://hex-rays.com/ida-pro/)
- **Debuggers:**
	- [gdb](https://www.gnu.org/software/gdb/)
	- [pwndbg](https://github.com/pwndbg/pwndbg)
- **Other:**
	- [strings](https://man7.org/linux/man-pages/man1/strings.1.html)
	- [xxd](https://man7.org/linux/man-pages/man1/xxd.1.html)
	- [Python](https://www.python.org/) (for scripting exploits)

## Running on macOS or Windows

The binary is for Linux x86-64. On macOS or Windows, use Docker to run it:

```bash
docker run --rm -i --platform linux/amd64 -v "$(pwd)":/work -w /work gcc:latest ./crackme
```

## Challenge Notes

- The binary prints the flag if you exploit it successfully.
- No source code is provided—reverse engineering is required.
- All necessary information is contained in the binary itself.

## License

This challenge is provided for educational and research purposes only.

---

Good luck and happy hacking!
