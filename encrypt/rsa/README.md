# RSA Wrapper

## Functions

- Random Key generation
- RSA Encryption
- RSA Decryption

## RSA Algorithm

1. Choose 2 prime numbers p and q
2. Compute n = p\*q
3. Calculate phi = (p-1) \* (q-1)
4. Choose an integer e such that 1 < e < phi(n) and gcd(e, phi(n)) = 1
5. Calculate d as d = e - 1 (mod phi(n)); d is te modular multiplicative inverse of e modulo phi(n)
6. For encryption, c = me mod n, where m = original message
7. For decryption, m = c d mod n

## RSA Keys

- n
- e
- d
