# nk256_full

Unicode-based Base-256,000 numeral encoding system (full version).

- Uses 256,000 Unicode characters starting from U+20000
- Designed for ultra-compressed integer encoding
- Not all characters are human-readable (may display as □ or blank)
- Fully reversible: perfect for database tagging, prime maps, internal IDs

## Example

```python
import nk256_full as nk256

n = 98765432101234567890
encoded = nk256.encode_nk256(n)
decoded = nk256.decode_nk256(encoded)

print("🔐 Encoded:", encoded)
print("🔓 Decoded:", decoded)
print("✅ Success:", decoded == n)
```
