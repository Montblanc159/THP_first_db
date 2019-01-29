# Data analysis with SQL

1. `SELECT * FROM albums;`
2. `SELECT * FROM albums WHERE Title LIKE '%Great%';`
3. `SELECT COUNT(Title) FROM albums`
4. `DELETE FROM albums WHERE title LIKE '%music%';`
5. `SELECT * FROM albums JOIN artists ON (artists.ArtistId = albums.ArtistId) WHERE artists.Name = 'AC/DC';`
6. `SELECT tracks.Name FROM tracks JOIN albums ON (tracks.AlbumId = albums.AlbumId) JOIN artists ON (albums.ArtistId = artists.ArtistId) WHERE artists.name = 'AC/DC';`
7. `SELECT tracks.Name FROM tracks JOIN albums ON (tracks.AlbumId = albums.AlbumId) JOIN artists ON (albums.ArtistId = artists.ArtistId) WHERE artists.Name = 'AC/DC' AND albums.title = 'Let There Be Rock';`
8. `SELECT SUM(tracks.UnitPrice) FROM tracks JOIN albums ON (tracks.AlbumId = albums.AlbumId) JOIN artists ON (albums.ArtistId = artists.ArtistId) WHERE artists.Name = 'AC/DC' AND albums.title = 'Let There Be Rock';`
9. `SELECT SUM(tracks.UnitPrice) FROM tracks JOIN albums ON (tracks.AlbumId = albums.AlbumId) JOIN artists ON (albums.ArtistId = artists.ArtistId) WHERE artists.Name = 'AC/DC' AND albums.title = 'Let There Be Rock';`
10. `SELECT ROUND(SUM(tracks.UnitPrice), 2) FROM tracks JOIN albums ON (tracks.AlbumId = albums.AlbumId) JOIN artists ON (albums.ArtistId = artists.ArtistId) WHERE artists.Name = 'Deep Purple';`
