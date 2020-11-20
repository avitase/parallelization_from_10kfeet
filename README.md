## Platform overview
1. Sockets
2. Cores
3. Threads
4. Ports (Superscalar)
5. Pipelining
6. Vectors

## Types of parallelization
- Asynchronous execution
- Data parallelism
- Task parallelism
- Threads

## Resource protection and thread safety
- Data races
- Functional programming
- Minimize contention
- Atomics
- Locks / Mutexes

## Libraries
- [TBB](https://github.com/oneapi-src/oneTBB)
- [ZeroMQ](https://zeromq.org/)
- [multiprocessing](https://docs.python.org/3.9/library/multiprocessing.html)
- (replace raw loops with [numpy](https://numpy.org/))

## Notes
- Even if we don't talk about programming with SIMD, we should introduce the data oriented design principle
- Before talking about parallelization at all: [Amdahl's Law](https://en.wikipedia.org/wiki/Amdahl%27s_law)
- Explain [Roofline model](https://en.wikipedia.org/wiki/Roofline_model): decide whether application is CPU or I/O bound

