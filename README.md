Every 2 mins for the last two months I've logged the live location of the
torch relay runner for the London 2012 Olympic Games.

This project contains the complete log files.

The torch ran from Saturday, 19th May 2012 to Friday, 27th July 2012 (70 days).

The last active co-ordinate is located in the middle of Tower Bridge, scene of the David Beckham opening ceremony set piece, so sadly the GPS data doesn't lead right up to the stadium and Heatherwick's cauldren.

Files
-----

- gps.txt - all latitude and longitude points whilst the torch was moving.
- gps-complete.txt - complete timestamp, latitude, longitude, and torch status

Notes
-----

- Co-ordinates are from the GPS device inside the torch relay vehicle.
- The data is accurate in so far as much as the BBC's torch relay tracking feed was correct.
- The first 30 minutes of data is missing because [I only realised](https://twitter.com/egzplicit/status/203754238105497600) that nobody might be recording this information for posterity on the morning that torch was lit.
- A raw dump of the feed is available from [matt.chadburn.co.uk/projects/torchrelay/gps.tar.gz](http://matt.chadburn.co.uk/projects/torchrelay/gps.tar.gz)

Bad Data
--------

The data isn't perfect.

For example, the data shows quite a few duplicate entries, Eg. 

    sort gps.txt  | uniq -c | sort

The main outliers seem to be the following, which you might want to
remove before using this data.

    54.642830595671, -3.5335360166058
    52.60276677965, -2.557581837071
    52.054212538206, -1.7763742603503
    53.897208954164, -1.5276432105434
    54.232146462689, -4.4053278890666
    54.177582, -6.337282
    53.289861020818, -3.7143573448173
    51.771603752612, -3.1046361544431
    54.651566, -6.219893
    57.543609, -4.048376
    53.34029583263, -6.258211044218
    53.334973, -2.856445
    54.083613, -4.637132
    58.213792, -6.330614
    58.957976, -2.905025
    51.49227142334, -0.082998275756836
    54.086105, -4.632797
    59.878601, -1.295786
    58.982800406393, -2.974800047885
    51.080360708057, -1.9193594565
    50.943850512605, -2.6294230476567
    51.608028411865, -0.067720413208008
    50.624913452655, -2.4460959579877

Sample
------

Here's the 24th July data passed through http://www.gpsvisualizer.com/

![Route map](https://raw.github.com/commuterjoy/torch-relay/master/assets/2012-07-24-route-map.png)


