
## Instalación de Scrapy
### instalando python 

```bash

sudo apt-get install python3 python3-dev python3-pip libxml2-dev libxslt1-dev zlib1g-dev libffi-dev libssl-dev

```

### Entorno virtual

```
python3 -m venv venv

source venv/bin/activate
```

### Entorno virtual

```
pip3 install autopep8 scrapy
```

### Iniciar un proyecto con scrapy

```
scrapy startproject quotes_scraperscra
```

## Spiders

Los Spinder son los archivos para obtener respuesta del servidor

```
scrapy crawl quotes
```


## Scrapy shell

### xpath en navegadores

```
$x('//')
```

### abrir scrapy shell xpath
```
scrapy shell 'http://quotes.toscrape.com/'
```

### usar xpath en scrapy
```
response.xpath('//h1/a/text()')
response.xpath('//h1/a/text()').get()
response.xpath('//span[@class="text" and @itemprop="text"]/text()').getall()

```

### metodos de response 

```
response.encoding
reposnse.headers
response.status
response.body

```





