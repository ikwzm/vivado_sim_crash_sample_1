Xilinx Vivado Simulator Crash Sample
------------------------------------

>>>>> project_1/project_1.sim/sim_1/behav/hs_err_pid6704.log
#
# A fatal error has been detected by the Java Runtime Environment:
#
#  EXCEPTION_ACCESS_VIOLATION (0xc0000005) at pc=0x000000001632abea, pid=6704, tid=11444
#
# JRE version: Java(TM) SE Runtime Environment (7.0_40-b43) (build 1.7.0_40-b43)
# Java VM: Java HotSpot(TM) 64-Bit Server VM (24.0-b56 mixed mode windows-amd64 compressed oops)
# Problematic frame:
# C  [librdi_wavedata.dll+0x5abea]
#
# Failed to write core dump. Minidumps are not enabled by default on client versions of Windows
#
# If you would like to submit a bug report, please visit:
#   http://bugreport.sun.com/bugreport/crash.jsp
# The crash happened outside the Java Virtual Machine in native code.
# See problematic frame for where to report the bug.
#

---------------  T H R E A D  ---------------

Current thread (0x0000000033c81000):  JavaThread "AWT-EventQueue-0" [_thread_in_native, id=11444, stack(0x0000000034100000,0x0000000034400000)]

siginfo: ExceptionCode=0xc0000005, reading address 0x000000183f3200f4

Registers:
RAX=0x0000000000000000, RBX=0x000000183f3200e0, RCX=0x000000003f0f3880, RDX=0x0000000016558938
RSP=0x00000000343fd7d0, RBP=0x000000003f0f2e00, RSI=0x000000003f2e6800, RDI=0x0000000000000000
R8 =0x000000003f0f2e00, R9 =0x000000183f3200e0, R10=0x000000000000003f, R11=0x0000000000000001
R12=0x000000003f5664a0, R13=0x0000000000000000, R14=0x0000000000000000, R15=0x00000000343fde58
RIP=0x000000001632abea, EFLAGS=0x0000000000010246

Top of Stack: (sp=0x00000000343fd7d0)
0x00000000343fd7d0:   0000000034e22408 0000000041970020
0x00000000343fd7e0:   00000000247804c0 000000004197c790
0x00000000343fd7f0:   0000000000000000 0000000024780100
0x00000000343fd800:   0000000000000000 0000000000000000
0x00000000343fd810:   0000000000000000 0000000000000000
0x00000000343fd820:   0000000000000000 000000000a903829
0x00000000343fd830:   0000000024780020 0000000000000000
0x00000000343fd840:   0000000000000050 000000001e329c40
0x00000000343fd850:   000000004197c790 000000000a92f080
0x00000000343fd860:   000000003cf499a0 0000000000000002
0x00000000343fd870:   0000020000000000 0000000000000050
0x00000000343fd880:   fffffffffffffffe 00000000343fd908
0x00000000343fd890:   000000004197c790 00000000164799af
0x00000000343fd8a0:   00000000603e1425 000000000a91796d
0x00000000343fd8b0:   00000000036b0020 0000000000000050
0x00000000343fd8c0:   0000000a00000000 0000000000000000 

Instructions: (pc=0x000000001632abea)
0x000000001632abca:   00 00 00 48 8d 4c 24 70 8b 01 89 02 8b 41 04 89
0x000000001632abda:   42 04 8b 41 08 89 42 08 48 8b 9c 24 38 01 00 00
0x000000001632abea:   44 8b 53 14 44 89 54 24 68 45 85 d2 0f 84 a8 05
0x000000001632abfa:   00 00 4c 8b 8c 24 40 01 00 00 66 41 39 79 0c 74 


Register to memory mapping:

RAX=0x0000000000000000 is an unknown value
RBX=0x000000183f3200e0 is an unknown value
RCX=0x000000003f0f3880 is an unknown value
RDX=0x0000000016558938 is an unknown value
RSP=0x00000000343fd7d0 is pointing into the stack for thread: 0x0000000033c81000
RBP=0x000000003f0f2e00 is an unknown value
RSI=0x000000003f2e6800 is an unknown value
RDI=0x0000000000000000 is an unknown value
R8 =0x000000003f0f2e00 is an unknown value
R9 =0x000000183f3200e0 is an unknown value
R10=0x000000000000003f is an unknown value
R11=0x0000000000000001 is an unknown value
R12=0x000000003f5664a0 is an unknown value
R13=0x0000000000000000 is an unknown value
R14=0x0000000000000000 is an unknown value
R15=0x00000000343fde58 is pointing into the stack for thread: 0x0000000033c81000


Stack: [0x0000000034100000,0x0000000034400000],  sp=0x00000000343fd7d0,  free space=3061k
Native frames: (J=compiled Java code, j=interpreted, Vv=VM code, C=native code)
C  [librdi_wavedata.dll+0x5abea]

Java frames: (J=compiled Java code, j=interpreted, Vv=VM code)
j  ui.views.simulator.executive.simulationi.SimulationExecutive_getVirtualObjectTreeData(JLjava/lang/String;)Ljava/lang/String;+0
j  ui.views.B.b.a.fLm()Lui/views/waveform/executive/gpb/WVTree$WVTreeMessage;+6
j  ui.views.B.e.e.load()V+7
j  ui.views.B.e.q.fND()V+4
j  ui.views.B.e.q.a(Lui/frmwork/a/f;)V+49
j  ui.frmwork.a.i.c(Lui/frmwork/a/f;)V+52
j  ui.frmwork.HTclEventBroker.a(JZ)V+319
j  ui.frmwork.s.run()V+9
J  java.awt.EventQueue$3.run()Ljava/lang/Object;
v  ~StubRoutines::call_stub
J  java.security.AccessController.doPrivileged(Ljava/security/PrivilegedAction;Ljava/security/AccessControlContext;)Ljava/lang/Object;
J  java.security.ProtectionDomain$1.doIntersectionPrivilege(Ljava/security/PrivilegedAction;Ljava/security/AccessControlContext;Ljava/security/AccessControlContext;)Ljava/lang/Object;
J  java.awt.EventQueue.dispatchEvent(Ljava/awt/AWTEvent;)V
J  java.awt.EventDispatchThread.pumpOneEventForFilters(I)V
j  java.awt.EventDispatchThread.pumpEventsForFilter(ILjava/awt/Conditional;Ljava/awt/EventFilter;)V+35
j  java.awt.EventDispatchThread.pumpEventsForHierarchy(ILjava/awt/Conditional;Ljava/awt/Component;)V+11
j  java.awt.EventDispatchThread.pumpEvents(ILjava/awt/Conditional;)V+4
j  java.awt.EventDispatchThread.pumpEvents(Ljava/awt/Conditional;)V+3
j  java.awt.EventDispatchThread.run()V+9
v  ~StubRoutines::call_stub

---------------  P R O C E S S  ---------------

