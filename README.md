### These are the scripts used to create the benchmark numbers for OrockCloud


How to use

```git clone https://github.com/donnydavis/orock-test-bench
./bench-fio.sh fio-job-template-device.fio /home/cloud-user/benchmark-output/  none /dev/sdb none
```

How to get the graph outputs
```
fio_plot -i /home/cloud-user/benchmark-output/ -T "OrockCloud Random Read Benchmark" -s "Donny Davis" -L -t iops -r randread
fio_plot -i /home/cloud-user/benchmark-output/ -T "OrockCloud Random Read Benchmark" -s "Donny Davis" -L -t iops -r randwrite
```
