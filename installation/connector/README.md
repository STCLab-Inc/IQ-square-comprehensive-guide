# Connector

### Kernel 파라미터 설정
1. Socket FD 수 제한 (open files)
   ```
   # 확인하기
   $ ulimit -n
   1024

   # 변경하기 (세션)
   $ ulimit -n 1048576

   # 변경하기 (영구, root 권한 필요)
   $ echo "" > /etc/sysctl.d/90-apinf-socket-fd.conf
   $ echo "fs.nr_open=1048576" >> /etc/sysctl.d/90-apinf-socket-fd.conf
   $ sysctl -p
   ```

2. Socket별 버퍼 크기 제한
   ```
   # 확인하기 (Ubuntu 22.04 기준)
   $ sysctl net.core.rmem_max
   $ sysctl net.core.wmem_max

   # 변경하기 (세션, read/write buffer 각각 100MB)
   $ sysctl -w net.core.rmem_max=104857600
   $ sysctl -w net.core.wmem_max=104857600

   # 변경하기 (영구, root 권한 필요)
   $ echo "" > /etc/sysctl.d/90-apinf-socket-buffer.conf
   $ echo "net.core.rmem_max=104857600" >> /etc/sysctl.d/90-apinf-socket-buffer.conf
   $ echo "net.core.wmem_max=104857600" >> /etc/sysctl.d/90-apinf-socket-buffer.conf
   $ sysctl -p
   ```