Java Threads: ( => current thread )
  0x000000003f527800 JavaThread "Image Fetcher 0" daemon [_thread_blocked, id=11840, stack(0x0000000045870000,0x0000000045b70000)]
  0x000000003dacd800 JavaThread "Run Simulation" [_thread_blocked, id=8304, stack(0x000000004e680000,0x000000004e980000)]
  0x000000003620d000 JavaThread "Monitor File Timestamp" [_thread_blocked, id=12232, stack(0x000000004e080000,0x000000004e380000)]
  0x000000003620e000 JavaThread "Monitor File Timestamp" [_thread_blocked, id=11828, stack(0x000000004d780000,0x000000004da80000)]
  0x000000003620f000 JavaThread "Monitor File Timestamp" [_thread_blocked, id=5744, stack(0x000000004ce80000,0x000000004d180000)]
  0x000000004151f800 JavaThread "hw_ila_monitor" [_thread_blocked, id=7016, stack(0x000000003c640000,0x000000003c940000)]
  0x000000003485d800 JavaThread "Update Runs" [_thread_blocked, id=6820, stack(0x000000004c580000,0x000000004c880000)]
  0x000000003048f800 JavaThread "Refresh Filesets" [_thread_blocked, id=6012, stack(0x000000004bf80000,0x000000004c280000)]
  0x000000003d7e0800 JavaThread "Timer-35" daemon [_thread_blocked, id=11976, stack(0x0000000046e80000,0x0000000047180000)]
  0x000000003d7d0800 JavaThread "RunnableQueue-35" daemon [_thread_blocked, id=11736, stack(0x0000000039040000,0x0000000039340000)]
  0x000000003d7d1800 JavaThread "Timer-34" daemon [_thread_blocked, id=4004, stack(0x0000000047980000,0x0000000047c80000)]
  0x0000000035918800 JavaThread "RunnableQueue-34" daemon [_thread_blocked, id=8132, stack(0x0000000047580000,0x0000000047880000)]
  0x0000000035911000 JavaThread "Timer-33" daemon [_thread_blocked, id=3472, stack(0x0000000036340000,0x0000000036640000)]
  0x000000003d040800 JavaThread "RunnableQueue-33" daemon [_thread_blocked, id=8892, stack(0x0000000051680000,0x0000000051980000)]
  0x0000000034b1f800 JavaThread "Timer-32" daemon [_thread_blocked, id=7232, stack(0x0000000051080000,0x0000000051380000)]
  0x000000003d03e800 JavaThread "RunnableQueue-32" daemon [_thread_blocked, id=9384, stack(0x0000000037240000,0x0000000037540000)]
  0x0000000034b67000 JavaThread "Timer-31" daemon [_thread_blocked, id=9208, stack(0x000000003bb40000,0x000000003be40000)]
  0x000000003d9d0800 JavaThread "RunnableQueue-31" daemon [_thread_blocked, id=800, stack(0x0000000049880000,0x0000000049b80000)]
  0x000000003d4b1800 JavaThread "Timer-30" daemon [_thread_blocked, id=4776, stack(0x0000000037b40000,0x0000000037e40000)]
  0x000000003d391800 JavaThread "RunnableQueue-30" daemon [_thread_blocked, id=9264, stack(0x0000000050780000,0x0000000050a80000)]
  0x000000003f651000 JavaThread "Timer-29" daemon [_thread_blocked, id=7812, stack(0x0000000038140000,0x0000000038440000)]
  0x000000003d371000 JavaThread "RunnableQueue-29" daemon [_thread_blocked, id=9816, stack(0x0000000050180000,0x0000000050480000)]
  0x000000003d2c1000 JavaThread "Timer-28" daemon [_thread_blocked, id=9172, stack(0x0000000037840000,0x0000000037b40000)]
  0x000000003d2b7000 JavaThread "RunnableQueue-28" daemon [_thread_blocked, id=2476, stack(0x000000004fb80000,0x000000004fe80000)]
  0x000000003f5d0800 JavaThread "Timer-27" daemon [_thread_blocked, id=6708, stack(0x000000004a480000,0x000000004a780000)]
  0x000000003f5d1000 JavaThread "RunnableQueue-27" daemon [_thread_blocked, id=11020, stack(0x000000004f580000,0x000000004f880000)]
  0x000000003d1f1000 JavaThread "Timer-26" daemon [_thread_blocked, id=8568, stack(0x0000000048c80000,0x0000000048f80000)]
  0x00000000347e2800 JavaThread "RunnableQueue-26" daemon [_thread_blocked, id=5684, stack(0x000000004ef80000,0x000000004f280000)]
  0x000000003cbd0800 JavaThread "Timer-25" daemon [_thread_blocked, id=4908, stack(0x0000000049e80000,0x000000004a180000)]
  0x000000003cbd2000 JavaThread "RunnableQueue-25" daemon [_thread_blocked, id=1292, stack(0x000000004e980000,0x000000004ec80000)]
  0x000000003cbc4800 JavaThread "Timer-24" daemon [_thread_blocked, id=7244, stack(0x0000000045f80000,0x0000000046280000)]
  0x000000003ce84800 JavaThread "RunnableQueue-24" daemon [_thread_blocked, id=5236, stack(0x000000004e380000,0x000000004e680000)]
  0x00000000418b3000 JavaThread "Timer-23" daemon [_thread_blocked, id=9556, stack(0x0000000049580000,0x0000000049880000)]
  0x0000000041883800 JavaThread "RunnableQueue-23" daemon [_thread_blocked, id=3684, stack(0x000000004dd80000,0x000000004e080000)]
  0x0000000041872000 JavaThread "Timer-22" daemon [_thread_blocked, id=10968, stack(0x0000000039940000,0x0000000039c40000)]
  0x0000000041815000 JavaThread "RunnableQueue-22" daemon [_thread_blocked, id=4860, stack(0x000000004da80000,0x000000004dd80000)]
  0x0000000041804800 JavaThread "Timer-21" daemon [_thread_blocked, id=4072, stack(0x000000004d480000,0x000000004d780000)]
  0x00000000362f0800 JavaThread "RunnableQueue-21" daemon [_thread_blocked, id=5412, stack(0x000000004d180000,0x000000004d480000)]
  0x00000000362f3000 JavaThread "Timer-20" daemon [_thread_blocked, id=1036, stack(0x0000000035a40000,0x0000000035d40000)]
  0x00000000362f4000 JavaThread "RunnableQueue-20" daemon [_thread_blocked, id=7772, stack(0x000000004cb80000,0x000000004ce80000)]
  0x00000000362f6000 JavaThread "Timer-19" daemon [_thread_blocked, id=4264, stack(0x0000000046280000,0x0000000046580000)]
  0x00000000362f7800 JavaThread "RunnableQueue-19" daemon [_thread_blocked, id=7124, stack(0x000000004c880000,0x000000004cb80000)]
  0x00000000362fa000 JavaThread "Timer-18" daemon [_thread_blocked, id=4320, stack(0x0000000048080000,0x0000000048380000)]
  0x0000000043353000 JavaThread "RunnableQueue-18" daemon [_thread_blocked, id=5800, stack(0x000000004c280000,0x000000004c580000)]
  0x0000000041772800 JavaThread "Timer-17" daemon [_thread_blocked, id=9916, stack(0x0000000046880000,0x0000000046b80000)]
  0x0000000041774000 JavaThread "RunnableQueue-17" daemon [_thread_blocked, id=12080, stack(0x000000004bc80000,0x000000004bf80000)]
  0x0000000041777800 JavaThread "Timer-16" daemon [_thread_blocked, id=7200, stack(0x000000004b680000,0x000000004b980000)]
  0x00000000416d1800 JavaThread "RunnableQueue-16" daemon [_thread_blocked, id=4116, stack(0x000000004b380000,0x000000004b680000)]
  0x00000000416d3800 JavaThread "Timer-15" daemon [_thread_blocked, id=9976, stack(0x000000003a840000,0x000000003ab40000)]
  0x00000000416d4800 JavaThread "RunnableQueue-15" daemon [_thread_blocked, id=7832, stack(0x000000004b080000,0x000000004b380000)]
  0x00000000416a1800 JavaThread "Timer-14" daemon [_thread_blocked, id=5972, stack(0x000000004aa80000,0x000000004ad80000)]
  0x00000000416a5000 JavaThread "RunnableQueue-14" daemon [_thread_blocked, id=7420, stack(0x000000004a780000,0x000000004aa80000)]
  0x0000000041691000 JavaThread "Timer-13" daemon [_thread_blocked, id=7632, stack(0x0000000049b80000,0x0000000049e80000)]
  0x0000000041641000 JavaThread "RunnableQueue-13" daemon [_thread_blocked, id=3576, stack(0x0000000048f80000,0x0000000049280000)]
  0x0000000041643000 JavaThread "Timer-12" daemon [_thread_blocked, id=9256, stack(0x0000000048380000,0x0000000048680000)]
  0x0000000041643800 JavaThread "RunnableQueue-12" daemon [_thread_blocked, id=5388, stack(0x0000000038a40000,0x0000000038d40000)]
  0x000000003f270800 JavaThread "Timer-11" daemon [_thread_blocked, id=10292, stack(0x0000000047180000,0x0000000047480000)]
  0x000000003f271000 JavaThread "RunnableQueue-11" daemon [_thread_blocked, id=1168, stack(0x0000000045c80000,0x0000000045f80000)]
  0x000000003f273000 JavaThread "Timer-10" daemon [_thread_blocked, id=7488, stack(0x0000000039c40000,0x0000000039f40000)]
  0x000000003f274000 JavaThread "RunnableQueue-10" daemon [_thread_blocked, id=6920, stack(0x0000000039340000,0x0000000039640000)]
  0x0000000041610800 JavaThread "Timer-9" daemon [_thread_blocked, id=10784, stack(0x000000003b140000,0x000000003b440000)]
  0x0000000041611000 JavaThread "RunnableQueue-9" daemon [_thread_blocked, id=7284, stack(0x000000003a540000,0x000000003a840000)]
  0x0000000041613000 JavaThread "Timer-8" daemon [_thread_blocked, id=6640, stack(0x0000000038740000,0x0000000038a40000)]
  0x0000000041614800 JavaThread "RunnableQueue-8" daemon [_thread_blocked, id=7576, stack(0x0000000037540000,0x0000000037840000)]
  0x00000000415f3000 JavaThread "Timer-7" daemon [_thread_blocked, id=9048, stack(0x0000000046b80000,0x0000000046e80000)]
  0x00000000415f3800 JavaThread "RunnableQueue-7" daemon [_thread_blocked, id=6540, stack(0x0000000047d80000,0x0000000048080000)]
  0x0000000041584000 JavaThread "Timer-6" daemon [_thread_blocked, id=9064, stack(0x000000003c340000,0x000000003c640000)]
  0x0000000041585000 JavaThread "RunnableQueue-6" daemon [_thread_blocked, id=1992, stack(0x000000003be40000,0x000000003c140000)]
  0x0000000041586800 JavaThread "Timer-5" daemon [_thread_blocked, id=9524, stack(0x000000003b840000,0x000000003bb40000)]
  0x0000000041581000 JavaThread "RunnableQueue-5" daemon [_thread_blocked, id=7916, stack(0x000000003b440000,0x000000003b740000)]
  0x0000000041511000 JavaThread "Timer-4" daemon [_thread_blocked, id=11084, stack(0x000000003ae40000,0x000000003b140000)]
  0x0000000041511800 JavaThread "RunnableQueue-4" daemon [_thread_blocked, id=5996, stack(0x000000003ab40000,0x000000003ae40000)]
  0x0000000041513000 JavaThread "Timer-3" daemon [_thread_blocked, id=10144, stack(0x000000003a240000,0x000000003a540000)]
  0x0000000041514000 JavaThread "RunnableQueue-3" daemon [_thread_blocked, id=12144, stack(0x0000000039f40000,0x000000003a240000)]
  0x000000003de98800 JavaThread "Timer-2" daemon [_thread_blocked, id=5364, stack(0x0000000039640000,0x0000000039940000)]
  0x000000003de99800 JavaThread "RunnableQueue-2" daemon [_thread_blocked, id=9312, stack(0x0000000038d40000,0x0000000039040000)]
  0x000000003de9a800 JavaThread "Timer-1" daemon [_thread_blocked, id=12224, stack(0x0000000038440000,0x0000000038740000)]
  0x000000003de9b800 JavaThread "RunnableQueue-1" daemon [_thread_blocked, id=9520, stack(0x0000000037e40000,0x0000000038140000)]
  0x000000003de92000 JavaThread "Timer-0" daemon [_thread_blocked, id=8740, stack(0x0000000036e40000,0x0000000037140000)]
  0x00000000413b3800 JavaThread "RunnableQueue-0" daemon [_thread_blocked, id=9880, stack(0x0000000035e60000,0x0000000036160000)]
  0x000000003f1a8000 JavaThread "Swing-Shell" daemon [_thread_blocked, id=9492, stack(0x0000000043b40000,0x0000000043e40000)]
  0x0000000040993800 JavaThread "Monitor File Timestamp" [_thread_blocked, id=9440, stack(0x0000000043540000,0x0000000043840000)]
  0x0000000003b8b800 JavaThread "Batik CleanerThread" daemon [_thread_blocked, id=7944, stack(0x000000003ea40000,0x000000003ed40000)]
  0x000000003de95000 JavaThread "D3D Screen Updater" daemon [_thread_blocked, id=7556, stack(0x000000003df40000,0x000000003e240000)]
  0x000000001e398800 JavaThread "Process Messages" [_thread_blocked, id=3856, stack(0x0000000035100000,0x0000000035400000)]
  0x000000001e39e000 JavaThread "Thread-3" [_thread_in_native, id=11908, stack(0x0000000004020000,0x0000000005420000)]
