# centime

## Overview
This project centers on performance testing the jsonplaceholder.typicode API using JMeter. The primary goal was to assess response times,concurrency handling and measure overall system stability under varying load conditions.

## Contents 
- ** Test Plan  ('Centime_Assessment.jmx')**-: Jmeter script which defines thread group and the required HTTP API calls to test the preformance 

## Strategry 
- **API Tested**: JSONPlaceholder.typicode 
- **Test Approach**:
  1. **Functional Verification** – Ensured API endpoints were responding correctly using Jenikings.
  2. **Load Testing** – Simulated multiple concurrent users making requests.
### **Baseline Performance Test**
- **Thread Group**: Single user sending sequential API requests.
- **Goal**: Establish a baseline response time without load.


### **Concurrent User Load Test**
- **Thread Group**: [5,10,25,50] users.
- **Ramp-up Time**: [1,5,5,10] seconds.
- **Duration**: [5,5,5,5] minutes. 
- **Goal**: Measure average response time and throughput under normal load.


### **Stress Test**
- **Thread Group**: 200 users.
- **Ramp-up Time**: 30 seconds.
- **Duration**: 10 minutes.
- **Goal**: Identify breaking points and API failure rate under heavy load.

### ** Spike Test**
- **Thread Group**: 500 virtual users.
- **Ramp-up Time**: 5 seconds (Short burst).
- **Goal**: Observe how the API handles a sudden surge in traffic.

\
