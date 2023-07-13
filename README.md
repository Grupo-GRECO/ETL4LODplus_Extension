![](img/logo_ETL4LODEXTENSION.png =250x250)


ETL4LOD+Extension é uma extensão do Kettle baseada no [ETL4LOD+](https://github.com/johncurcio/ETL4LODPlus/releases) para trabalhar com Linked Open Data, integrando com o GraphDB e FAIR Datapoints.

## Usando o Projeto

Usar o projeto é tão simples quanto [baixar a versão mais recente dos plugins](https://github.com/NickolasGomes/ETL4LOD-FAIR/releases) e extrair o ``steps.zip`` na pasta ``plugins/`` da sua instalação do Kettle 9.2+.

## Desenvolvimento

### Pré-requisitos

* [Pentaho Data Integration](https://sourceforge.net/projects/pentaho/)

Este projeto tem as seguintes dependências:

* [Java 8](https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html) para desenvolvimento.
* [Maven](https://maven.apache.org/) para gestão das dependências.
* [Kettle 8.1+](https://sourceforge.net/projects/pentaho/) para testes e deploy.

Todas as dependências estão na pasta "dependency" para instalação.

Este projeto foi desenvolvido na IDE Eclipse, porém é agnóstico em relação a IDEs - não é necessário o uso do Eclipse para desenvolver neste projeto.

### Instalando

Para rodar o projeto em sua máquina, instale todos os pré-requisitos (cuidado especial na versão do java, que tem que ser Java 8), mude a variável ``pdi.home``, que representa o caminho referente a sua instalação do Pentaho Data Integration, no pom do projeto pai ``ETL4LODPLUSFAIR\plugins\pom.xml`` - <pdi.home>Caminho\data-integration</pdi.home>. Após isso, rode o comando ``mvn clean install`` dentro do pasta ``plugins`` (projeto pai). Isso instalará os plugins no Kettle especificado em ``pdi.home``.

Abra o Kettle 9.2 e uma pasta chamada LinkedDataBR deve aparecer com os plugins deste projeto. 

### Deployment

Para fazer deploy, rode na pasta do projeto pai:

``mvn clean install``

Tendo certeza de apontar a variável ``pdi.home`` para a sua instalação do Kettle 9.2.

## Contribuição

Para mais informações sobre o desenvolvimento, por favor, leia [CONTRIBUTING.md](CONTRIBUTING.md).

## Versionamento

Usamos [SemVer](http://semver.org/) para versionamento do ETL4LOD+. Para ver as versões liberadas, entre nas [tags deste repositorio](https://github.com/johncurcio/ETL4LODPlus/tags).

## Licença

Este projeto usa a licença do MIT, veja [LICENSE.md](LICENSE) para mais detalhes.

## Inspirado em

* [ETL4LOD](https://github.com/rogersmendonca/ETL4LOD),  [ETL4LOD-graph](https://github.com/rogersmendonca/ETL4LOD-Graph) e [ETL4LOD+](https://github.com/johncurcio/ETL4LODPlus/)