=>0x0000000033c81000 JavaThread "AWT-EventQueue-0" [_thread_in_native, id=11444, stack(0x0000000034100000,0x0000000034400000)]
  0x0000000033c27800 JavaThread "TimerQueue" daemon [_thread_blocked, id=7720, stack(0x0000000033e00000,0x0000000034100000)]
  0x000000003052b000 JavaThread "AWT-Windows" daemon [_thread_in_native, id=5564, stack(0x0000000030bd0000,0x0000000030ed0000)]
  0x000000003052c800 JavaThread "AWT-Shutdown" [_thread_blocked, id=11500, stack(0x00000000308d0000,0x0000000030bd0000)]
  0x000000003052d800 JavaThread "Java2D Disposer" daemon [_thread_blocked, id=7304, stack(0x00000000305d0000,0x00000000308d0000)]
  0x0000000025ee3000 JavaThread "Service Thread" daemon [_thread_blocked, id=6192, stack(0x000000002d460000,0x000000002d760000)]
  0x0000000025ec1000 JavaThread "C1 CompilerThread3" daemon [_thread_blocked, id=1892, stack(0x000000002d360000,0x000000002d460000)]
  0x0000000025ec2800 JavaThread "C2 CompilerThread2" daemon [_thread_blocked, id=8812, stack(0x000000002d260000,0x000000002d360000)]
  0x0000000025e81000 JavaThread "C2 CompilerThread1" daemon [_thread_blocked, id=9888, stack(0x000000002d160000,0x000000002d260000)]
  0x0000000025e83000 JavaThread "C2 CompilerThread0" daemon [_thread_blocked, id=6956, stack(0x000000002d060000,0x000000002d160000)]
  0x0000000025e85000 JavaThread "Attach Listener" daemon [_thread_blocked, id=3352, stack(0x000000002cd60000,0x000000002d060000)]
  0x000000002c0b1800 JavaThread "Signal Dispatcher" daemon [_thread_blocked, id=11268, stack(0x000000002ca60000,0x000000002cd60000)]
  0x000000002c0b3800 JavaThread "Surrogate Locker Thread (Concurrent GC)" daemon [_thread_blocked, id=10480, stack(0x000000002c760000,0x000000002ca60000)]
  0x00000000250e1000 JavaThread "Finalizer" daemon [_thread_blocked, id=6536, stack(0x000000002c460000,0x000000002c760000)]
  0x00000000250e3000 JavaThread "Reference Handler" daemon [_thread_blocked, id=10560, stack(0x000000002c160000,0x000000002c460000)]
  0x000000001e3e7800 JavaThread "main" [_thread_blocked, id=11504, stack(0x000000001e4c0000,0x000000001e5c0000)]

