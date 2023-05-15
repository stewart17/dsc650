---
title: Assignment 1
subtitle: Computer performance, reliability, and scalability calculation
author: Stewart Wilson
---

## 1.2 

#### a. Data Sizes

| Data Item                                  | Size per Item | 
|--------------------------------------------|--------------:|
| 128 character message.                     | 128 Bytes     |
| 1024x768 PNG image                         | 0.47 MB       |
| 1024x768 RAW image                         | 2.36 MB       | 
| HD (1080p) HEVC Video (15 minutes)         | 167.96 MB     |
| HD (1080p) Uncompressed Video (15 minutes) | 167,961.6 MB  |
| 4K UHD HEVC Video (15 minutes)             | 671.85 MB     |
| 4k UHD Uncompressed Video (15 minutes)     | 671,846.4 MB  |
| Human Genome (Uncompressed)                | 200 GB        |

##### Explanations
- 128 character message: 1 byte per character x 128 = 128
- 1024x768 PNG image: 1024x768x24(true color)/5(PNG Compression Ratio) = 0.47
- 1024x768 RAW image: Same as above just don't do compression calculation
- HD (1080p) HEVC Video (15 minutes): 1920x1080x24(True color)x30(fps)x900(15minutes)/1000(HEVC Compression)=167mb
- HD (1080p) Uncompressed Video (15 minutes): Same as above just no compression
- 4K UHD HEVC Video (15 minutes):3840x2160x24x30x900/1000=671mb
- 4k UHD Uncompressed Video (15 minutes): Same as above just no compression
- Perfectly it'd  be 700mb (3bil 2bit pairs) but to actually sequence the genes it'd be closer to 200 [source](https://medium.com/precision-medicine/how-big-is-the-human-genome-e90caa3409b0)

#### b. Scaling

|                                           | Size            | # HD     | 
|-------------------------------------------|----------------:|---------:|
| Daily Twitter Tweets (Uncompressed)       | 178.8 GB        |  1       |
| Daily Twitter Tweets (Snappy Compressed)  | 105 GB          |  1       |
| Daily Instagram Photos                    | 675.9 TB        |  68      |
| Daily YouTube Videos                      | 481,201.17 TB   |48,121    |
| Yearly Twitter Tweets (Uncompressed)      | 63.7 TB         |  7       |
| Yearly Twitter Tweets (Snappy Compressed) | 37.47 GB        |  4       |
| Yearly Instagram Photos                   | 246,703.5 TB    |24,671    |
| Yearly YouTube Videos                     | 175,638,427.1 TB|17,563,843|

#### c. Reliability
|                                    | # HD         | # Failures |
|------------------------------------|-------------:|-----------:|
| Twitter Tweets (Uncompressed)      | 7            | .1         |
| Twitter Tweets (Snappy Compressed) | 4            | .05        |
| Instagram Photos                   | 24,671       | 338        |
| YouTube Videos                     | 17,563,843   | 240,625    |

#### d. Latency

|                           | One Way Latency      |
|---------------------------|---------------------:|
| Los Angeles to Amsterdam  | 75 ms                |
| Low Earth Orbit Satellite | 25 ms                |
| Geostationary Satellite   | 125 ms               |
| Earth to the Moon         | 1300 ms              |
| Earth to Mars             | 14.2 minutes        | 

##### Explanations
- 1 way latency [almost impossible](https://cs.stackexchange.com/questions/602/measuring-one-way-network-latency) to accurately find so i just divided round trip latency by 2
- [source for LA to amsterdam](https://wondernetwork.com/pings/Los%20Angeles/Amsterdam)
- [source for low earth orbit satellite](https://www.analog.com/en/analog-dialogue/articles/internet-from-space-rfic-in-high-capacity-low-latency-leo-satellite-terminals.html) 
- [geostationary](https://www.satsig.net/latency.htm) latency would be best when satellite directly overhead
-[fastest latency is 1250](https://space.stackexchange.com/questions/35590/what-is-the-lowest-latency-achievable-in-reliable-earth-moon-communications)
-earth to mars changes depending on position of planets. [currently](https://interimm.org/comms-latency/en/) it's 14 minutes
