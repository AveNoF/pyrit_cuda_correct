# pyrit_cuda_correct
This is pyrit cuda module which I removed error of oiginal version(original version is here:https://github.com/JPaulMora/Pyrit).


[Executing '/usr/local/cuda/bin/nvcc -m64 C -Xcompiler "-fPIC" --ptx ./_cpyrit_cudakernel.cu'
nvcc warning : The 'compute_20', 'sm_20', and 'sm_21' architectures are deprecated, and may be removed in a future release (Use -Wno-deprecated-gpu-targets to suppress warning).
nvcc fatal   : Don't know what to do with 'C'
Traceback (most recent call last):
  File "setup.py", line 166, in <module>
    setup(**setup_args)
  File "/usr/lib/python2.7/distutils/core.py", line 151, in setup
    dist.run_commands()
  File "/usr/lib/python2.7/distutils/dist.py", line 953, in run_commands
    self.run_command(cmd)
  File "/usr/lib/python2.7/distutils/dist.py", line 972, in run_command
    cmd_obj.run()
  File "/usr/lib/python2.7/distutils/command/build.py", line 128, in run
    self.run_command(cmd_name)
  File "/usr/lib/python2.7/distutils/cmd.py", line 326, in run_command
    self.distribution.run_command(command)
  File "/usr/lib/python2.7/distutils/dist.py", line 972, in run_command
    cmd_obj.run()
  File "setup.py", line 91, in run
    subprocess.check_call(nvcc_cmd, shell=True)
  File "/usr/lib/python2.7/subprocess.py", line 541, in check_call
    raise CalledProcessError(retcode, cmd)
subprocess.CalledProcessError: Command '/usr/local/cuda/bin/nvcc -m64 C -Xcompiler "-fPIC" --ptx ./_cpyrit_cudakernel.cu' returned non-zero exit status 1]

The original version has such a compile error inspite of appropriate environment.