Other Threads:
  0x00000000250d4800 VMThread [stack: 0x000000002bf60000,0x000000002c060000] [id=10036]
  0x0000000025ee1800 WatcherThread [stack: 0x000000002d760000,0x000000002d860000] [id=8716]

VM state:not at safepoint (normal execution)

VM Mutex/Monitor currently owned by a thread: None

Heap
 par new generation   total 55296K, used 38826K [0x0000000730000000, 0x0000000733c00000, 0x0000000733c00000)
  eden space 49152K,  73% used [0x0000000730000000, 0x000000073236cfb8, 0x0000000733000000)
  from space 6144K,  41% used [0x0000000733600000, 0x000000073387dbc8, 0x0000000733c00000)
  to   space 6144K,   0% used [0x0000000733000000, 0x0000000733000000, 0x0000000733600000)
 concurrent mark-sweep generation total 102300K, used 64631K [0x0000000733c00000, 0x0000000739fe7000, 0x00000007f0000000)
 concurrent-mark-sweep perm gen total 262144K, used 58444K [0x00000007f0000000, 0x0000000800000000, 0x0000000800000000)

Card table byte_map: [0x0000000025160000,0x00000000257f0000] byte_map_base: 0x00000000217e0000

Polling page: 0x000000001e5c0000

Code Cache  [0x000000001e5e0000, 0x0000000020200000, 0x00000000245e0000)
 total_blobs=7995 nmethods=7230 adapters=680 free_code_cache=69750Kb largest_free_block=71205696

Compilation events (10 events):
Event: 94.711 Thread 0x0000000025ec2800 9317   !   4       javax.swing.TimerQueue::containsTimer (45 bytes)
Event: 94.720 Thread 0x0000000025ec2800 nmethod 9317 0x000000001f7d7890 code [0x000000001f7d7a20, 0x000000001f7d7d10]
Event: 94.732 Thread 0x0000000025e81000 9318       4       java.util.ArrayList::isEmpty (13 bytes)
Event: 94.733 Thread 0x0000000025e81000 nmethod 9318 0x000000001fc3dd90 code [0x000000001fc3dec0, 0x000000001fc3df38]
Event: 94.736 Thread 0x0000000025ec1000 9319       3       com.jidesoft.grid.TreeTableModel::aat (13 bytes)
Event: 94.737 Thread 0x0000000025ec1000 nmethod 9319 0x000000001ec81650 code [0x000000001ec81800, 0x000000001ec81d38]
Event: 94.741 Thread 0x0000000025ec1000 9320       3       javax.swing.DefaultListSelectionModel::set (50 bytes)
Event: 94.742 Thread 0x0000000025ec1000 nmethod 9320 0x000000001ec80cd0 code [0x000000001ec80e80, 0x000000001ec81438]
Event: 94.742 Thread 0x0000000025ec1000 9321       3       javax.swing.JComboBox::setSelectedItem (138 bytes)
Event: 94.744 Thread 0x0000000025ec1000 nmethod 9321 0x000000001f7d6910 code [0x000000001f7d6b20, 0x000000001f7d7558]

