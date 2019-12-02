# gdal2tiles

This is a fork of the [official `gdal2tiles.py` script](https://github.com/OSGeo/gdal/blob/master/gdal/swig/python/scripts/gdal2tiles.py).

I essentially only want to switch to retina tiles, which are 512x512 instead of
256x256. It seemed like the easiest way to do that was to fork it and switch
every instance of `256` with `512`. [[0]](https://gis.stackexchange.com/questions/112009/use-gdal2tiles-to-generate-512px-tiles)

## Using

Install GDAL; I suggest either through Homebrew: `brew install gdal` or through conda:

```
conda create -n gdal python gdal -c conda-forge
```

then
```
git clone https://github.com/nst-guide/gdal2tiles
cd gdal2tiles
./gdal2tiles.py
```