This project was the assignment of my supervisor for my curricular stage and also represents the heart of my bachelor's thesis. 
As an addictional microservice of a larger sustainability web architecture, this project was about building a working "TileServer", that is a server which provides vector tiles, and a tile-based map which makes requestes to the server for the vector tiles, and then visualizes them.

There is a video demo of the working map and also my pdf presentation of the project, which explains theoric context, technology stack, design choises and all that is about the project.

This 3-months-program has thoroughly trained me. I've learned to adapt myself at every situation/unknown (to me) tecnology. It was long and hard, but so useful, first to learn about these tecnologies, then to grow as a full-stack developer.

However, the project technology stack is buildt like this:
 - SvelteKit frontend on which we mount a MapLibre GL JS map, that makes the requestes to the tileserver and displays vector tiles
 - FastAPI Tileserver with some responsability-organized python files, such as tilemath (for the intra-tile calculations) or the db initializer. This makes SQL queries to the db and returns mvt tiles (encapsulated into HTTP response)
 - Duckdb (spatial extension) database, which allows me to build tiles database-side and on-demand (on-the-fly).

 For the project addictional features, please take a look at my presentation (Presentazione.pdf).