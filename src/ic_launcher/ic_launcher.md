## Instructions
- exported directly in inkscape to png.\
  &rarr; to keep the shadow of the logo in the image\
  &rarr; importing directly from svg in Android Studio will remove the shadow.

- imported with Image Asset and selected launcher.\
  &rarr; set the background background color to #CD201F

- rename ic\_launcher\_round and replace ic\_launcher with it
  ```bash
  for x in `find -iname 'ic_launcher_round*'` ; do rename  -f -e 's/launcher_round/launcher/' $x  ; done
  ```

### Export Quality
Image size: 1000px x 1000px\
Bit depth: GrayAlpha\_8\
Compression: Z\_NO\_COMPRESSION

## Additional Information
In the ic\_launcher.svg there is a less visible circle. This is
needed to help Image Asset not place the icon to far to the left.

This svg has a stronger shadow compared to the other svg's in
this repository.
