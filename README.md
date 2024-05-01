# RoboCup Brasil Small Size League Entry Level Technical Challenges

This is the AsciiDoc source for the official RoboCup Small Size League Entry Level technical challenges rules.

Each year has its own directory with its .adoc files containing rules for each technical challenge that will or had happened in that specific year.

### Using AsciiDoctor natively
Install AsciiDoctor on your system (https://asciidoctor.org/). Afterwards, build HTML5 version with
```
# Build the HTML5 version
asciidoctor sslrules.adoc
# Build the PDF version
asciidoctor-pdf sslrules.adoc
```

### Using docker image
If you have Docker installed, you can use the official AsciiDoctor image:
```
# Pull image once
docker pull asciidoctor/docker-asciidoctor
# Build the HTML5 version
docker run -v $PWD:/documents/ asciidoctor/docker-asciidoctor asciidoctor -r asciidoctor-diagram sslrules.adoc
# Build the PDF version
docker run -v $PWD:/documents/ asciidoctor/docker-asciidoctor asciidoctor-pdf -r asciidoctor-diagram sslrules.adoc
```
