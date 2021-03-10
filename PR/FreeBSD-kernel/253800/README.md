# 253800 – [panic] FreeBSD-13.0 (releng/13.0) panic upon duplicate IPv4 detection / page fault while in kernel mode (in function rtsock_routemsg_info)

## Summary

https://bugs.freebsd.org/bugzilla/show_bug.cgi?id=253800

## Root Causes

* Page fault at boot
* Miss memmory access at `rtsock_routemsg`
* Following patches fixed this issue?

## Resolution

* xxx At-view and separation logic may avoid page fault

## Timeline

### 2021-02-23 22:31:07 +0000

https://cgit.freebsd.org/src/commit/?id=9c4a8d24f0ffd5243fa5c6fe27178f669f16d1f5

### 2021-02-24 16:42:48 +0000

https://cgit.freebsd.org/src/commit/?id=cc3fa1e29fda2cc761e793a61cef3bd2522b3468