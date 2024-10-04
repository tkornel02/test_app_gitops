# Alap image kiválasztása
FROM node:14

# Munkkönyvtár létrehozása a konténerben
WORKDIR /usr/src/app

# package.json másolása az app mappából
COPY app/package*.json ./

# Függőségek telepítése
RUN npm install

# Alkalmazás forráskódjának másolása az app mappából
COPY app .

# Port meghatározása, amin az alkalmazás fut
EXPOSE 3000

# Alkalmazás indítása
CMD [ "node", "hello-world-app.js" ]