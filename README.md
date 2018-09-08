# PB16110766 陆万航 编译原理h HW1
## 不同参数下编译输出的结果
* 实验使用的源代码为source.c，为一个简单的冒泡排序算法，对应的shell文件为comp.sh
* 执行时，cd到对应目录下后，执行命令 /bin/sh comp.sh
* 在编译中加入不同的参数，从而得到不同的编译结果：
### 利用-E编译生成结果
执行命令gcc -E source.c -o Egcc，即可将预处理的结果写入到文档Egcc中，Egcc中的内容如下所示：
```
# 1 "source.c"
# 1 "<built-in>"
# 1 "<command-line>"
# 31 "<command-line>"
# 1 "/usr/include/stdc-predef.h" 1 3 4
# 32 "<command-line>" 2
# 1 "source.c"
# 1 "/usr/include/stdio.h" 1 3 4
# 27 "/usr/include/stdio.h" 3 4
# 1 "/usr/include/x86_64-linux-gnu/bits/libc-header-start.h" 1 3 4
# 33 "/usr/include/x86_64-linux-gnu/bits/libc-header-start.h" 3 4
# 1 "/usr/include/features.h" 1 3 4
# 424 "/usr/include/features.h" 3 4
# 1 "/usr/include/x86_64-linux-gnu/sys/cdefs.h" 1 3 4
# 427 "/usr/include/x86_64-linux-gnu/sys/cdefs.h" 3 4
# 1 "/usr/include/x86_64-linux-gnu/bits/wordsize.h" 1 3 4
# 428 "/usr/include/x86_64-linux-gnu/sys/cdefs.h" 2 3 4
# 1 "/usr/include/x86_64-linux-gnu/bits/long-double.h" 1 3 4
# 429 "/usr/include/x86_64-linux-gnu/sys/cdefs.h" 2 3 4
# 425 "/usr/include/features.h" 2 3 4
# 448 "/usr/include/features.h" 3 4
# 1 "/usr/include/x86_64-linux-gnu/gnu/stubs.h" 1 3 4
# 10 "/usr/include/x86_64-linux-gnu/gnu/stubs.h" 3 4
# 1 "/usr/include/x86_64-linux-gnu/gnu/stubs-64.h" 1 3 4
# 11 "/usr/include/x86_64-linux-gnu/gnu/stubs.h" 2 3 4
# 449 "/usr/include/features.h" 2 3 4
# 34 "/usr/include/x86_64-linux-gnu/bits/libc-header-start.h" 2 3 4
# 28 "/usr/include/stdio.h" 2 3 4





# 1 "/usr/lib/gcc/x86_64-linux-gnu/7/include/stddef.h" 1 3 4
# 216 "/usr/lib/gcc/x86_64-linux-gnu/7/include/stddef.h" 3 4

# 216 "/usr/lib/gcc/x86_64-linux-gnu/7/include/stddef.h" 3 4
typedef long unsigned int size_t;
# 34 "/usr/include/stdio.h" 2 3 4

# 1 "/usr/include/x86_64-linux-gnu/bits/types.h" 1 3 4
# 27 "/usr/include/x86_64-linux-gnu/bits/types.h" 3 4
# 1 "/usr/include/x86_64-linux-gnu/bits/wordsize.h" 1 3 4
# 28 "/usr/include/x86_64-linux-gnu/bits/types.h" 2 3 4


typedef unsigned char __u_char;
typedef unsigned short int __u_short;
typedef unsigned int __u_int;
typedef unsigned long int __u_long;


typedef signed char __int8_t;
typedef unsigned char __uint8_t;
typedef signed short int __int16_t;
typedef unsigned short int __uint16_t;
typedef signed int __int32_t;
typedef unsigned int __uint32_t;

typedef signed long int __int64_t;
typedef unsigned long int __uint64_t;







typedef long int __quad_t;
typedef unsigned long int __u_quad_t;







typedef long int __intmax_t;
typedef unsigned long int __uintmax_t;
# 130 "/usr/include/x86_64-linux-gnu/bits/types.h" 3 4
# 1 "/usr/include/x86_64-linux-gnu/bits/typesizes.h" 1 3 4
# 131 "/usr/include/x86_64-linux-gnu/bits/types.h" 2 3 4


typedef unsigned long int __dev_t;
typedef unsigned int __uid_t;
typedef unsigned int __gid_t;
typedef unsigned long int __ino_t;
typedef unsigned long int __ino64_t;
typedef unsigned int __mode_t;
typedef unsigned long int __nlink_t;
typedef long int __off_t;
typedef long int __off64_t;
typedef int __pid_t;
typedef struct { int __val[2]; } __fsid_t;
typedef long int __clock_t;
typedef unsigned long int __rlim_t;
typedef unsigned long int __rlim64_t;
typedef unsigned int __id_t;
typedef long int __time_t;
typedef unsigned int __useconds_t;
typedef long int __suseconds_t;

typedef int __daddr_t;
typedef int __key_t;


typedef int __clockid_t;


typedef void * __timer_t;


typedef long int __blksize_t;




typedef long int __blkcnt_t;
typedef long int __blkcnt64_t;


typedef unsigned long int __fsblkcnt_t;
typedef unsigned long int __fsblkcnt64_t;


typedef unsigned long int __fsfilcnt_t;
typedef unsigned long int __fsfilcnt64_t;


typedef long int __fsword_t;

typedef long int __ssize_t;


typedef long int __syscall_slong_t;

typedef unsigned long int __syscall_ulong_t;



typedef __off64_t __loff_t;
typedef char *__caddr_t;


typedef long int __intptr_t;


typedef unsigned int __socklen_t;




typedef int __sig_atomic_t;
# 36 "/usr/include/stdio.h" 2 3 4
# 1 "/usr/include/x86_64-linux-gnu/bits/types/__FILE.h" 1 3 4



struct _IO_FILE;
typedef struct _IO_FILE __FILE;
# 37 "/usr/include/stdio.h" 2 3 4
# 1 "/usr/include/x86_64-linux-gnu/bits/types/FILE.h" 1 3 4



struct _IO_FILE;


typedef struct _IO_FILE FILE;
# 38 "/usr/include/stdio.h" 2 3 4



# 1 "/usr/include/x86_64-linux-gnu/bits/libio.h" 1 3 4
# 35 "/usr/include/x86_64-linux-gnu/bits/libio.h" 3 4
# 1 "/usr/include/x86_64-linux-gnu/bits/_G_config.h" 1 3 4
# 19 "/usr/include/x86_64-linux-gnu/bits/_G_config.h" 3 4
# 1 "/usr/lib/gcc/x86_64-linux-gnu/7/include/stddef.h" 1 3 4
# 20 "/usr/include/x86_64-linux-gnu/bits/_G_config.h" 2 3 4

# 1 "/usr/include/x86_64-linux-gnu/bits/types/__mbstate_t.h" 1 3 4
# 13 "/usr/include/x86_64-linux-gnu/bits/types/__mbstate_t.h" 3 4
typedef struct
{
  int __count;
  union
  {
    unsigned int __wch;
    char __wchb[4];
  } __value;
} __mbstate_t;
# 22 "/usr/include/x86_64-linux-gnu/bits/_G_config.h" 2 3 4




typedef struct
{
  __off_t __pos;
  __mbstate_t __state;
} _G_fpos_t;
typedef struct
{
  __off64_t __pos;
  __mbstate_t __state;
} _G_fpos64_t;
# 36 "/usr/include/x86_64-linux-gnu/bits/libio.h" 2 3 4
# 53 "/usr/include/x86_64-linux-gnu/bits/libio.h" 3 4
# 1 "/usr/lib/gcc/x86_64-linux-gnu/7/include/stdarg.h" 1 3 4
# 40 "/usr/lib/gcc/x86_64-linux-gnu/7/include/stdarg.h" 3 4
typedef __builtin_va_list __gnuc_va_list;
# 54 "/usr/include/x86_64-linux-gnu/bits/libio.h" 2 3 4
# 149 "/usr/include/x86_64-linux-gnu/bits/libio.h" 3 4
struct _IO_jump_t; struct _IO_FILE;




typedef void _IO_lock_t;





struct _IO_marker {
  struct _IO_marker *_next;
  struct _IO_FILE *_sbuf;



  int _pos;
# 177 "/usr/include/x86_64-linux-gnu/bits/libio.h" 3 4
};


enum __codecvt_result
{
  __codecvt_ok,
  __codecvt_partial,
  __codecvt_error,
  __codecvt_noconv
};
# 245 "/usr/include/x86_64-linux-gnu/bits/libio.h" 3 4
struct _IO_FILE {
  int _flags;




  char* _IO_read_ptr;
  char* _IO_read_end;
  char* _IO_read_base;
  char* _IO_write_base;
  char* _IO_write_ptr;
  char* _IO_write_end;
  char* _IO_buf_base;
  char* _IO_buf_end;

  char *_IO_save_base;
  char *_IO_backup_base;
  char *_IO_save_end;

  struct _IO_marker *_markers;

  struct _IO_FILE *_chain;

  int _fileno;



  int _flags2;

  __off_t _old_offset;



  unsigned short _cur_column;
  signed char _vtable_offset;
  char _shortbuf[1];



  _IO_lock_t *_lock;
# 293 "/usr/include/x86_64-linux-gnu/bits/libio.h" 3 4
  __off64_t _offset;







  void *__pad1;
  void *__pad2;
  void *__pad3;
  void *__pad4;

  size_t __pad5;
  int _mode;

  char _unused2[15 * sizeof (int) - 4 * sizeof (void *) - sizeof (size_t)];

};


typedef struct _IO_FILE _IO_FILE;


struct _IO_FILE_plus;

extern struct _IO_FILE_plus _IO_2_1_stdin_;
extern struct _IO_FILE_plus _IO_2_1_stdout_;
extern struct _IO_FILE_plus _IO_2_1_stderr_;
# 337 "/usr/include/x86_64-linux-gnu/bits/libio.h" 3 4
typedef __ssize_t __io_read_fn (void *__cookie, char *__buf, size_t __nbytes);







typedef __ssize_t __io_write_fn (void *__cookie, const char *__buf,
     size_t __n);







typedef int __io_seek_fn (void *__cookie, __off64_t *__pos, int __w);


typedef int __io_close_fn (void *__cookie);
# 389 "/usr/include/x86_64-linux-gnu/bits/libio.h" 3 4
extern int __underflow (_IO_FILE *);
extern int __uflow (_IO_FILE *);
extern int __overflow (_IO_FILE *, int);
# 433 "/usr/include/x86_64-linux-gnu/bits/libio.h" 3 4
extern int _IO_getc (_IO_FILE *__fp);
extern int _IO_putc (int __c, _IO_FILE *__fp);
extern int _IO_feof (_IO_FILE *__fp) __attribute__ ((__nothrow__ , __leaf__));
extern int _IO_ferror (_IO_FILE *__fp) __attribute__ ((__nothrow__ , __leaf__));

extern int _IO_peekc_locked (_IO_FILE *__fp);





extern void _IO_flockfile (_IO_FILE *) __attribute__ ((__nothrow__ , __leaf__));
extern void _IO_funlockfile (_IO_FILE *) __attribute__ ((__nothrow__ , __leaf__));
extern int _IO_ftrylockfile (_IO_FILE *) __attribute__ ((__nothrow__ , __leaf__));
# 462 "/usr/include/x86_64-linux-gnu/bits/libio.h" 3 4
extern int _IO_vfscanf (_IO_FILE * __restrict, const char * __restrict,
   __gnuc_va_list, int *__restrict);
extern int _IO_vfprintf (_IO_FILE *__restrict, const char *__restrict,
    __gnuc_va_list);
extern __ssize_t _IO_padn (_IO_FILE *, int, __ssize_t);
extern size_t _IO_sgetn (_IO_FILE *, void *, size_t);

extern __off64_t _IO_seekoff (_IO_FILE *, __off64_t, int, int);
extern __off64_t _IO_seekpos (_IO_FILE *, __off64_t, int);

extern void _IO_free_backup_area (_IO_FILE *) __attribute__ ((__nothrow__ , __leaf__));
# 42 "/usr/include/stdio.h" 2 3 4




typedef __gnuc_va_list va_list;
# 57 "/usr/include/stdio.h" 3 4
typedef __off_t off_t;
# 71 "/usr/include/stdio.h" 3 4
typedef __ssize_t ssize_t;






typedef _G_fpos_t fpos_t;
# 131 "/usr/include/stdio.h" 3 4
# 1 "/usr/include/x86_64-linux-gnu/bits/stdio_lim.h" 1 3 4
# 132 "/usr/include/stdio.h" 2 3 4



extern struct _IO_FILE *stdin;
extern struct _IO_FILE *stdout;
extern struct _IO_FILE *stderr;






extern int remove (const char *__filename) __attribute__ ((__nothrow__ , __leaf__));

extern int rename (const char *__old, const char *__new) __attribute__ ((__nothrow__ , __leaf__));



extern int renameat (int __oldfd, const char *__old, int __newfd,
       const char *__new) __attribute__ ((__nothrow__ , __leaf__));







extern FILE *tmpfile (void) ;
# 173 "/usr/include/stdio.h" 3 4
extern char *tmpnam (char *__s) __attribute__ ((__nothrow__ , __leaf__)) ;




extern char *tmpnam_r (char *__s) __attribute__ ((__nothrow__ , __leaf__)) ;
# 190 "/usr/include/stdio.h" 3 4
extern char *tempnam (const char *__dir, const char *__pfx)
     __attribute__ ((__nothrow__ , __leaf__)) __attribute__ ((__malloc__)) ;







extern int fclose (FILE *__stream);




extern int fflush (FILE *__stream);
# 213 "/usr/include/stdio.h" 3 4
extern int fflush_unlocked (FILE *__stream);
# 232 "/usr/include/stdio.h" 3 4
extern FILE *fopen (const char *__restrict __filename,
      const char *__restrict __modes) ;




extern FILE *freopen (const char *__restrict __filename,
        const char *__restrict __modes,
        FILE *__restrict __stream) ;
# 265 "/usr/include/stdio.h" 3 4
extern FILE *fdopen (int __fd, const char *__modes) __attribute__ ((__nothrow__ , __leaf__)) ;
# 278 "/usr/include/stdio.h" 3 4
extern FILE *fmemopen (void *__s, size_t __len, const char *__modes)
  __attribute__ ((__nothrow__ , __leaf__)) ;




extern FILE *open_memstream (char **__bufloc, size_t *__sizeloc) __attribute__ ((__nothrow__ , __leaf__)) ;





extern void setbuf (FILE *__restrict __stream, char *__restrict __buf) __attribute__ ((__nothrow__ , __leaf__));



extern int setvbuf (FILE *__restrict __stream, char *__restrict __buf,
      int __modes, size_t __n) __attribute__ ((__nothrow__ , __leaf__));




extern void setbuffer (FILE *__restrict __stream, char *__restrict __buf,
         size_t __size) __attribute__ ((__nothrow__ , __leaf__));


extern void setlinebuf (FILE *__stream) __attribute__ ((__nothrow__ , __leaf__));







extern int fprintf (FILE *__restrict __stream,
      const char *__restrict __format, ...);




extern int printf (const char *__restrict __format, ...);

extern int sprintf (char *__restrict __s,
      const char *__restrict __format, ...) __attribute__ ((__nothrow__));





extern int vfprintf (FILE *__restrict __s, const char *__restrict __format,
       __gnuc_va_list __arg);




extern int vprintf (const char *__restrict __format, __gnuc_va_list __arg);

extern int vsprintf (char *__restrict __s, const char *__restrict __format,
       __gnuc_va_list __arg) __attribute__ ((__nothrow__));



extern int snprintf (char *__restrict __s, size_t __maxlen,
       const char *__restrict __format, ...)
     __attribute__ ((__nothrow__)) __attribute__ ((__format__ (__printf__, 3, 4)));

extern int vsnprintf (char *__restrict __s, size_t __maxlen,
        const char *__restrict __format, __gnuc_va_list __arg)
     __attribute__ ((__nothrow__)) __attribute__ ((__format__ (__printf__, 3, 0)));
# 365 "/usr/include/stdio.h" 3 4
extern int vdprintf (int __fd, const char *__restrict __fmt,
       __gnuc_va_list __arg)
     __attribute__ ((__format__ (__printf__, 2, 0)));
extern int dprintf (int __fd, const char *__restrict __fmt, ...)
     __attribute__ ((__format__ (__printf__, 2, 3)));







extern int fscanf (FILE *__restrict __stream,
     const char *__restrict __format, ...) ;




extern int scanf (const char *__restrict __format, ...) ;

extern int sscanf (const char *__restrict __s,
     const char *__restrict __format, ...) __attribute__ ((__nothrow__ , __leaf__));
# 395 "/usr/include/stdio.h" 3 4
extern int fscanf (FILE *__restrict __stream, const char *__restrict __format, ...) __asm__ ("" "__isoc99_fscanf")

                               ;
extern int scanf (const char *__restrict __format, ...) __asm__ ("" "__isoc99_scanf")
                              ;
extern int sscanf (const char *__restrict __s, const char *__restrict __format, ...) __asm__ ("" "__isoc99_sscanf") __attribute__ ((__nothrow__ , __leaf__))

                      ;
# 420 "/usr/include/stdio.h" 3 4
extern int vfscanf (FILE *__restrict __s, const char *__restrict __format,
      __gnuc_va_list __arg)
     __attribute__ ((__format__ (__scanf__, 2, 0))) ;





extern int vscanf (const char *__restrict __format, __gnuc_va_list __arg)
     __attribute__ ((__format__ (__scanf__, 1, 0))) ;


extern int vsscanf (const char *__restrict __s,
      const char *__restrict __format, __gnuc_va_list __arg)
     __attribute__ ((__nothrow__ , __leaf__)) __attribute__ ((__format__ (__scanf__, 2, 0)));
# 443 "/usr/include/stdio.h" 3 4
extern int vfscanf (FILE *__restrict __s, const char *__restrict __format, __gnuc_va_list __arg) __asm__ ("" "__isoc99_vfscanf")



     __attribute__ ((__format__ (__scanf__, 2, 0))) ;
extern int vscanf (const char *__restrict __format, __gnuc_va_list __arg) __asm__ ("" "__isoc99_vscanf")

     __attribute__ ((__format__ (__scanf__, 1, 0))) ;
extern int vsscanf (const char *__restrict __s, const char *__restrict __format, __gnuc_va_list __arg) __asm__ ("" "__isoc99_vsscanf") __attribute__ ((__nothrow__ , __leaf__))



     __attribute__ ((__format__ (__scanf__, 2, 0)));
# 477 "/usr/include/stdio.h" 3 4
extern int fgetc (FILE *__stream);
extern int getc (FILE *__stream);





extern int getchar (void);
# 495 "/usr/include/stdio.h" 3 4
extern int getc_unlocked (FILE *__stream);
extern int getchar_unlocked (void);
# 506 "/usr/include/stdio.h" 3 4
extern int fgetc_unlocked (FILE *__stream);
# 517 "/usr/include/stdio.h" 3 4
extern int fputc (int __c, FILE *__stream);
extern int putc (int __c, FILE *__stream);





extern int putchar (int __c);
# 537 "/usr/include/stdio.h" 3 4
extern int fputc_unlocked (int __c, FILE *__stream);







extern int putc_unlocked (int __c, FILE *__stream);
extern int putchar_unlocked (int __c);






extern int getw (FILE *__stream);


extern int putw (int __w, FILE *__stream);







extern char *fgets (char *__restrict __s, int __n, FILE *__restrict __stream)
     ;
# 603 "/usr/include/stdio.h" 3 4
extern __ssize_t __getdelim (char **__restrict __lineptr,
          size_t *__restrict __n, int __delimiter,
          FILE *__restrict __stream) ;
extern __ssize_t getdelim (char **__restrict __lineptr,
        size_t *__restrict __n, int __delimiter,
        FILE *__restrict __stream) ;







extern __ssize_t getline (char **__restrict __lineptr,
       size_t *__restrict __n,
       FILE *__restrict __stream) ;







extern int fputs (const char *__restrict __s, FILE *__restrict __stream);





extern int puts (const char *__s);






extern int ungetc (int __c, FILE *__stream);






extern size_t fread (void *__restrict __ptr, size_t __size,
       size_t __n, FILE *__restrict __stream) ;




extern size_t fwrite (const void *__restrict __ptr, size_t __size,
        size_t __n, FILE *__restrict __s);
# 673 "/usr/include/stdio.h" 3 4
extern size_t fread_unlocked (void *__restrict __ptr, size_t __size,
         size_t __n, FILE *__restrict __stream) ;
extern size_t fwrite_unlocked (const void *__restrict __ptr, size_t __size,
          size_t __n, FILE *__restrict __stream);







extern int fseek (FILE *__stream, long int __off, int __whence);




extern long int ftell (FILE *__stream) ;




extern void rewind (FILE *__stream);
# 707 "/usr/include/stdio.h" 3 4
extern int fseeko (FILE *__stream, __off_t __off, int __whence);




extern __off_t ftello (FILE *__stream) ;
# 731 "/usr/include/stdio.h" 3 4
extern int fgetpos (FILE *__restrict __stream, fpos_t *__restrict __pos);




extern int fsetpos (FILE *__stream, const fpos_t *__pos);
# 757 "/usr/include/stdio.h" 3 4
extern void clearerr (FILE *__stream) __attribute__ ((__nothrow__ , __leaf__));

extern int feof (FILE *__stream) __attribute__ ((__nothrow__ , __leaf__)) ;

extern int ferror (FILE *__stream) __attribute__ ((__nothrow__ , __leaf__)) ;



extern void clearerr_unlocked (FILE *__stream) __attribute__ ((__nothrow__ , __leaf__));
extern int feof_unlocked (FILE *__stream) __attribute__ ((__nothrow__ , __leaf__)) ;
extern int ferror_unlocked (FILE *__stream) __attribute__ ((__nothrow__ , __leaf__)) ;







extern void perror (const char *__s);





# 1 "/usr/include/x86_64-linux-gnu/bits/sys_errlist.h" 1 3 4
# 26 "/usr/include/x86_64-linux-gnu/bits/sys_errlist.h" 3 4
extern int sys_nerr;
extern const char *const sys_errlist[];
# 782 "/usr/include/stdio.h" 2 3 4




extern int fileno (FILE *__stream) __attribute__ ((__nothrow__ , __leaf__)) ;




extern int fileno_unlocked (FILE *__stream) __attribute__ ((__nothrow__ , __leaf__)) ;
# 800 "/usr/include/stdio.h" 3 4
extern FILE *popen (const char *__command, const char *__modes) ;





extern int pclose (FILE *__stream);





extern char *ctermid (char *__s) __attribute__ ((__nothrow__ , __leaf__));
# 840 "/usr/include/stdio.h" 3 4
extern void flockfile (FILE *__stream) __attribute__ ((__nothrow__ , __leaf__));



extern int ftrylockfile (FILE *__stream) __attribute__ ((__nothrow__ , __leaf__)) ;


extern void funlockfile (FILE *__stream) __attribute__ ((__nothrow__ , __leaf__));
# 868 "/usr/include/stdio.h" 3 4

# 2 "source.c" 2


# 3 "source.c"
int main()
{
        int a[8]={13,19,32,42,54,64,21,21};
        int temp=0;
        int i,j;
        for (i=0;i<8;i++)
        {
                for(j=i+1;j<8;j++)
                {
                        if (a[i]<a[j])
                        {
                                temp=a[i];
                                a[i]=a[j];
                                a[j]=temp;
                        }
                }
        }
        for (i=0;i<8;i++)
                printf("%d ",a[i]);
        printf("\n");
 return 0;
}
```
通过查阅资料，-E只激活了预处理，没有生成文件，但可以通过重定向输出到一个文件中并查看其内容。
可以看出，在#1部分，主要是对#include<stdio.h>进行了处理，对其中的变量和函数进行了定义和声明，而程序的主体main（）函数在#3部分，没有进行修改和翻译。
### 利用-S编译生成结果
执行命令gcc  -S source.c，生成文件source.s，内容如下：
```
	.file	"source.c"
	.text
	.section	.rodata
.LC0:
	.string	"%d "
	.text
	.globl	main
	.type	main, @function
main:
.LFB0:
	.cfi_startproc				;the initialization
	pushq	%rbp
	.cfi_def_cfa_offset 16
	.cfi_offset 6, -16
	movq	%rsp, %rbp
	.cfi_def_cfa_register 6
	subq	$64, %rsp
	movq	%fs:40, %rax
	movq	%rax, -8(%rbp)
	xorl	%eax, %eax
	movl	$13, -48(%rbp)
	movl	$19, -44(%rbp)
	movl	$32, -40(%rbp)
	movl	$42, -36(%rbp)
	movl	$54, -32(%rbp)
	movl	$64, -28(%rbp)
	movl	$21, -24(%rbp)
	movl	$21, -20(%rbp)
	movl	$0, -52(%rbp)
	movl	$0, -60(%rbp)
	jmp	.L2
.L6:
	movl	-60(%rbp), %eax
	addl	$1, %eax
	movl	%eax, -56(%rbp)
	jmp	.L3
.L5:						;the main part: compare and sort
	movl	-60(%rbp), %eax
	cltq
	movl	-48(%rbp,%rax,4), %edx
	movl	-56(%rbp), %eax
	cltq
	movl	-48(%rbp,%rax,4), %eax
	cmpl	%eax, %edx
	jge	.L4
	movl	-60(%rbp), %eax
	cltq
	movl	-48(%rbp,%rax,4), %eax
	movl	%eax, -52(%rbp)
	movl	-56(%rbp), %eax
	cltq
	movl	-48(%rbp,%rax,4), %edx
	movl	-60(%rbp), %eax
	cltq
	movl	%edx, -48(%rbp,%rax,4)
	movl	-56(%rbp), %eax
	cltq
	movl	-52(%rbp), %edx
	movl	%edx, -48(%rbp,%rax,4)
.L4:
	addl	$1, -56(%rbp)
.L3:
	cmpl	$7, -56(%rbp)
	jle	.L5
	addl	$1, -60(%rbp)
.L2:
	cmpl	$7, -60(%rbp)
	jle	.L6
	movl	$0, -60(%rbp)
	jmp	.L7
.L8:
	movl	-60(%rbp), %eax
	cltq
	movl	-48(%rbp,%rax,4), %eax
	movl	%eax, %esi
	leaq	.LC0(%rip), %rdi
	movl	$0, %eax
	call	printf@PLT
	addl	$1, -60(%rbp)
.L7:
	cmpl	$7, -60(%rbp)				;judge whether it is the end 			
	jle	.L8
	movl	$10, %edi
	call	putchar@PLT				;the output
	movl	$0, %eax
	movq	-8(%rbp), %rcx
	xorq	%fs:40, %rcx
	je	.L10
	call	__stack_chk_fail@PLT
.L10:
	leave
	.cfi_def_cfa 7, 8
	ret
	.cfi_endproc
.LFE0:
	.size	main, .-main
	.ident	"GCC: (Ubuntu 7.3.0-16ubuntu3) 7.3.0"
	.section	.note.GNU-stack,"",@progbits
```
此时，c文件经过了预处理和编译两个步骤，生成了汇编代码。
### 利用-S编译生成结果
执行命令gcc  -c source.c，生成可执行文件source.o。
执行命令objdump -D source.o,可以得到source.o中的所有部分的汇编信息：
```
source.o:     file format elf64-x86-64


Disassembly of section .text:

0000000000000000 <main>:
   0:	55                   	push   %rbp
   1:	48 89 e5             	mov    %rsp,%rbp
   4:	48 83 ec 40          	sub    $0x40,%rsp
   8:	64 48 8b 04 25 28 00 	mov    %fs:0x28,%rax
   f:	00 00 
  11:	48 89 45 f8          	mov    %rax,-0x8(%rbp)
  15:	31 c0                	xor    %eax,%eax
  17:	c7 45 d0 0d 00 00 00 	movl   $0xd,-0x30(%rbp)
  1e:	c7 45 d4 13 00 00 00 	movl   $0x13,-0x2c(%rbp)
  25:	c7 45 d8 20 00 00 00 	movl   $0x20,-0x28(%rbp)
  2c:	c7 45 dc 2a 00 00 00 	movl   $0x2a,-0x24(%rbp)
  33:	c7 45 e0 36 00 00 00 	movl   $0x36,-0x20(%rbp)
  3a:	c7 45 e4 40 00 00 00 	movl   $0x40,-0x1c(%rbp)
  41:	c7 45 e8 15 00 00 00 	movl   $0x15,-0x18(%rbp)
  48:	c7 45 ec 15 00 00 00 	movl   $0x15,-0x14(%rbp)
  4f:	c7 45 cc 00 00 00 00 	movl   $0x0,-0x34(%rbp)
  56:	c7 45 c4 00 00 00 00 	movl   $0x0,-0x3c(%rbp)
  5d:	eb 59                	jmp    b8 <main+0xb8>
  5f:	8b 45 c4             	mov    -0x3c(%rbp),%eax
  62:	83 c0 01             	add    $0x1,%eax
  65:	89 45 c8             	mov    %eax,-0x38(%rbp)
  68:	eb 44                	jmp    ae <main+0xae>
  6a:	8b 45 c4             	mov    -0x3c(%rbp),%eax
  6d:	48 98                	cltq   
  6f:	8b 54 85 d0          	mov    -0x30(%rbp,%rax,4),%edx
  73:	8b 45 c8             	mov    -0x38(%rbp),%eax
  76:	48 98                	cltq   
  78:	8b 44 85 d0          	mov    -0x30(%rbp,%rax,4),%eax
  7c:	39 c2                	cmp    %eax,%edx
  7e:	7d 2a                	jge    aa <main+0xaa>
  80:	8b 45 c4             	mov    -0x3c(%rbp),%eax
  83:	48 98                	cltq   
  85:	8b 44 85 d0          	mov    -0x30(%rbp,%rax,4),%eax
  89:	89 45 cc             	mov    %eax,-0x34(%rbp)
  8c:	8b 45 c8             	mov    -0x38(%rbp),%eax
  8f:	48 98                	cltq   
  91:	8b 54 85 d0          	mov    -0x30(%rbp,%rax,4),%edx
  95:	8b 45 c4             	mov    -0x3c(%rbp),%eax
  98:	48 98                	cltq   
  9a:	89 54 85 d0          	mov    %edx,-0x30(%rbp,%rax,4)
  9e:	8b 45 c8             	mov    -0x38(%rbp),%eax
  a1:	48 98                	cltq   
  a3:	8b 55 cc             	mov    -0x34(%rbp),%edx
  a6:	89 54 85 d0          	mov    %edx,-0x30(%rbp,%rax,4)
  aa:	83 45 c8 01          	addl   $0x1,-0x38(%rbp)
  ae:	83 7d c8 07          	cmpl   $0x7,-0x38(%rbp)
  b2:	7e b6                	jle    6a <main+0x6a>
  b4:	83 45 c4 01          	addl   $0x1,-0x3c(%rbp)
  b8:	83 7d c4 07          	cmpl   $0x7,-0x3c(%rbp)
  bc:	7e a1                	jle    5f <main+0x5f>
  be:	c7 45 c4 00 00 00 00 	movl   $0x0,-0x3c(%rbp)
  c5:	eb 20                	jmp    e7 <main+0xe7>
  c7:	8b 45 c4             	mov    -0x3c(%rbp),%eax
  ca:	48 98                	cltq   
  cc:	8b 44 85 d0          	mov    -0x30(%rbp,%rax,4),%eax
  d0:	89 c6                	mov    %eax,%esi
  d2:	48 8d 3d 00 00 00 00 	lea    0x0(%rip),%rdi        # d9 <main+0xd9>
  d9:	b8 00 00 00 00       	mov    $0x0,%eax
  de:	e8 00 00 00 00       	callq  e3 <main+0xe3>
  e3:	83 45 c4 01          	addl   $0x1,-0x3c(%rbp)
  e7:	83 7d c4 07          	cmpl   $0x7,-0x3c(%rbp)
  eb:	7e da                	jle    c7 <main+0xc7>
  ed:	bf 0a 00 00 00       	mov    $0xa,%edi
  f2:	e8 00 00 00 00       	callq  f7 <main+0xf7>
  f7:	b8 00 00 00 00       	mov    $0x0,%eax
  fc:	48 8b 4d f8          	mov    -0x8(%rbp),%rcx
 100:	64 48 33 0c 25 28 00 	xor    %fs:0x28,%rcx
 107:	00 00 
 109:	74 05                	je     110 <main+0x110>
 10b:	e8 00 00 00 00       	callq  110 <main+0x110>
 110:	c9                   	leaveq 
 111:	c3                   	retq   

Disassembly of section .rodata:

0000000000000000 <.rodata>:
   0:	25                   	.byte 0x25
   1:	64 20 00             	and    %al,%fs:(%rax)

Disassembly of section .comment:

0000000000000000 <.comment>:
   0:	00 47 43             	add    %al,0x43(%rdi)
   3:	43 3a 20             	rex.XB cmp (%r8),%spl
   6:	28 55 62             	sub    %dl,0x62(%rbp)
   9:	75 6e                	jne    79 <main+0x79>
   b:	74 75                	je     82 <main+0x82>
   d:	20 37                	and    %dh,(%rdi)
   f:	2e 33 2e             	xor    %cs:(%rsi),%ebp
  12:	30 2d 31 36 75 62    	xor    %ch,0x62753631(%rip)        # 62753649 <main+0x62753649>
  18:	75 6e                	jne    88 <main+0x88>
  1a:	74 75                	je     91 <main+0x91>
  1c:	33 29                	xor    (%rcx),%ebp
  1e:	20 37                	and    %dh,(%rdi)
  20:	2e 33 2e             	xor    %cs:(%rsi),%ebp
  23:	30 00                	xor    %al,(%rax)

Disassembly of section .eh_frame:

0000000000000000 <.eh_frame>:
   0:	14 00                	adc    $0x0,%al
   2:	00 00                	add    %al,(%rax)
   4:	00 00                	add    %al,(%rax)
   6:	00 00                	add    %al,(%rax)
   8:	01 7a 52             	add    %edi,0x52(%rdx)
   b:	00 01                	add    %al,(%rcx)
   d:	78 10                	js     1f <.eh_frame+0x1f>
   f:	01 1b                	add    %ebx,(%rbx)
  11:	0c 07                	or     $0x7,%al
  13:	08 90 01 00 00 1c    	or     %dl,0x1c000001(%rax)
  19:	00 00                	add    %al,(%rax)
  1b:	00 1c 00             	add    %bl,(%rax,%rax,1)
  1e:	00 00                	add    %al,(%rax)
  20:	00 00                	add    %al,(%rax)
  22:	00 00                	add    %al,(%rax)
  24:	12 01                	adc    (%rcx),%al
  26:	00 00                	add    %al,(%rax)
  28:	00 41 0e             	add    %al,0xe(%rcx)
  2b:	10 86 02 43 0d 06    	adc    %al,0x60d4302(%rsi)
  31:	03 0d 01 0c 07 08    	add    0x8070c01(%rip),%ecx        # 8070c38 <main+0x8070c38>
	...
```
可以看出.text部分和用-S生成的汇编代码一致。
###利用-o编译生成结果
该指令可以将编译结果输出到一个文档中，命名为a.out
###利用-m32编译生成结果
在执行命令之前，首先需sudo apt-get install gcc-multilib，否则编译会报错：
```
In file included from source.c:1:0:
/usr/include/stdio.h:27:10: fatal error: bits/libc-header-start.h: No such file or directory
 #include <bits/libc-header-start.h>
          ^~~~~~~~~~~~~~~~~~~~~~~~~~

```
执行命令gcc -S source.c -m32 -o source32.s，便可得到在32位下编译得到的汇编代码：
```
	.file	"source.c"
	.text
	.section	.rodata
.LC0:
	.string	"%d "
	.text
	.globl	main
	.type	main, @function
main:
.LFB0:
	.cfi_startproc
	leal	4(%esp), %ecx
	.cfi_def_cfa 1, 0
	andl	$-16, %esp
	pushl	-4(%ecx)
	pushl	%ebp
	.cfi_escape 0x10,0x5,0x2,0x75,0
	movl	%esp, %ebp
	pushl	%ebx
	pushl	%ecx
	.cfi_escape 0xf,0x3,0x75,0x78,0x6
	.cfi_escape 0x10,0x3,0x2,0x75,0x7c
	subl	$48, %esp
	call	__x86.get_pc_thunk.bx
	addl	$_GLOBAL_OFFSET_TABLE_, %ebx
	movl	%gs:20, %eax
	movl	%eax, -12(%ebp)
	xorl	%eax, %eax
	movl	$13, -44(%ebp)
	movl	$19, -40(%ebp)
	movl	$32, -36(%ebp)
	movl	$42, -32(%ebp)
	movl	$54, -28(%ebp)
	movl	$64, -24(%ebp)
	movl	$21, -20(%ebp)
	movl	$21, -16(%ebp)
	movl	$0, -48(%ebp)
	movl	$0, -56(%ebp)
	jmp	.L2
.L6:
	movl	-56(%ebp), %eax
	addl	$1, %eax
	movl	%eax, -52(%ebp)
	jmp	.L3
.L5:
	movl	-56(%ebp), %eax
	movl	-44(%ebp,%eax,4), %edx
	movl	-52(%ebp), %eax
	movl	-44(%ebp,%eax,4), %eax
	cmpl	%eax, %edx
	jge	.L4
	movl	-56(%ebp), %eax
	movl	-44(%ebp,%eax,4), %eax
	movl	%eax, -48(%ebp)
	movl	-52(%ebp), %eax
	movl	-44(%ebp,%eax,4), %edx
	movl	-56(%ebp), %eax
	movl	%edx, -44(%ebp,%eax,4)
	movl	-52(%ebp), %eax
	movl	-48(%ebp), %edx
	movl	%edx, -44(%ebp,%eax,4)
.L4:
	addl	$1, -52(%ebp)
.L3:
	cmpl	$7, -52(%ebp)
	jle	.L5
	addl	$1, -56(%ebp)
.L2:
	cmpl	$7, -56(%ebp)
	jle	.L6
	movl	$0, -56(%ebp)
	jmp	.L7
.L8:
	movl	-56(%ebp), %eax
	movl	-44(%ebp,%eax,4), %eax
	subl	$8, %esp
	pushl	%eax
	leal	.LC0@GOTOFF(%ebx), %eax
	pushl	%eax
	call	printf@PLT
	addl	$16, %esp
	addl	$1, -56(%ebp)
.L7:
	cmpl	$7, -56(%ebp)
	jle	.L8
	subl	$12, %esp
	pushl	$10
	call	putchar@PLT
	addl	$16, %esp
	movl	$0, %eax
	movl	-12(%ebp), %ecx
	xorl	%gs:20, %ecx
	je	.L10
	call	__stack_chk_fail_local
.L10:
	leal	-8(%ebp), %esp
	popl	%ecx
	.cfi_restore 1
	.cfi_def_cfa 1, 0
	popl	%ebx
	.cfi_restore 3
	popl	%ebp
	.cfi_restore 5
	leal	-4(%ecx), %esp
	.cfi_def_cfa 4, 4
	ret
	.cfi_endproc
.LFE0:
	.size	main, .-main
	.section	.text.__x86.get_pc_thunk.bx,"axG",@progbits,__x86.get_pc_thunk.bx,comdat
	.globl	__x86.get_pc_thunk.bx
	.hidden	__x86.get_pc_thunk.bx
	.type	__x86.get_pc_thunk.bx, @function
__x86.get_pc_thunk.bx:
.LFB1:
	.cfi_startproc
	movl	(%esp), %ebx
	ret
	.cfi_endproc
.LFE1:
	.hidden	__stack_chk_fail_local
	.ident	"GCC: (Ubuntu 7.3.0-16ubuntu3) 7.3.0"
	.section	.note.GNU-stack,"",@progbits
```
###利用-m64编译生成结果
执行命令gcc -S source.c -m64 -o source64.s，便可得到在64位下编译得到的汇编代码：
```
	.file	"source.c"
	.text
	.section	.rodata
.LC0:
	.string	"%d "
	.text
	.globl	main
	.type	main, @function
main:
.LFB0:
	.cfi_startproc
	pushq	%rbp
	.cfi_def_cfa_offset 16
	.cfi_offset 6, -16
	movq	%rsp, %rbp
	.cfi_def_cfa_register 6			;this part of initialization is very different from the 32-bit version
	subq	$64, %rsp			;in 32-bit version, we use %esp,and the number is different (32-bit: subl $48,%esp)
	movq	%fs:40, %rax
	movq	%rax, -8(%rbp)
	xorl	%eax, %eax
	movl	$13, -48(%rbp)			;all the numbers needs 4 more bytes to be stored and so comes the difference in the number minused
	movl	$19, -44(%rbp)
	movl	$32, -40(%rbp)
	movl	$42, -36(%rbp)
	movl	$54, -32(%rbp)
	movl	$64, -28(%rbp)
	movl	$21, -24(%rbp)
	movl	$21, -20(%rbp)
	movl	$0, -52(%rbp)
	movl	$0, -60(%rbp)
	jmp	.L2
.L6:						;the below part is almost the same as the 32-bit version except for the difference mentioned above
	movl	-60(%rbp), %eax
	addl	$1, %eax
	movl	%eax, -56(%rbp)
	jmp	.L3
.L5:
	movl	-60(%rbp), %eax
	cltq
	movl	-48(%rbp,%rax,4), %edx
	movl	-56(%rbp), %eax
	cltq
	movl	-48(%rbp,%rax,4), %eax
	cmpl	%eax, %edx
	jge	.L4
	movl	-60(%rbp), %eax
	cltq
	movl	-48(%rbp,%rax,4), %eax
	movl	%eax, -52(%rbp)
	movl	-56(%rbp), %eax
	cltq
	movl	-48(%rbp,%rax,4), %edx
	movl	-60(%rbp), %eax
	cltq
	movl	%edx, -48(%rbp,%rax,4)
	movl	-56(%rbp), %eax
	cltq
	movl	-52(%rbp), %edx
	movl	%edx, -48(%rbp,%rax,4)
.L4:
	addl	$1, -56(%rbp)
.L3:
	cmpl	$7, -56(%rbp)
	jle	.L5
	addl	$1, -60(%rbp)
.L2:
	cmpl	$7, -60(%rbp)
	jle	.L6
	movl	$0, -60(%rbp)
	jmp	.L7
.L8:
	movl	-60(%rbp), %eax
	cltq
	movl	-48(%rbp,%rax,4), %eax
	movl	%eax, %esi
	leaq	.LC0(%rip), %rdi
	movl	$0, %eax
	call	printf@PLT
	addl	$1, -60(%rbp)
.L7:
	cmpl	$7, -60(%rbp)
	jle	.L8
	movl	$10, %edi
	call	putchar@PLT
	movl	$0, %eax
	movq	-8(%rbp), %rcx
	xorq	%fs:40, %rcx
	je	.L10
	call	__stack_chk_fail@PLT
.L10:									;this place is also different from the 32-bit version
	leave
	.cfi_def_cfa 7, 8
	ret
	.cfi_endproc
.LFE0:
	.size	main, .-main
	.ident	"GCC: (Ubuntu 7.3.0-16ubuntu3) 7.3.0"
	.section	.note.GNU-stack,"",@progbits
```
可以看出，32位的汇编代码和64位的代码基本相同，但在注释处略有不同
## 根据NFA编写对应的程序
### 使用方式：
* 编写的程序为analysis.c，对应的shell文件为anashell.sh
* 输入 /bin/sh anashell.sh 即可完成编译和执行，接下来便可以输入需要检查的字符串，按回车输出结果。
### 思考与解答
* 根据输入的字符串，检查每一个字符。用数组c[256]来存储读入的字符串，通过修改下标i来检查对应的字符，通过if条件判断语句来使结果不同。
* 根据课件第16页给出的图，在第1、6个状态（即当前字符为<或>时），注意i++，检查下一位后才能得到最终判断的结果。在第4，8个状态需要i--，防止因为提前检查下一个字符而最终漏读一个字符。
* 最终结果输出关系算符在字符串中的位置，如果关系算符占用两个字符（<=和>=），则输出第一个字符在字符串中的位置。
