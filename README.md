# GeyserMC

version: "3.7"
services:
  geyser:
    image: mightydetail/geyser:latest
    container_name: geyser
    restart: unless-stopped
    ports:
      - "19132:19132/udp"
    volumes:
      - /opt/geyser:/data
