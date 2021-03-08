## Platform overview
1. Sockets
2. Cores
3. Threads
4. Ports (Superscalar)
5. Pipelining
6. Vectors

## Types of parallelization
- Asynchronous execution
  - Example: [(Boost) Asio](https://think-async.com/Asio/) one `io::context` with multiple threads vs. many single threaded `io::context`s, cf. for example [CppCon 2019: Robert Leahy "The Networking TS in Practice: Patterns for Real World Problems", Slide 22ff](https://youtu.be/3wy1OPqNZZ8?t=1759)
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
- [(Boost) Asio](https://think-async.com/Asio/)
- [ZeroMQ](https://zeromq.org/)
- [multiprocessing](https://docs.python.org/3.9/library/multiprocessing.html)
- (replace raw loops with [numpy](https://numpy.org/))

## Notes
- Even if we don't talk about programming with SIMD, we should introduce the data oriented design principle
- Before talking about parallelization at all: [Amdahl's Law](https://en.wikipedia.org/wiki/Amdahl%27s_law)
- Explain [Roofline model](https://en.wikipedia.org/wiki/Roofline_model): decide whether application is CPU or I/O bound

## Articles to read
- [Python Concurrency: The Tricky Bits](https://python.hamel.dev/concurrency/), discussed on [the Real Python podcast](https://realpython.com/podcasts/rpp/50/#t=2127) and based on [David Beazley's PyCon 2015 talk](https://youtu.be/MCs5OvhV9S4)
