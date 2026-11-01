# Confini dei comuni italiani

`comuni-italia.geojson`: confini dei 7.896 comuni italiani (codice ISTAT, nome, sigla della provincia, regione),
coordinate WGS84 arrotondate a 4 decimali (circa 10 metri).

Serve al database de Il Cercatore per decidere **dal server** in quale comune è stata fatta una raccolta
certificata, partendo dalla posizione GPS (non si fida più del nome del comune mandato dal telefono).
Si carica una volta sola con `supabase/certificati-robusti.sql` dell'app.

Fonte: [openpolis/geojson-italy](https://github.com/openpolis/geojson-italy) (dati ISTAT, confini amministrativi),
convertito da TopoJSON a GeoJSON senza altre modifiche.