GC Heap History (10 events):
Event: 53.403 GC heap before
{Heap before GC invocations=18 (full 6):
 par new generation   total 55296K, used 23454K [0x0000000730000000, 0x0000000733c00000, 0x0000000733c00000)
  eden space 49152K,  39% used [0x0000000730000000, 0x000000073131f520, 0x0000000733000000)
  from space 6144K,  63% used [0x0000000733600000, 0x00000007339c86b8, 0x0000000733c00000)
  to   space 6144K,   0% used [0x0000000733000000, 0x0000000733000000, 0x0000000733600000)
 concurrent mark-sweep generation total 93496K, used 61958K [0x0000000733c00000, 0x000000073974e000, 0x00000007f0000000)
 concurrent-mark-sweep perm gen total 262144K, used 53005K [0x00000007f0000000, 0x0000000800000000, 0x0000000800000000)
Event: 54.092 GC heap after
Heap after GC invocations=19 (full 7):
 par new generation   total 55296K, used 0K [0x0000000730000000, 0x0000000733c00000, 0x0000000733c00000)
  eden space 49152K,   0% used [0x0000000730000000, 0x0000000730000000, 0x0000000733000000)
  from space 6144K,   0% used [0x0000000733600000, 0x0000000733600000, 0x0000000733c00000)
  to   space 6144K,   0% used [0x0000000733000000, 0x0000000733000000, 0x0000000733600000)
 concurrent mark-sweep generation total 102300K, used 61379K [0x0000000733c00000, 0x0000000739fe7000, 0x00000007f0000000)
 concurrent-mark-sweep perm gen total 262144K, used 52979K [0x00000007f0000000, 0x0000000800000000, 0x0000000800000000)
}
Event: 87.327 GC heap before
{Heap before GC invocations=19 (full 7):
 par new generation   total 55296K, used 49152K [0x0000000730000000, 0x0000000733c00000, 0x0000000733c00000)
  eden space 49152K, 100% used [0x0000000730000000, 0x0000000733000000, 0x0000000733000000)
  from space 6144K,   0% used [0x0000000733600000, 0x0000000733600000, 0x0000000733c00000)
  to   space 6144K,   0% used [0x0000000733000000, 0x0000000733000000, 0x0000000733600000)
 concurrent mark-sweep generation total 102300K, used 61379K [0x0000000733c00000, 0x0000000739fe7000, 0x00000007f0000000)
 concurrent-mark-sweep perm gen total 262144K, used 53125K [0x00000007f0000000, 0x0000000800000000, 0x0000000800000000)
Event: 87.335 GC heap after
Heap after GC invocations=20 (full 7):
 par new generation   total 55296K, used 2286K [0x0000000730000000, 0x0000000733c00000, 0x0000000733c00000)
  eden space 49152K,   0% used [0x0000000730000000, 0x0000000730000000, 0x0000000733000000)
  from space 6144K,  37% used [0x0000000733000000, 0x000000073323bb58, 0x0000000733600000)
  to   space 6144K,   0% used [0x0000000733600000, 0x0000000733600000, 0x0000000733c00000)
 concurrent mark-sweep generation total 102300K, used 61379K [0x0000000733c00000, 0x0000000739fe7000, 0x00000007f0000000)
 concurrent-mark-sweep perm gen total 262144K, used 53125K [0x00000007f0000000, 0x0000000800000000, 0x0000000800000000)
}
Event: 91.318 GC heap before
{Heap before GC invocations=20 (full 7):
 par new generation   total 55296K, used 51438K [0x0000000730000000, 0x0000000733c00000, 0x0000000733c00000)
  eden space 49152K, 100% used [0x0000000730000000, 0x0000000733000000, 0x0000000733000000)
  from space 6144K,  37% used [0x0000000733000000, 0x000000073323bb58, 0x0000000733600000)
  to   space 6144K,   0% used [0x0000000733600000, 0x0000000733600000, 0x0000000733c00000)
 concurrent mark-sweep generation total 102300K, used 61379K [0x0000000733c00000, 0x0000000739fe7000, 0x00000007f0000000)
 concurrent-mark-sweep perm gen total 262144K, used 54760K [0x00000007f0000000, 0x0000000800000000, 0x0000000800000000)
Event: 91.328 GC heap after
Heap after GC invocations=21 (full 7):
 par new generation   total 55296K, used 4913K [0x0000000730000000, 0x0000000733c00000, 0x0000000733c00000)
  eden space 49152K,   0% used [0x0000000730000000, 0x0000000730000000, 0x0000000733000000)
  from space 6144K,  79% used [0x0000000733600000, 0x0000000733acc6e0, 0x0000000733c00000)
  to   space 6144K,   0% used [0x0000000733000000, 0x0000000733000000, 0x0000000733600000)
 concurrent mark-sweep generation total 102300K, used 61379K [0x0000000733c00000, 0x0000000739fe7000, 0x00000007f0000000)
 concurrent-mark-sweep perm gen total 262144K, used 54760K [0x00000007f0000000, 0x0000000800000000, 0x0000000800000000)
}
Event: 92.363 GC heap before
{Heap before GC invocations=21 (full 7):
 par new generation   total 55296K, used 54065K [0x0000000730000000, 0x0000000733c00000, 0x0000000733c00000)
  eden space 49152K, 100% used [0x0000000730000000, 0x0000000733000000, 0x0000000733000000)
  from space 6144K,  79% used [0x0000000733600000, 0x0000000733acc6e0, 0x0000000733c00000)
  to   space 6144K,   0% used [0x0000000733000000, 0x0000000733000000, 0x0000000733600000)
 concurrent mark-sweep generation total 102300K, used 61379K [0x0000000733c00000, 0x0000000739fe7000, 0x00000007f0000000)
 concurrent-mark-sweep perm gen total 262144K, used 54841K [0x00000007f0000000, 0x0000000800000000, 0x0000000800000000)
Event: 92.378 GC heap after
Heap after GC invocations=22 (full 7):
 par new generation   total 55296K, used 3554K [0x0000000730000000, 0x0000000733c00000, 0x0000000733c00000)
  eden space 49152K,   0% used [0x0000000730000000, 0x0000000730000000, 0x0000000733000000)
  from space 6144K,  57% used [0x0000000733000000, 0x00000007333789f0, 0x0000000733600000)
  to   space 6144K,   0% used [0x0000000733600000, 0x0000000733600000, 0x0000000733c00000)
 concurrent mark-sweep generation total 102300K, used 64631K [0x0000000733c00000, 0x0000000739fe7000, 0x00000007f0000000)
 concurrent-mark-sweep perm gen total 262144K, used 54841K [0x00000007f0000000, 0x0000000800000000, 0x0000000800000000)
}
Event: 93.458 GC heap before
{Heap before GC invocations=22 (full 7):
 par new generation   total 55296K, used 52706K [0x0000000730000000, 0x0000000733c00000, 0x0000000733c00000)
  eden space 49152K, 100% used [0x0000000730000000, 0x0000000733000000, 0x0000000733000000)
  from space 6144K,  57% used [0x0000000733000000, 0x00000007333789f0, 0x0000000733600000)
  to   space 6144K,   0% used [0x0000000733600000, 0x0000000733600000, 0x0000000733c00000)
 concurrent mark-sweep generation total 102300K, used 64631K [0x0000000733c00000, 0x0000000739fe7000, 0x00000007f0000000)
 concurrent-mark-sweep perm gen total 262144K, used 55633K [0x00000007f0000000, 0x0000000800000000, 0x0000000800000000)
Event: 93.467 GC heap after
Heap after GC invocations=23 (full 7):
 par new generation   total 55296K, used 2550K [0x0000000730000000, 0x0000000733c00000, 0x0000000733c00000)
  eden space 49152K,   0% used [0x0000000730000000, 0x0000000730000000, 0x0000000733000000)
  from space 6144K,  41% used [0x0000000733600000, 0x000000073387dbc8, 0x0000000733c00000)
  to   space 6144K,   0% used [0x0000000733000000, 0x0000000733000000, 0x0000000733600000)
 concurrent mark-sweep generation total 102300K, used 64631K [0x0000000733c00000, 0x0000000739fe7000, 0x00000007f0000000)
 concurrent-mark-sweep perm gen total 262144K, used 55633K [0x00000007f0000000, 0x0000000800000000, 0x0000000800000000)
}

