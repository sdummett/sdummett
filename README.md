```asm
		global		_start

		section		.text
_start:
		mov			rax, 4
		mov			rbx, 1
		mov			rcx, msg1
		mov			rdx, 0x14
		int			0x80
		mov			rax, 4
		mov			rbx, 1
		mov			rcx, msg2
		mov			rdx, 0x2b
		int			0x80
		mov			rax, 1
		mov			rbx, 42
		int			0x80

		section   .data
msg1:	db	"Hi there! I'm Stone", 0x0a
msg2:	db	"I'm a computer science student at 42 Paris."
```
