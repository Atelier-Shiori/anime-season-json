# Anime Seasons

This repository includes anime season data for [MAL Library](https://github.com/chikorita157/MALLibrary), where it is used to display interactive season charts.

This is a JSON version of the [orginal](https://github.com/erengy/anime-seasons).

## Seasons

The data currently consists of all anime seasons between **Winter 2011** to **Winter 2017**.

Seasons are laid out in the following manner. Note that the winter season starts in the previous year (e.g. Winter 2016 starts in December 2015):

<table>
  <thead>
    <tr>
      <th align="center" colspan="3">Winter</th>
      <th align="center" colspan="3">Spring</th>
      <th align="center" colspan="3">Summer</th>
      <th align="center" colspan="3">Fall</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td bgcolor="#F0FFFF">12</td>
      <td bgcolor="#F0FFFF">1</td>
      <td bgcolor="#F0FFFF">2</td>
      <td bgcolor="#F0FFF0">3</td>
      <td bgcolor="#F0FFF0">4</td>
      <td bgcolor="#F0FFF0">5</td>
      <td bgcolor="#FFFFF0">6</td>
      <td bgcolor="#FFFFF0">7</td>
      <td bgcolor="#FFFFF0">8</td>
      <td bgcolor="#FAEBD7">9</td>
      <td bgcolor="#FAEBD7">10</td>
      <td bgcolor="#FAEBD7">11</td>
    </tr>
  </tbody>
</table>

## Database

The following information is available for each anime in a season:

Tag|Description
:--|:----------
`type`|1: TV<br>2: OVA<br>3: Movie<br>4: Special<br>5: ONA<br>6: Music
`id`|MyAnimeList ID
`producers`|Producers, licensors and studios
`image`|Poster image URL
`title`|Main romaji title

The rest of the information is retrieved directly from the active service by each client on demand. Ideally, it should have been possible to retrieve the entire information this way. But MyAnimeList does not provide such a method in its public API, which is why MAL Library needs this database.

This is a converted version of the [XML files](https://github.com/erengy/anime-seasons). I decided to convert them to JSON since it's easier to work with than XML.

Note that the data for a season does not include series continuing from previous seasons. Also note that some files, especially the older ones, may be out of date.

## License

This repository is in the public domain.

All data comes from MyAnimeList.net, which is a property of MyAnimeList, LLC.
