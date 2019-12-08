# resize

```
sips -Z 640 *.png
for i in *.png; do sips -s format jpeg -s formatOptions 85 "${i}" --out "${i%png}jpg"; done
for i in *.jpg; do cwebp -q 85 "${i}" -o "${i%jpg}webp"; done
```