Deoptimization events (10 events):
Event: 93.743 Thread 0x0000000033c81000 Uncommon trap: reason=class_check action=maybe_recompile pc=0x000000001f436d88 method=java.util.HashMap.putForCreate(Ljava/lang/Object;Ljava/lang/Object;)V @ 114
Event: 93.743 Thread 0x0000000033c81000 Uncommon trap: reason=class_check action=maybe_recompile pc=0x000000001f436d88 method=java.util.HashMap.putForCreate(Ljava/lang/Object;Ljava/lang/Object;)V @ 114
Event: 93.744 Thread 0x0000000033c81000 Uncommon trap: reason=class_check action=maybe_recompile pc=0x000000001f436d88 method=java.util.HashMap.putForCreate(Ljava/lang/Object;Ljava/lang/Object;)V @ 114
Event: 93.769 Thread 0x0000000033c81000 Uncommon trap: reason=class_check action=maybe_recompile pc=0x000000001eda1ab8 method=java.util.HashMap.putForCreate(Ljava/lang/Object;Ljava/lang/Object;)V @ 114
Event: 93.798 Thread 0x0000000033c81000 Uncommon trap: reason=unreached action=reinterpret pc=0x000000001ec6da54 method=javax.swing.JLabel.setText(Ljava/lang/String;)V @ 87
Event: 94.266 Thread 0x0000000033c81000 Uncommon trap: reason=unreached action=reinterpret pc=0x000000001fa9e208 method=sun.swing.SwingUtilities2.getLeftSideBearing(Ljavax/swing/JComponent;Ljava/awt/FontMetrics;C)I @ 126
Event: 94.516 Thread 0x0000000033c81000 Uncommon trap: reason=unreached action=reinterpret pc=0x000000001fc66b24 method=javax.swing.JComponent.paintChildren(Ljava/awt/Graphics;)V @ 447
Event: 94.516 Thread 0x0000000033c81000 Uncommon trap: reason=unreached action=reinterpret pc=0x000000001fc66b24 method=javax.swing.JComponent.paintChildren(Ljava/awt/Graphics;)V @ 447
Event: 94.593 Thread 0x0000000033c81000 Uncommon trap: reason=unreached action=reinterpret pc=0x000000001e8faff4 method=sun.java2d.SunGraphics2D.setRenderingHint(Ljava/awt/RenderingHints$Key;Ljava/lang/Object;)V @ 482
Event: 94.598 Thread 0x0000000033c81000 Uncommon trap: reason=null_check action=make_not_entrant pc=0x000000001e6fbe74 method=java.awt.geom.AffineTransform.equals(Ljava/lang/Object;)Z @ 1

Internal exceptions (10 events):
Event: 94.472 Thread 0x0000000033c81000 Threw 0x0000000731bb98b8 at C:\jdk7u2_64p\jdk7u40\hotspot\src\share\vm\prims\jvm.cpp:1244
Event: 94.473 Thread 0x0000000033c81000 Threw 0x0000000731bc48f0 at C:\jdk7u2_64p\jdk7u40\hotspot\src\share\vm\prims\jvm.cpp:1244
Event: 94.474 Thread 0x0000000033c81000 Threw 0x0000000731bca5e0 at C:\jdk7u2_64p\jdk7u40\hotspot\src\share\vm\prims\jvm.cpp:1244
Event: 94.474 Thread 0x0000000033c81000 Threw 0x0000000731bcd3a0 at C:\jdk7u2_64p\jdk7u40\hotspot\src\share\vm\prims\jvm.cpp:1244
Event: 94.474 Thread 0x0000000033c81000 Threw 0x0000000731bcffc8 at C:\jdk7u2_64p\jdk7u40\hotspot\src\share\vm\prims\jvm.cpp:1244
Event: 94.477 Thread 0x0000000033c81000 Threw 0x0000000731bdfee8 at C:\jdk7u2_64p\jdk7u40\hotspot\src\share\vm\prims\jvm.cpp:1244
Event: 94.595 Thread 0x0000000033c81000 Threw 0x0000000731f715c0 at C:\jdk7u2_64p\jdk7u40\hotspot\src\share\vm\prims\jvm.cpp:1244
Event: 94.597 Thread 0x0000000033c81000 Threw 0x00000007321bfcc8 at C:\jdk7u2_64p\jdk7u40\hotspot\src\share\vm\prims\jvm.cpp:1244
Event: 94.598 Thread 0x0000000033c81000 Implicit null exception at 0x000000001e6fbdcc to 0x000000001e6fbe65
Event: 94.601 Thread 0x0000000033c81000 Threw 0x00000007321d3628 at C:\jdk7u2_64p\jdk7u40\hotspot\src\share\vm\prims\jvm.cpp:1244

Events (10 events):
Event: 94.598 Thread 0x0000000033c81000 DEOPT PACKING pc=0x000000001e6fbe74 sp=0x00000000343fb450
Event: 94.598 Thread 0x0000000033c81000 DEOPT UNPACKING pc=0x000000001e619064 sp=0x00000000343fb3e0 mode 2
Event: 94.600 loading class 0x000000001e488680
Event: 94.600 loading class 0x000000001e488680 done
Event: 94.600 loading class 0x000000001e488750
Event: 94.601 loading class 0x0000000040a4f470
Event: 94.601 loading class 0x0000000040a4f470 done
Event: 94.601 loading class 0x000000001e488750 done
Event: 94.601 loading class 0x000000003cf4b6c0
Event: 94.601 loading class 0x000000003cf4b6c0 done


