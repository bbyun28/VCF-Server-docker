# Getting VCF-Server started with [Docker](https://www.docker.com/)
<p>Type this into your commandline</p>

`docker run -d -p 8000:9000 jiangjp880123/vcf-server`   

<p>Then visit http://localhost:8000</p>

<p>Relevant links:</p>

[VCF-Server Homepage](https://www.diseasegps.org/VCF-Server?lan=eng)


# More advanced usage

<p>Store data on local</p>
`mkdir data`   
`docker run -d -p 8000:9000 -v ${PWD}/data:data jiangjp880123/vcf-server`   

Build from Dockerfile:   

`docker build -t vcfserver:1.0 .`
