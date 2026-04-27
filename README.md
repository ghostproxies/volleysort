# VolleySort™

[![VolleySort™](https://repository-images.githubusercontent.com/1206306104/751e7be5-5b3d-4e6d-876b-0bec1bd2c8b8)](https://github.com/ghostproxies/volleysort)

## Table of Contents

- [Introduction](README.md?tab=readme-ov-file#introduction)
- [Author](README.md?tab=readme-ov-file#author)
- [License](README.md?tab=readme-ov-file#license)
- [Reference](README.md?tab=readme-ov-file#reference)

## Introduction

VolleySort™ is the hyper-efficient gap sequence for Shell Sort.

## Author

VolleySort™ was created by [William Stafford Parsons](https://github.com/williamstaffordparsons) as a product of [GhostProxies](https://ghostproxies.com).

## License

VolleySort™ is licensed with the [BSD-3-Clause](LICENSE) license.

## Reference

VolleySort™ was implemented in C.

[volleysort.c](volleysort.c)

The `volleysort` function sorts (in ascending order without guaranteeing the preserved order of duplicate elements) an `elements` array of `elements_length` elements.

The integral type of each element in `elements` must match the integral type of `element`.

Each of the following sorting algorithm speed test results log the fastest process execution speed (from an AMD A4-9120C with `gcc -O3`) among several repetitions of a test that sorts various quantities (100k runs of 10, 10k runs of 100, 1k runs of 1k, 200 runs of 10k, 20 runs of 100k and 4 runs of 1m) of pseudorandom numbers (divided between mostly-sorted and unsorted distributions).

| Sorting Algorithm | Milliseconds |
| --- | --- |
| **`volleysort`** | **16ms, 27ms, 44ms, 121ms, 165ms, 518ms** |
| `shellsort_sedgewick_1982` | 17ms, 31ms, 53ms, 138ms, 182ms, 554ms |
| `shellsort_ciura` | 17ms, 32ms, 55ms, 164ms, 215ms, 685ms |
| `shellsort_papernov_stasevich` | 17ms, 32ms, 60ms, 181ms, 297ms, 936ms |
| `shellsort_sedgewick_1986` | 18ms, 31ms, 52ms, 165ms, 208ms, 658ms |
| `shellsort_lee` | 18ms, 31ms, 57ms, 167ms, 219ms, 686ms |
| `shellsort_tokuda` | 18ms, 32ms, 57ms, 167ms, 217ms, 677ms |
| `shellsort_hibbard` | 18ms, 32ms, 59ms, 181ms, 278ms, 913ms |
| `shellsort_knuth` | 18ms, 33ms, 53ms, 149ms, 202ms, 657ms |
| `shellsort_incerpi_knuth_sedgewick` | 18ms, 34ms, 56ms, 161ms, 210ms, 650ms |
| `shellsort` | 24ms, 45ms, 70ms, 202ms, 285ms, 858ms |
