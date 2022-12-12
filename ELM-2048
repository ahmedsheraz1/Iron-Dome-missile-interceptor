Python 3.10.2 (v3.10.2:a58ebcc701, Jan 13 2022, 14:50:16) [Clang 13.0.0 (clang-1300.0.29.30)] on darwin
Type "help", "copyright", "credits" or "license()" for more information.
import multiprocessing, time, signal
p = multiprocessing.Process(target=time.sleep, args=(1000,))
print(p, p.is_alive())
<Process name='Process-1' parent=11766 initial> False
p.start()
print(p, p.is_alive())
<Process name='Process-1' pid=11787 parent=11766 started> True
p.terminate()
time.sleep(0.1)
print(p, p.is_alive())
<Process name='Process-1' pid=11787 parent=11766 stopped exitcode=-SIGTERM> False
p.exitcode == -signal.SIGTERM
True
