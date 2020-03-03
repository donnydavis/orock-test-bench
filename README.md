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

fio-plot and fio 3.14 were used to create the IOPS benchmark data
https://github.com/louwrentius/fio-plot

### Object Storage Benchmarks

Warp was used to create the object store benchmark data
