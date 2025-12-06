# How I Jacked Into Pwn: A Short Roadmap for New Chooms

I’m not some legendary console cowboy, choom. I’m just a runner who got curious about how machines break, and kept following that neon trail until things started making sense.  
Here’s the path I took. It’s not perfect, but it works, and it might give you a head start on your own pwn journey.

## 1. Learn the Metal Before You Bend It
Before trying to exploit anything, I had to understand how programs actually live:
- Memory layout: stack, heap, registers  
- How a program runs  
- How compilers translate code  
- Threads, processes, and basic syscalls  

I also learned how to inspect binaries and understand what they’re doing while running.

**Resources I used:**
- YouTube videos on assembly basics  
- Writing tiny assembly programs and debugging them with `gdb`
- General OS/process/thread/syscall explanations  
- My own **pwn_presentation.pdf** (ENGINEERS SPARK ISETCOM Club) for memory mapping and fundamentals https://www.canva.com/design/DAG1EJyVf8w/HG9XiA7Mwwda3WCDv-_RTg/edit?utm_content=DAG1EJyVf8w&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton
**Tools:** `gdb`, `objdump`, `strace`, `ltrace`

## 2. C Is Your New Chrome Spine
I’m not a master, but learning C helped me understand how bugs are born.  
Stuff I focused on:
- Pointers  
- Buffer overflows  
- Format strings  
- Basic type confusion  

The best practice was writing my own small, buggy programs and breaking them.

**Resources I used:**
- Standard C tutorials  
- Random C crash-course videos  
- Debugging C programs with `gdb`

## 3. Assembly: The Low-Level Street Language
Assembly isn’t something I fully mastered, but knowing enough to read what the CPU is doing made exploit dev way clearer.

I learned:
- x86 and x64 basics  
- Registers and calling conventions  
- How instructions map to control flow  
- How the stack behaves during function calls

**Resources I used:**
- YouTube assembly playlists  
- My own pwn presentation for calling conventions & virtual memory  
- Writing tiny assembly snippets then stepping through them in `gdb`

## 4. Classic Vulns: First Real Runs
This is where pwn actually clicked for me. I’m still learning, but getting these basics down helped a lot:
- Simple stack overflows  
- Ret2win  
- Ret2libc  
- Ret2shellcode  
- GOT/PLT hijacking  
- ROP chains

**Resources I used:**
- **pwn.college – Return Oriented Programming path**  
- My own notes and experiments  
- Public CTF writeups

## 5. Full-Stack Exploit Dev
I’m not claiming expertise, choom. Just enough skill to not embarrass myself too often.  
This stage was about understanding protections and how to get around them:
- ASLR  
- PIE  
- NX  
- Stack canaries  
- Intro to heap exploitation  

**Resources I used:**
- DreamHack CTF platform  
- HackTheBox pwn challenges  
- More pwn.college labs  
- Random writeups that explain their steps clearly

## 6. Write, Break, Repeat
Nothing boosted my skills more than this loop:
- Write tiny programs  
- Introduce bugs  
- Try to exploit them  
- Repeat

Even now, I’m learning new tricks by breaking my own code.

## 7. Community: The Alleyway Taverns
I learned a lot from people smarter than me:
- Discord groups  
- CTF writeups  
- HackTheBox forums  
- CTFtime challenge archives  

Not for validation, but because other runners leave behind preem clues.

---

# Short Recap Table

| Stage | Goal | Resources Used |
|-------|------|----------------|
| 1 | Basics | YouTube assembly, pwn_presentation.pdf, gdb tools, OS basics |
| 2 | C | C tutorials, debugging exercises |
| 3 | Assembly | YouTube guides, writing & debugging tiny asm |
| 4 | Classic vulns | pwn.college ROP path |
| 5 | Protections | DreamHack CTF, HTB pwn tracks |
| 6 | Practice | Writing and breaking my own code |

---

# Final Words
I’m still learning, still messing up, still improving.  
Pwn isn’t a skill you magically “master.” It’s a path you walk, one crash, breakpoint, and exploit at a time.  
If you keep pushing forward, the binaries eventually start making sense, and every challenge becomes a new opportunity to sharpen your edge.

