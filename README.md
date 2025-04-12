# nk256

Unicode-based Base-256,000 numeral encoding system.

- Uses 256,000 Unicode characters from U+20000 and upward
- Designed for ultra-compression of massive integers
- Not all characters may render properly (some may appear as □)
- Fully reversible and numerically sortable
- Ideal for internal compression, tagging, indexing

## Example

```python
import nk256

n = 12345678901234567890
encoded = nk256.encode_nk256(n)
decoded = nk256.decode_nk256(encoded)

print("🔐 Encoded:", encoded)
print("🔓 Decoded:", decoded)
print("✅ Success:", decoded == n)
```
