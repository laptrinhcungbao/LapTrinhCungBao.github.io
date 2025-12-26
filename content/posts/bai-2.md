---
title: "Bài 2: Quản lý đa luồng (Multi-threading) trong Java"
date: 2025-12-26T21:00:00+07:00
draft: false
---
Đa luồng giúp ứng dụng Java xử lý nhiều công việc cùng lúc. Điều này cực kỳ quan trọng khi xây dựng Server để phục vụ nhiều Client.

```java
public class MyThread extends Thread {
    public void run() {
        System.out.println("Luồng đang chạy...");
    }
    public static void main(String[] args) {
        MyThread t1 = new MyThread();
        t1.start();
    }
}