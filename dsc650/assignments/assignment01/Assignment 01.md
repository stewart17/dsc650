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
| 1024x768 PNG image                         | 3.15 MB       |
| 1024x768 RAW image                         | 1.38 MB       | 
| HD (1080p) HEVC Video (15 minutes)         | 160 MB        |
| HD (1080p) Uncompressed Video (15 minutes) | 160,180 MB    |
| 4K UHD HEVC Video (15 minutes)             | 640 MB        |
| 4k UHD Uncompressed Video (15 minutes)     | 640,722 MB    |
| Human Genome (Uncompressed)                | 200 GB        |

##### Explanations
- 128 character message: 
- 1024

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
| Earth to Mars             | 11.99 minutes        | 

##### Explanations