Dynamic libraries:
0x0000000140000000 - 0x000000014003b000 	G:\Xilinx\Vivado\2013.4\bin\unwrapped\win64.o\vivado.exe
0x00000000779a0000 - 0x0000000077b49000 	C:\Windows\SYSTEM32\ntdll.dll
0x0000000077780000 - 0x000000007789f000 	C:\Windows\system32\kernel32.dll
0x000007fefd800000 - 0x000007fefd86b000 	C:\Windows\system32\KERNELBASE.dll
0x000000000a900000 - 0x000000000a945000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\SHSMP64.dll
0x00000000778a0000 - 0x000000007799a000 	C:\Windows\system32\USER32.dll
0x000007fefe1b0000 - 0x000007fefe217000 	C:\Windows\system32\GDI32.dll
0x000007feffc00000 - 0x000007feffc0e000 	C:\Windows\system32\LPK.dll
0x000007fefeab0000 - 0x000007fefeb79000 	C:\Windows\system32\USP10.dll
0x000007fefe220000 - 0x000007fefe2bf000 	C:\Windows\system32\msvcrt.dll
0x000007fefe4c0000 - 0x000007fefe59b000 	C:\Windows\system32\ADVAPI32.dll
0x000007feff9a0000 - 0x000007feff9bf000 	C:\Windows\SYSTEM32\sechost.dll
0x000007feffad0000 - 0x000007feffbfd000 	C:\Windows\system32\RPCRT4.dll
0x000007fefc890000 - 0x000007fefc89c000 	C:\Windows\system32\VERSION.dll
0x0000000180000000 - 0x0000000180013000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\libboost_signals.dll
0x00000000001e0000 - 0x00000000002ce000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\stlport.5.2.dll
0x000000006c3d0000 - 0x000000006c4a3000 	C:\Windows\WinSxS\amd64_microsoft.vc90.crt_1fc8b3b9a1e18e3b_9.0.30729.6161_none_08e61857a83bc251\MSVCP90.dll
0x000000006e700000 - 0x000000006e7a3000 	C:\Windows\WinSxS\amd64_microsoft.vc90.crt_1fc8b3b9a1e18e3b_9.0.30729.6161_none_08e61857a83bc251\MSVCR90.dll
0x0000000000410000 - 0x0000000000dfb000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_common.dll
0x0000000000e00000 - 0x00000000010e9000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\libCOIN-all.dll
0x0000000000300000 - 0x0000000000310000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\libboost_date_time.dll
0x0000000001100000 - 0x0000000001127000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\libboost_filesystem.dll
0x0000000001140000 - 0x0000000001149000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\libboost_system.dll
0x0000000001160000 - 0x00000000011d1000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\libboost_program_options.dll
0x00000000011f0000 - 0x00000000012a1000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\libboost_regex.dll
0x00000000012c0000 - 0x00000000012de000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\libboost_thread.dll
0x00000000012f0000 - 0x00000000012fc000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\libboost_chrono.dll
0x0000000001310000 - 0x0000000001353000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\libcurl.dll
0x000007fefe7b0000 - 0x000007fefe7fd000 	C:\Windows\system32\WS2_32.dll
0x000007feff990000 - 0x000007feff998000 	C:\Windows\system32\NSI.dll
0x000007fefe5d0000 - 0x000007fefe622000 	C:\Windows\system32\WLDAP32.dll
0x0000000001360000 - 0x00000000013e3000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\libhdlpsolve.dll
0x0000000001400000 - 0x00000000014b7000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\libhdxml.dll
0x00000000014d0000 - 0x0000000001ab9dbc 	G:\Xilinx\Vivado\2013.4\lib\win64.o\libisl_iostreams.dll
0x0000000001ad0000 - 0x0000000001aea000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\libboost_iostreams.dll
0x0000000001b00000 - 0x0000000001b23000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdizlib.dll
0x0000000001b40000 - 0x0000000001b5e000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\libisl_iosutils.dll
0x0000000001b70000 - 0x0000000001b99000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\libisl_sysinfo.dll
0x000000006a440000 - 0x000000006ac09000 	G:\Xilinx\Vivado\2013.4\tps\win64\jre\bin\server\jvm.dll
0x000007fef7ad0000 - 0x000007fef7ad9000 	C:\Windows\system32\WSOCK32.dll
0x000007fefb560000 - 0x000007fefb59b000 	C:\Windows\system32\WINMM.dll
0x0000000077b70000 - 0x0000000077b77000 	C:\Windows\system32\PSAPI.DLL
0x000000006c2f0000 - 0x000000006c3c2000 	C:\Windows\system32\MSVCR100.dll
0x0000000001bc0000 - 0x0000000001bd5000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\pthreadVC2.dll
0x0000000001be0000 - 0x0000000001c31000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_commonxillic.dll
0x000007feea620000 - 0x000007feea80e000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\libXil_lmgr11.dll
0x000007fefaa70000 - 0x000007fefaa86000 	C:\Windows\system32\NETAPI32.dll
0x000007fefaa60000 - 0x000007fefaa6c000 	C:\Windows\system32\netutils.dll
0x000007fefd2a0000 - 0x000007fefd2c3000 	C:\Windows\system32\srvcli.dll
0x000007fefaa40000 - 0x000007fefaa55000 	C:\Windows\system32\wkscli.dll
0x000007fefe420000 - 0x000007fefe4b7000 	C:\Windows\system32\COMDLG32.dll
0x000007feffc10000 - 0x000007feffc81000 	C:\Windows\system32\SHLWAPI.dll
0x000007feed880000 - 0x000007feed920000 	C:\Windows\WinSxS\amd64_microsoft.windows.common-controls_6595b64144ccf1df_5.82.7601.18201_none_a4d3b9377117c3df\COMCTL32.dll
0x000007fefec00000 - 0x000007feff988000 	C:\Windows\system32\SHELL32.dll
0x000007fefe630000 - 0x000007fefe707000 	C:\Windows\system32\OLEAUT32.dll
0x000007fefdd60000 - 0x000007fefdf63000 	C:\Windows\system32\ole32.dll
0x000007fefd9e0000 - 0x000007fefda1a000 	C:\Windows\system32\WINTRUST.dll
0x000007fefd870000 - 0x000007fefd9dc000 	C:\Windows\system32\CRYPT32.dll
0x000007fefd7f0000 - 0x000007fefd7ff000 	C:\Windows\system32\MSASN1.dll
0x0000000001c50000 - 0x0000000001c66000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdiconfig.dll
0x0000000010000000 - 0x000000001012a000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\tcl85t.dll
0x0000000012000000 - 0x0000000012282000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\xerces-c_3_1.dll
0x000007fefdf70000 - 0x000007fefe1b0000 	C:\Windows\system32\WININET.dll
0x000007fefdac0000 - 0x000007fefdac4000 	C:\Windows\system32\api-ms-win-downlevel-user32-l1-1-0.dll
0x000007fefdaa0000 - 0x000007fefdaa4000 	C:\Windows\system32\api-ms-win-downlevel-shlwapi-l1-1-0.dll
0x000007fefda90000 - 0x000007fefda94000 	C:\Windows\system32\api-ms-win-downlevel-version-l1-1-0.dll
0x000007fefdad0000 - 0x000007fefdad3000 	C:\Windows\system32\api-ms-win-downlevel-normaliz-l1-1-0.dll
0x0000000077b60000 - 0x0000000077b63000 	C:\Windows\system32\normaliz.DLL
0x000007fefe800000 - 0x000007fefeaa9000 	C:\Windows\system32\iertutil.dll
0x000007fefda80000 - 0x000007fefda85000 	C:\Windows\system32\api-ms-win-downlevel-advapi32-l1-1-0.dll
0x000007fef9bb0000 - 0x000007fef9c21000 	C:\Windows\system32\WINHTTP.dll
0x000007fef9b40000 - 0x000007fef9ba4000 	C:\Windows\system32\webio.dll
0x000007fefe2c0000 - 0x000007fefe41f000 	C:\Windows\system32\urlmon.dll
0x000007fefdab0000 - 0x000007fefdab4000 	C:\Windows\system32\api-ms-win-downlevel-ole32-l1-1-0.dll
0x000000006e4c0000 - 0x000000006e4d1000 	C:\Windows\WinSxS\amd64_microsoft.vc90.openmp_1fc8b3b9a1e18e3b_9.0.30729.6161_none_390d35aa0a1f21f9\VCOMP90.DLL
0x0000000001ca0000 - 0x0000000001cb2000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_commonmain.dll
0x0000000001cd0000 - 0x0000000001cd7000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_commonversion.dll
0x000007fefe5a0000 - 0x000007fefe5ce000 	C:\Windows\system32\IMM32.DLL
0x000007feff9c0000 - 0x000007feffac9000 	C:\Windows\system32\MSCTF.dll
0x0000000005420000 - 0x00000000058a0000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_commontasks.dll
0x0000000006210000 - 0x000000000689c000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_coretasks.dll
0x00000000068a0000 - 0x0000000006a9d000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_chipscope.dll
0x0000000006aa0000 - 0x0000000006b0f000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\liblmx6.0.dll
0x0000000006b10000 - 0x0000000007c0c000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_constraints.dll
0x0000000007c10000 - 0x000000000a146000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_device.dll
0x000000000a150000 - 0x000000000a1ce000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\libboost_serialization.dll
0x000000000a950000 - 0x000000000b0f1000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\libverific.dll
0x000000000a1d0000 - 0x000000000a5f0000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_netlist.dll
0x000000000b100000 - 0x000000000b547000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_psta.dll
0x000000000b550000 - 0x000000000eda6000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_designutils.dll
0x000000000a5f0000 - 0x000000000a8c4000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_bitstream.dll
0x000000000edb0000 - 0x000000000f2f4000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_xdm.dll
0x000000000f300000 - 0x000000000f731000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_drc.dll
0x0000000010130000 - 0x0000000010a51000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_timing.dll
0x000000000f740000 - 0x000000000f943000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_dlyest.dll
0x000000000f950000 - 0x000000000f9ef000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\libise.dll
0x000000000f9f0000 - 0x000000000fce1000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_filemgmt.dll
0x0000000012290000 - 0x0000000013ae3000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_coregen.dll
0x0000000010a60000 - 0x0000000011236000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_coregenipxact.dll
0x0000000013af0000 - 0x0000000015092000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_place.dll
0x0000000011240000 - 0x000000001181e000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_abc_nomp.dll
0x000000000fd10000 - 0x000000000fd2a000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_hmetis.dll
0x0000000011820000 - 0x0000000011df9000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_power.dll
0x00000000150a0000 - 0x000000001589a000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_route.dll
0x00000000158a0000 - 0x0000000015d94000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_project.dll
0x000000000fd70000 - 0x000000000fda2000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_board.dll
0x0000000015da0000 - 0x00000000162c2000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_labtools.dll
0x00000000162d0000 - 0x0000000016742000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_wavedata.dll
0x000000000fde0000 - 0x000000000fe1d000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_simbridge_kernel.dll
0x000000000fe30000 - 0x000000000fe4f000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_wavedata_SimpleApi.dll
0x000000000fe60000 - 0x000000000fe94000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_xicom_sci.dll
0x0000000016750000 - 0x0000000016cfa000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_memdata.dll
0x0000000016d00000 - 0x000000001740c000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_rsb.dll
0x0000000017410000 - 0x00000000180c3000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_ip.dll
0x000000000fee0000 - 0x000000000ff13000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_bmg.dll
0x00000000180d0000 - 0x00000000184e7000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_runs.dll
0x00000000184f0000 - 0x0000000019e02000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_synth.dll
0x000000001ae10000 - 0x000000001cd03000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_tcltasks.dll
0x000000001cd10000 - 0x000000001cde4000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_dsp.dll
0x000000000ff70000 - 0x000000000ffe0000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_edk.dll
0x000000001cdf0000 - 0x000000001d00b000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_simdata.dll
0x000000001d510000 - 0x000000001d764000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_vivadotasks.dll
0x000000001d780000 - 0x000000001dbe7000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_implflow.dll
0x000000001dc00000 - 0x000000001df83000 	G:\Xilinx\Vivado\2013.4\lib\win64.o\librdi_pwropt.dll
0x000000006e4b0000 - 0x000000006e4bf000 	G:\Xilinx\Vivado\2013.4\tps\win64\jre\bin\verify.dll
0x000000006e480000 - 0x000000006e4a8000 	G:\Xilinx\Vivado\2013.4\tps\win64\jre\bin\java.dll
0x000000006e460000 - 0x000000006e475000 	G:\Xilinx\Vivado\2013.4\tps\win64\jre\bin\zip.dll
0x000000006e440000 - 0x000000006e459000 	G:\Xilinx\Vivado\2013.4\tps\win64\jre\bin\net.dll

