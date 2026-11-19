# Raycasting #

Raycasting programs based on https://lodev.org/cgtutor/raycasting.html and https://www.youtube.com/watch?v=2IEUa2gYJHQ

### Contents and Use ###

Basic untextured raycaster (walls are all colored squares):

g++ raycaster_untextured.cpp -o untextured_raycaster $(sdl2-config --cflags --libs) && ./untextured_raycaster

Textured raycaster (walls upgraded to basic textures):

g++ raycaster_textured.cpp -o textured_raycaster $(sdl2-config --cflags --libs) && ./textured_raycaster

Textured raycaster with floors and ceilings added:

g++ raycaster_textured_floors.cpp -o floor_ceiling $(sdl2-config --cflags --libs) $(pkg-config --cflags --libs SDL2_image) && ./floor_ceiling

Textured raycaster with floors/ceilings and sprites added:

g++ raycaster_textured_floors_sprites.cpp -o sprites $(sdl2-config --cflags --libs) $(pkg-config --cflags --libs SDL2_image) && ./sprites