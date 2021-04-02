# log-stress-test
A Docker container which does nothing but spew a large number of logs to stdout.

This project has two requirements:
1. Robustness to CPU pressure: Noisy neighbors should not impact the average volume of data logged. (temorary spikes in CPU usage should not impact the volume of data logged, measured over the course of about a minute)
2. Traceability: It should be possible to detect any lost log lines. This is achieved by starting each logged line with a sequence number.

