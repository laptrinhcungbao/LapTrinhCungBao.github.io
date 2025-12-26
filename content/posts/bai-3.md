---
title: "Bài 3: Kết nối MySQL bằng JDBC"
date: 2025-12-26T21:05:00+07:00
draft: false
---
JDBC là cầu nối giúp Java tương tác với các hệ quản trị CSDL như MySQL hay SQL Server.

```java
Connection conn = DriverManager.getConnection("jdbc:mysql://localhost:3306/db", "user", "pass");
Statement stmt = conn.createStatement();
ResultSet rs = stmt.executeQuery("SELECT * FROM students");