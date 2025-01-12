# diagrams.net AWS Architecture Icons

AWS Architecture Icons version:
[2022-04-30](https://d1.awsstatic.com/webteam/architecture-icons/q2-2022/Asset-Package_04302022.e942f826cd826cfa2d32455f3a7973ad4b92eb6a.zip)

## What is it?

Shapes library with [AWS Architecture Icons](https://aws.amazon.com/architecture/icons/)
for [diagrams.net](https://diagrams.net/)
([formerly draw.io](https://www.diagrams.net/blog/move-diagrams-net)) application.

The library can be loaded into diagrams.net by downloading particular `xml` files
and [loading them into application](https://www.diagrams.net/blog/custom-libraries)
or using links provided below.

## How it's different from the built-in AWS shapes library?

- more up-to-date
- shapes have connection points
- shapes size is 50x50 px instead of 78x78 px
  (I found it much more suitable personally)
- version with a single library with all the icons

## Library links

Click on the link to load library to diagrams.net.

[All icons as a single library](https://app.diagrams.net/?splash=0&clibs=Uhttps://raw.githubusercontent.com/m-radzikowski/diagrams-aws-icons/master/20220430/AWS%20Architecture%20Icons%2020220430.xml)
(may take few seconds to load)

## Previous versions

- [2021-09-17](https://app.diagrams.net/?splash=0&clibs=Uhttps://raw.githubusercontent.com/m-radzikowski/diagrams-aws-icons/master/20210917/AWS%20Architecture%20Icons%2020210917.xml)
- [2020-09-11](https://app.diagrams.net/?splash=0&clibs=Uhttps://raw.githubusercontent.com/m-radzikowski/diagrams-aws-icons/master/20200911/AWS%20Architecture%20Icons.xml)

## Generating library

Icons library is generated using [icons-asset-generator](https://github.com/m-radzikowski/icons-asset-generator):

```bash
poetry run icons-asset-generator \
    --filename-includes _48 \
    --filename-excludes Dark \
    --image-name-remove Light Arch_ Res_ _48 . - _  \
    --library-name-remove  . - _ \
    --path "./Asset-Package_04302022/" \
    diagrams.net \
    --size height=50
```

## Copyright

All right to the icons belong to Amazon Web Services.
