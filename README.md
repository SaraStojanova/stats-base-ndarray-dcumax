# 📊 Stats Base: Cumulative Maximum for Ndarrays

Welcome to the **Stats Base Ndarray Dcumax** repository! This library computes the cumulative maximum value of a one-dimensional double-precision floating-point ndarray. You can find the latest releases [here](https://github.com/SaraStojanova/stats-base-ndarray-dcumax/releases).

---

## Table of Contents

1. [Introduction](#introduction)
2. [Features](#features)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Examples](#examples)
6. [API Documentation](#api-documentation)
7. [Contributing](#contributing)
8. [License](#license)
9. [Contact](#contact)

---

## Introduction

The **Stats Base Ndarray Dcumax** library provides a simple and efficient way to compute the cumulative maximum of a one-dimensional array. It is designed for developers and data scientists who need a reliable tool for statistical analysis in JavaScript. 

With this library, you can easily manage large datasets and perform complex calculations with minimal effort. 

## Features

- **Easy to Use**: Simple API for quick implementation.
- **Performance**: Optimized for speed and efficiency.
- **Compatibility**: Works seamlessly with Node.js and JavaScript environments.
- **Lightweight**: Minimal dependencies for a clean setup.
- **Versatile**: Suitable for a variety of applications in statistics and data analysis.

## Installation

To install the library, use npm:

```bash
npm install stats-base-ndarray-dcumax
```

You can also clone the repository directly:

```bash
git clone https://github.com/SaraStojanova/stats-base-ndarray-dcumax.git
cd stats-base-ndarray-dcumax
npm install
```

## Usage

To use the library, first require it in your JavaScript file:

```javascript
const dcumax = require('stats-base-ndarray-dcumax');
```

Then, you can compute the cumulative maximum of your ndarray:

```javascript
const ndarray = require('ndarray');
const data = ndarray(new Float64Array([1.0, 2.5, 3.1, 2.0, 5.5]), [5]);
const result = dcumax(data);
console.log(result);
```

## Examples

### Basic Example

Here's a simple example to demonstrate how to use the library:

```javascript
const dcumax = require('stats-base-ndarray-dcumax');
const ndarray = require('ndarray');

const data = ndarray(new Float64Array([4.0, 2.0, 5.0, 1.0, 3.0]), [5]);
const result = dcumax(data);
console.log(result); // Output: [4.0, 4.0, 5.0, 5.0, 5.0]
```

### Working with Larger Datasets

For larger datasets, the library remains efficient:

```javascript
const dcumax = require('stats-base-ndarray-dcumax');
const ndarray = require('ndarray');

const largeData = ndarray(new Float64Array(1000000).fill(0).map((_, i) => Math.random() * 100), [1000000]);
const result = dcumax(largeData);
console.log(result);
```

## API Documentation

### `dcumax(data)`

- **Parameters**: 
  - `data`: A one-dimensional ndarray of double-precision floating-point numbers.
  
- **Returns**: An ndarray containing the cumulative maximum values.

### Example:

```javascript
const result = dcumax(ndarray(new Float64Array([1.0, 3.0, 2.0]), [3]));
console.log(result); // Output: [1.0, 3.0, 3.0]
```

## Contributing

We welcome contributions! To contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add new feature'`).
5. Push to the branch (`git push origin feature/YourFeature`).
6. Create a pull request.

Please ensure that your code follows the project's coding standards and includes appropriate tests.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For any questions or feedback, please reach out:

- **Author**: Sara Stojanova
- **Email**: sara@example.com
- **GitHub**: [SaraStojanova](https://github.com/SaraStojanova)

Thank you for using **Stats Base Ndarray Dcumax**! Check out the [Releases](https://github.com/SaraStojanova/stats-base-ndarray-dcumax/releases) section for updates and new features.