VM Arguments:
jvm_args: -Dsun.java2d.pmoffscreen=false -Xverify:none -Dswing.aatext=true -XX:-UsePerfData -Djdk.map.althashing.threshold=512 -XX:StringTableSize=4072 -Djava.util.Arrays.useLegacyMergeSort=true -XX:PermSize=256m -XX:MaxPermSize=256m -XX:NewSize=60m -XX:MaxNewSize=60m -XX:+UseConcMarkSweepGC -XX:+UseParNewGC -XX:+CMSParallelRemarkEnabled -XX:+CMSScavengeBeforeRemark -XX:+UseNUMA -XX:+AggressiveOpts -XX:+UseFastAccessorMethods -XX:+UseFastEmptyMethods -XX:+UseBiasedLocking -XX:+TieredCompilation -Xms128m -Xmx3072m -Xss3m 
java_command: <unknown>
Launcher Type: generic

Environment Variables:
PATH=G:/Xilinx/Vivado/2013.4/bin;G:/Xilinx/Vivado/2013.4/lib/win64.o;G:/Xilinx/Vivado/2013.4/tps/win64/jre/bin/server;G:/Xilinx/Vivado/2013.4/tps/win64/jre/bin;G:/Xilinx/SDK/2013.4/bin/nt64;G:/Xilinx/Vivado/2013.4/ids_lite/EDK/bin/nt64;G:/Xilinx/Vivado/2013.4/ids_lite/EDK/lib/nt64;G:/Xilinx/Vivado/2013.4/ids_lite/ISE/bin/nt64;G:/Xilinx/Vivado/2013.4/ids_lite/ISE/lib/nt64;G:\Tools\DesignPlayer\bin;G:\Cygwin\bin;G:\Cygwin\opt\ghdl\bin;g:\tools\imagemagick-6.2.8-q16;G:\Tools\scala\bin;C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\;C:\Program Files (x86)\ATI Technologies\ATI.ACE\Core-Static;G:\Tools\doxygen\bin;C:\Program Files (x86)\JustSystems\JSLIB32;G:\altera\13.0sp1\modelsim_ase\win32aloem
USERNAME=XXXXX
OS=Windows_NT
PROCESSOR_IDENTIFIER=Intel64 Family 6 Model 30 Stepping 5, GenuineIntel



---------------  S Y S T E M  ---------------

OS: Windows 7 , 64 bit Build 7601 Service Pack 1

CPU:total 8 (4 cores per cpu, 2 threads per core) family 6 model 30 stepping 5, cmov, cx8, fxsr, mmx, sse, sse2, sse3, ssse3, sse4.1, sse4.2, popcnt, ht, tsc, tscinvbit

Memory: 4k page, physical 8379444k(6394800k free), swap 16757024k(13137792k free)

vm_info: Java HotSpot(TM) 64-Bit Server VM (24.0-b56) for windows-amd64 JRE (1.7.0_40-b43), built on Aug 26 2013 22:38:32 by "java_re" with unknown MS VC++:1600

time: Tue Apr 01 19:49:17 2014
elapsed time: 94 seconds

