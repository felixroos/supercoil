# supercoil

supercoil is a live codable modular synth in a single HTML file, inspired by SuperCollider.

You can use it here: <https://felixroos.github.io/supercoil/>

The HTML file is [doughbeat](https://github.com/felixroos/doughbeat) with a minimal version of [kabelsalat](https://kabel.salat.dev) up front. You can look at the source code within doughbeat [here](https://felixroos.github.io/doughbeat/#Ly8gZ3JhcGggbGliCmNsYXNzIE5vZGUgewogIGNvbnN0cnVjdG9yKHR5cGUsIGlucykgewogICAgdGhpcy50eXBlID0gdHlwZTsKICAgIHRoaXMuaW5zID0gaW5zOwogIH0KfQpsZXQgcmVnaXN0ZXIgPSAodHlwZSwgbm9kZUNsYXNzID0gTm9kZSkgPT4gewogIE5vZGUucHJvdG90eXBlW3R5cGVdID0gZnVuY3Rpb24gKC4uLmFyZ3MpIHsKICAgIHJldHVybiBuZXcgbm9kZUNsYXNzKHR5cGUsIFt0aGlzLCAuLi5hcmdzXSk7CiAgfTsKICByZXR1cm4gKC4uLmFyZ3MpID0+IG5ldyBub2RlQ2xhc3ModHlwZSwgYXJncyk7Cn07Ck5vZGUucHJvdG90eXBlLm91dCA9IGZ1bmN0aW9uKCkgewogIGNvbnN0IGdyYXBoID0gdGhpczsKICBjb25zdCBzb3J0ZWQgPSBbXTsKICBsZXQgY29kZSA9ICIiOwogIGNvbnN0IG5vZGVzID0ge307CiAgY29uc3QgZ2V0SWQgPSAoaW5wdXQpID0+CiAgICB0eXBlb2YgaW5wdXQgPT09ICJudW1iZXIiID8gaW5wdXQgOiBgbiR7c29ydGVkLmluZGV4T2YoaW5wdXQpfWA7CiAgY29uc3QgdmlzaXRlZCA9IG5ldyBTZXQoKTsKICBmdW5jdGlvbiBkZnMobm9kZSkgewogICAgaWYgKHR5cGVvZiBub2RlICE9PSAib2JqZWN0IiB8fCB2aXNpdGVkLmhhcyhub2RlKSkgewogICAgICByZXR1cm47CiAgICB9CiAgICB2aXNpdGVkLmFkZChub2RlKTsKICAgIGZvciAobGV0IGkgaW4gbm9kZS5pbnMpIHsKICAgICAgZGZzKG5vZGUuaW5zW2ldKTsKICAgIH0KICAgIHNvcnRlZC5wdXNoKG5vZGUpOwogICAgY29uc3QgYXJncyA9IG5vZGUuaW5zLm1hcChnZXRJZCkuam9pbigiLCIpOwogICAgY29uc3Qgbm9kZUlkID0gZ2V0SWQobm9kZSk7CiAgICBub2Rlc1tub2RlSWRdID0gbm9kZTsKICAgIGNvZGUgKz0gYFxuY29uc3QgJHtub2RlSWR9ID0gbm9kZXNbJyR7bm9kZUlkfSddLnVwZGF0ZSgke2FyZ3N9KTsgLy8gJHtub2RlLnR5cGV9YDsKICB9CiAgZGZzKGdyYXBoKTsKICBjb2RlICs9IGBcbnJldHVybiAke2dldElkKGdyYXBoKX1gOwogIGNvbnNvbGUubG9nKGNvZGUpOwogIGxldCB1cGRhdGUgPSBuZXcgRnVuY3Rpb24oIm5vZGVzIiwgY29kZSk7CiAgbGV0IHRpY2sgPSAoKSA9PiB1cGRhdGUobm9kZXMpOwogIHJldHVybiB0aWNrOwp9CgovLyBzdGFydCBvZiBkc3AgbGliCmxldCBJU1IgPSAxIC8gNDQxMDA7CmNvbnN0IHNpbmUgPSByZWdpc3RlcigKICAic2luZSIsCiAgY2xhc3MgZXh0ZW5kcyBOb2RlIHsKICAgIHBoYXNlID0gMDsKICAgIHVwZGF0ZSA9IChmcmVxKSA9PiBNYXRoLnNpbigodGhpcy5waGFzZSArPSAyICogTWF0aC5QSSAqIGZyZXEgKiBJU1IpKTsKICB9Cik7CmNvbnN0IGFkZCA9IHJlZ2lzdGVyKAogICJhZGQiLAogIGNsYXNzIGV4dGVuZHMgTm9kZSB7CiAgICB1cGRhdGUgPSAoYSwgYikgPT4gYSArIGI7CiAgfQopOwpjb25zdCBtdWwgPSByZWdpc3RlcigKICAibXVsIiwKICBjbGFzcyBleHRlbmRzIE5vZGUgewogICAgdXBkYXRlID0gKGEsIGIpID0+IGEgKiBiOwogIH0KKTsKY29uc3QgZHVzdCA9IHJlZ2lzdGVyKAogICJkdXN0IiwKICBjbGFzcyBleHRlbmRzIE5vZGUgewogICAgdXBkYXRlID0gKGRlbnNpdHkpID0+IChNYXRoLnJhbmRvbSgpIDwgZGVuc2l0eSAqIElTUiA/IE1hdGgucmFuZG9tKCkgOiAwKTsKICB9Cik7CmNvbnN0IHJhbmdlID0gcmVnaXN0ZXIoCiAgInJhbmdlIiwKICBjbGFzcyBleHRlbmRzIE5vZGUgewogICAgdXBkYXRlKGlucHV0LCBtaW4sIG1heCkgewogICAgICBjb25zdCB1bmkgPSAoaW5wdXQgKyAxKSAqIDAuNTsKICAgICAgcmV0dXJuIHVuaSAqIChtYXggLSBtaW4pICsgbWluOwogICAgfQogIH0KKTsKY29uc3QgaW1wdWxzZSA9IHJlZ2lzdGVyKAogICJpbXB1bHNlIiwKICBjbGFzcyBleHRlbmRzIE5vZGUgewogICAgcGhhc2UgPSAxOwogICAgdXBkYXRlKGZyZXEpIHsKICAgICAgdGhpcy5waGFzZSArPSBJU1IgKiBmcmVxOwogICAgICBsZXQgdiA9IHRoaXMucGhhc2UgPj0gMSA/IDEgOiAwOwogICAgICB0aGlzLnBoYXNlID0gdGhpcy5waGFzZSAlIDE7CiAgICAgIHJldHVybiB2OwogICAgfQogIH0KKTsKCmNvbnN0IGxwZiA9IHJlZ2lzdGVyKAogICJscGYiLAogIGNsYXNzIGV4dGVuZHMgTm9kZSB7CiAgICBzMCA9IDA7CiAgICBzMSA9IDA7CiAgICB1cGRhdGUocywgY3V0b2ZmLCByZXNvbmFuY2UgPSAwKSB7CiAgICAgIC8vIE91dCBvZiBib3VuZCB2YWx1ZXMgY2FuIHByb2R1Y2UgTmFOcwogICAgICBjdXRvZmYgPSBNYXRoLm1pbihjdXRvZmYsIDEpOwogICAgICByZXNvbmFuY2UgPSBNYXRoLm1heChyZXNvbmFuY2UsIDApOwogICAgICB2YXIgYyA9IE1hdGgucG93KDAuNSwgKDEgLSBjdXRvZmYpIC8gMC4xMjUpOwogICAgICB2YXIgciA9IE1hdGgucG93KDAuNSwgKHJlc29uYW5jZSArIDAuMTI1KSAvIDAuMTI1KTsKICAgICAgdmFyIG1yYyA9IDEgLSByICogYzsKICAgICAgdmFyIHYwID0gdGhpcy5zMDsKICAgICAgdmFyIHYxID0gdGhpcy5zMTsKICAgICAgLy8gQXBwbHkgdGhlIGZpbHRlciB0byB0aGUgc2FtcGxlCiAgICAgIHYwID0gbXJjICogdjAgLSBjICogdjEgKyBjICogczsKICAgICAgdjEgPSBtcmMgKiB2MSArIGMgKiB2MDsKICAgICAgcyA9IHYxOwogICAgICB0aGlzLnMwID0gdjA7CiAgICAgIHRoaXMuczEgPSB2MTsKICAgICAgcmV0dXJuIHM7CiAgICB9CiAgfQopOwoKY29uc3Qgc2F3ID0gcmVnaXN0ZXIoInNhdyIsIGNsYXNzIGV4dGVuZHMgTm9kZSB7IApwaGFzZSA9IDAKdXBkYXRlID0gKGZyZXEpID0+IHsKICB0aGlzLnBoYXNlICs9IElTUiAqIGZyZXE7CiAgcmV0dXJuICh0aGlzLnBoYXNlICUgMSkgKiAyIC0gMTsKfQp9KQovLyBlbmQgb2YgbGliCgoKbGV0IGRzcCA9IHNhdyg1NSkubHBmKHNpbmUoLjUpLnJhbmdlKC40LC44KSkub3V0KCkKCgo=) ( might be out of date, but you get the idea )

## Usage

Here's an example of an audio graph:

```js
saw(55).lpf(sine(2).range(0.2, 0.8), 0.2).out();
```

In this example, we have a sawtooth wave at 55Hz going into a filter that is modulated with a sine wave.
You can chain any of the below functions. Make sure to end with `.out()`.

## API

- [x] `saw(freq)` sawtooth oscillator
- [x] `sine(freq)` sine oscillator
- [x] `pulse(freq, duty)` pulse oscillator
- [x] `range(input, min, max)` scales bipolar signal to range
- [x] `delay(input, time)` delay signal by time
- [ ] ad
- [x] `add(a, b)` add
- [x] `adsr(input, a,d,s,r)` ADSR envelope
- [ ] and
- [ ] apply
- [ ] ar
- [ ] audioin
- [ ] bpf
- [ ] brown
- [ ] bytebeat
- [ ] cc
- [ ] clockdiv
- [ ] cos
- [ ] debug
- [ ] delay
- [ ] distort
- [ ] div
- [x] `dust(density)` random single sample impulses
- [ ] exp
- [ ] floatbeat
- [ ] fold
- [ ] fork
- [ ] greater
- [ ] hold
- [ ] hpf
- [x] `impulse(freq)` single sample oscillator
- [ ] lag
- [ ] lfnoise
- [ ] log
- [x] `lpf(input, freq, res)` low pass filter
- [ ] map
- [ ] midicc
- [ ] midifreq
- [ ] midigate
- [ ] midinote
- [ ] mix
- [ ] mod
- [ ] module
- [ ] mouseX
- [x] `mul(a, b)` multiply
- [ ]
- more to come?
