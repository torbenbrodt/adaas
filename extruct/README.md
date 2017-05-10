# Scrapy Extruct
Docker image for Scrapy Extruct.

```bash
git clone --recursive https://github.com/torbenbrodt/adaas
cd adaas
docker-compose up
```

## Demo
```bash
curl "http://localhost:10005/extruct/http://www.spiegel.de/politik/ausland/donald-trump-feuert-james-comey-putsch-von-oben-kommentar-a-1146923.html" | json_reformat
{
    "json-ld": [
        {
            "name": "a-1146923",
            "keywords": [
                "Thema: Donald Trump",
                "Thema: FBI",
                "Thema: Meinung"
            ],
            "mainEntityOfPage": "http://www.spiegel.de/politik/ausland/donald-trump-feuert-james-comey-putsch-von-oben-kommentar-a-1146923.html",
            "dateModified": "2017-05-10T11:57:00+0200",
            "thumbnailUrl": "http://cdn2.spiegel.de/images/image-1139979-thumb-etly-1139979.jpg",
            "datePublished": "2017-05-10T11:57:00+0200",
            "@type": "NewsArticle",
            "author": [
                {
                    "@type": "Person",
                    "name": "Veit Medick"
                }
            ],
            "headline": "Trump feuert FBI-Chef Comey: Putsch von oben",
            "@context": "http://schema.org",
            "dateCreated": "2017-05-10T11:57:00+0200",
            "publisher": {
                "@type": "Organization",
                "name": "SPIEGEL ONLINE",
                "logo": {
                    "height": 60,
                    "@type": "ImageObject",
                    "url": "http://www.spiegel.de/static/sys/v12/logo/spiegel_online_logo_451_60_amp.png",
                    "width": 451
                }
            },
            "image": {
                "height": 566,
                "@type": "ImageObject",
                "url": "http://cdn2.spiegel.de/images/image-1139979-galleryV9-etly-1139979.jpg",
                "width": 850
            },
            "creator": [
                "Veit Medick"
            ],
            "url": "http://www.spiegel.de/politik/ausland/donald-trump-feuert-james-comey-putsch-von-oben-kommentar-a-1146923.html",
            "articleSection": "Politik"
        }
    ],
    "status": "ok",
    "url": "http://www.spiegel.de/politik/ausland/donald-trump-feuert-james-comey-putsch-von-oben-kommentar-a-1146923.html",
    "microdata": [

    ]
}
```
