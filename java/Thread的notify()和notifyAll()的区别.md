# Thread的notify()和notifyAll()的区别?

notify()会随机唤醒被锁保护的对象的等待队列中的一个线程，将该线程从等待队列移至同步队列。获取到锁后才能从wait()方法返回。

notifyAll()会唤醒被锁保护的对象的等待队列中的全部线程，将全部线程从等待队列移至同步队列。但只有获取到锁的线程才能从wait()方法返回。