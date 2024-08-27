# supercoil

supercoil is a single-HTML audio graph live-coding editor. It is [doughbeat](https://github.com/felixroos/doughbeat) with a minimal version of [kabelsalat](https://kabel.salat.dev) inside.

You can use it here: <https://felixroos.github.io/supercoil/>

## Usage

Here's an example of an audio graph:

```js
let dsp = saw(55).lpf(sine(2).range(0.2, 0.8), 0.2).out();
```

In this example, we have a sawtooth wave at 55Hz going into a filter that is modulated with a sine wave.
You have to start with `let dsp =`, then define your graph and end with `.out()`.

## API

- `saw(freq)` sawtooth oscillator
- `sine(freq)` sine oscillator
- `add(a, b)` add
- `mul(a, b)` multiply
- `dust(density)` random single sample impulses
- `range(input, min, max)` scales bipolar signal to range
- `impulse(freq)` single sample oscillator
- `lpf(input, freq, res)` low pass filter
- more to come
