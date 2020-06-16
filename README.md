This script watches for BloodHound json and zip in the `data/` folder and sends them to Neo4j.

It is only a proof of concept, do not use in production!

# Build

`docker build . -t bh-auto`

# Run

`Docker run --rm -v $(pwd)/data:/app/data --network host --name bh-auto bh-auto`
