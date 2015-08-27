# CUDA
* AWS instance for GPU computing:
  1. Setup G2 EC2 instance with LINUX 
  2. Generate key-pair
  3. Add the pub-key to local machine
  4. chmod 400 <pub-key>.pem
  5. enable the inbound port for remote login on this instance for the instance group-key
  6. ssh login to the EC2 instance
  7. sudo yum update -y
  8.  sudo reboot
  9.  sudo yum groupinstall -y "Development tools"
  10.  sudo yum install kernel-devel-`uname -r`
  11.  wget http://us.download.nvidia.com/XFree86/Linux-x86_64/340.46/NVIDIA-Linux-x86_64-340.46.run
  12.  sudo /bin/bash ./NVIDIA-Linux-x86_64-340.46.run
  13.  nvidia-smi -q | head
