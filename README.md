# Tileserver GL Configuration
A basic configuration for [maptiler/tileserver-gl](https://github.com/maptiler/tileserver-gl).

# How to run the services?
There is one step required before you go. Download tiles from [Planet
Vector and raster map tiles](https://data.maptiler.com/downloads/planet/) and place them in the `./docker/services/tileserver/volumes/tiles` directory to be loaded on startup. Then by invoking the following command you can run your own tileserver at [http://127.0.0.1:8080](http://127.0.0.1:8080):

```bash
docker compose up --remove-orphans --build --force-recreate
```

# How to add new fonts/styles?
Add them to the `./docker/services/tileserver/volumes/fonts` and/or `./docker/services/tileserver/volumes/styles` directory.

# References
[1] https://openmaptiles.org/  
[2] https://openmaptiles.org/docs/  
[3] https://openmaptiles.org/styles/  
[4] https://data.maptiler.com/downloads/  
[5] https://github.com/maptiler/tileserver-gl  
[6] https://documentation.maptiler.com/hc/en-us/articles/8358453119249-MapTiler-Server-and-TileServer-GL-compared  
[7] https://github.com/maptiler/tileserver-gl/issues/530#issuecomment-821288022  
[8] https://github.com/korywka/fonts.pbf  
[9] https://docs.maptiler.com/gl-style-specification  
