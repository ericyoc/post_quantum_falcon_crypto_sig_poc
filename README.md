# FALCON: Post-Quantum Signature Algorithm

This repository contains a Python implementation of the FALCON (Fast Fourier Lattice-based Compact Signatures over NTRU) post-quantum signature algorithm. FALCON is a lattice-based signature scheme that offers strong security guarantees against both classical and quantum attacks. NTRU is an open-source public-key cryptosystem that uses lattice-based cryptography to encrypt and decrypt data.

## Motivating Articles and Related Work
Opiłka, F., Niemiec, M., Gagliardi, M., & Kourtis, M. A. (2024). Performance Analysis of Post-Quantum Cryptography Algorithms for Digital Signature. Applied Sciences, 14(12), 4994. 
https://www.mdpi.com/2076-3417/14/12/4994

Mondal, P., Kundu, S., Bhattacharya, S., Karmakar, A., & Verbauwhede, I. (2024, February). A practical key-recovery attack on LWE-based key-encapsulation mechanism schemes using Rowhammer. In International Conference on Applied Cryptography and Network Security (pp. 271-300). Cham: Springer Nature Switzerland.
https://link.springer.com/chapter/10.1007/978-3-031-54776-8_11

FALCON 
https://falcon-sign.info/

Post-Quantum Cryptography NIST 
https://csrc.nist.gov/projects/post-quantum-cryptography



## Results
### Original Image:
![](https://github.com/ericyoc/post_quantum_falcon_crypto_sig_poc/blob/main/original_image.jpg)

### Different Image:
![](https://github.com/ericyoc/post_quantum_falcon_crypto_sig_poc/blob/main/diff_image.jpg)

### Tampered Image:
![](https://github.com/ericyoc/post_quantum_falcon_crypto_sig_poc/blob/main/tampered_image.jpg)

### Results Table:
![](https://github.com/ericyoc/post_quantum_falcon_crypto_sig_poc/blob/main/results_table_falcon.jpg)

## Why Post-Quantum Cryptography Matters

In the era of rapidly advancing quantum computing technology, traditional cryptographic algorithms based on integer factorization and discrete logarithms are becoming increasingly vulnerable. Quantum computers have the potential to solve these problems efficiently, rendering current security measures obsolete. This poses a significant risk to the confidentiality and integrity of sensitive data.

Post-quantum cryptography aims to address this challenge by developing algorithms that are resistant to attacks by both classical and quantum computers. By adopting post-quantum cryptographic techniques, we can ensure the long-term security of our digital assets and protect them against future quantum threats.

## FALCON Algorithm

FALCON is a post-quantum signature algorithm that provides a high level of security and efficiency. It is based on the hardness of lattice problems, which are believed to be resistant to quantum attacks. FALCON utilizes the Fast Fourier Transform (FFT) and the NTRU lattice structure to achieve compact signatures and fast verification.

Key features of FALCON include:

- **Security**: FALCON offers strong security guarantees against both classical and quantum attacks. It relies on the hardness of solving lattice problems, which are conjectured to be intractable even for quantum computers.
- **Compactness**: FALCON generates compact signatures, reducing storage and transmission overhead compared to other post-quantum signature schemes.
- **Efficiency**: The use of FFT and NTRU lattices enables fast signature generation and verification, making FALCON suitable for various applications.
- **Scalability**: FALCON supports different security levels by adjusting the parameters, allowing flexibility in balancing security and performance requirements.

## Implementation

The Python code in this repository demonstrates the usage of the FALCON algorithm for signing and verifying images. It includes the following key components:

- `falcon.py`: The core implementation of the FALCON algorithm, including key generation, signing, and verification functions.
- `sign_image` function: Signs an image using the FALCON algorithm and retries the signing process if the signature norm is too large.
- `verify_image` function: Verifies the signature of an image using the FALCON algorithm.
- Additional utility functions for image handling and conversion.
- A `main` function that demonstrates the end-to-end process of signing and verifying an image, along with performance metrics and additional checks.

The code also includes a results table that summarizes the algorithm metrics, such as signature length, signing time, verification time, and the validity of the signature. It performs additional checks, including verifying the signature with a different image and a tampered image, to ensure the correctness and robustness of the implementation.

## Conclusion

In a world where quantum computers pose a significant threat to traditional cryptographic algorithms, post-quantum cryptography is crucial for maintaining the security and confidentiality of sensitive data. The FALCON algorithm provides a robust and efficient solution for digital signatures that are resistant to quantum attacks.

By implementing the FALCON algorithm, as demonstrated in this Python code, developers can incorporate post-quantum security measures into their applications, ensuring the long-term protection of digital assets. It is essential to adopt post-quantum cryptography proactively to mitigate the risks associated with the advent of quantum computing and safeguard sensitive information from potential breaches.

## References

- FALCON: Fast Fourier Lattice-based Compact Signatures over NTRU (https://falcon-sign.info/)
- Post-Quantum Cryptography (https://csrc.nist.gov/projects/post-quantum-cryptography)

Feel free to contribute to this repository, provide feedback, and join the discussion on post-quantum cryptography and the FALCON algorithm.

## Disclaimer
The Python code is for academic and research purposes only.

## License
Copyright 2024 Eric Yocam

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.

