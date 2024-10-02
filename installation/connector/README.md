# Connector

### Kernel 파라미터 설정
1. Socket FD 수 제한 (open files)
   ```
   # 확인하기
   $ ulimit -n
   1024

   # 변경하기
   $ ulimit -n 1048576
   ```

2. Socket별 버퍼 크기 제한
   ```
   # 확인하기 (Ubuntu 22.04 기준)
   $ sysctl net.core.rmem_max
   $ sysctl net.core.wmem_max

   # 변경하기 (read/write buffer 각각 100MB)
   $ sysctl -w net.core.rmem_max=104857600
   $ sysctl -w net.core.wmem_max=104857600
   ```