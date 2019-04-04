# EPM Tag Port 

## Operando sobre Datasets obtidos através do Sistema EPM (o software PIMS da Elipse Software)

Nos processos de análises de dados uma das etapas iniciais é a definição um conjunto de dados sobre os quais serão realizadas inúmeras ações e processamentos para então, extrair as tão preciosas informações para direcionamento de ações futuras.

Na grande maioria das vezes, estes dados são coletados e armazenados em algum grande sistema de informação, de onde precisam ser selecionados e extraídos e empacotados em um formato padrão para posterior encaminhamento aos analistas.

Em geral, para séries temporais, o padrão utilizado é um arquivo *.CSV* (*Comma Separated Values*), porém atualmente, com as novas demandas de grandes volumes de dados, maior capacidade de processamento, etc., um padrão aberto vem se destacando para atender estes e outros requisitos - é o [HDF5](https://www.hdfgroup.org/), o formato de arquivo escolhido para armazenar os *datasets* extraídos a partir de um **Sistema EPM**.

## O que é o Sistema EPM e como gerar datasets no formato [HDF5](https://www.hdfgroup.org/)

O **Elipse Plant Manager**, ou simplesmente **EPM**, é um *software* do tipo *PIMS* (*Process/Plant Information Management System*) que coleta, processa, armazena e disponibiliza dados de processo oferecendo aos seus usuários uma plataforma completa para aplicação dos seus conhecimentos técnicos e atuação objetiva em uma estratégia de melhoria e/ou gestão continuada de processos.

Esta plataforma oferece inúmeras ferramentas para visualização e manipulação de dados de processo como: gráficos de tendência, integração com planilhas eletrônicas, relatórios, *dashboards web*, sistemas de automatização de processamentos e integrações com a linguagem Python, hoje referência para qualquer implementação de *Big Analytics*.

Para atingir esse objetivo, o **Sistema EPM** disponibiliza diversas ferramentas que foram desenvolvidas para auxiliar o usuário nesse processo de manipulação de dados, uma dessas ferramentas é o **EpmTagPort**, que permite ao usuário a exportação de um pacote de dados e informações de um **EPM Server** para outro, gerando um arquivo com a extensão *.hdf5*. Além disso, por se tratar de um padrão aberto, também é possível manipular diretamente este arquivo por qualquer sistema que suporte este formato.

Mais informações referentes ao **EPM** no site da [EPM - Elipse Software](https://www.elipse.com.br/produto/elipse-plant-manager/).

**Para uma rápida ideia do que é o Sistema EPM, assista ao vídeo a seguir** *(só 2 minutinhos)* **!**
[![O EPM](http://img.youtube.com/vi/TSiWcU43rGU/0.jpg)](https://youtu.be/TSiWcU43rGU)

---

## Por que [HDF5](https://www.hdfgroup.org/)?

O arquivo [HDF5](https://www.hdfgroup.org/) tem um formato hierárquico de organizar os dados muito semelhante ao sistema de diretórios, o que permite a criação de *Datasets* com dados complexos de fácil e eficiente acesso, o que justifica sua ampla usabilidade no armazenamento de grandes quantidades de dados numéricos, além de também permitir que os metadados sejam armazenados junto aos *Datasets*.

Os arquivos [HDF5](https://www.hdfgroup.org/) são estruturados usando dois tipos de objetos, os *Grupos* e os *Datasets*. Fazendo uma analogia com o sistema de diretórios, os *grupos* são como as pastas e os *datasets* como arquivos, sendo que dentro de um *grupo* podemos ter diversos *datasets*. O [HDF5](https://www.hdfgroup.org/) também nos permite armazenar os *metadados* de um *grupo* e/ou *dataset* junto ao objeto, como será demonstrado nos exemplos a seguir.

---

Os tópicos a seguir disponibilizam exemplos de como realizar análises sobre séries temporais utilizando a linguagem Python sobre dados de processo armazenados em arquivos no formato [HDF5](https://www.hdfgroup.org/) gerados a partir da ferramenta **EPMTagPort**.

* Exemplos

  * [Basics_TagPort_HDF5](examples/Basics_TagPort_HDF5.ipynb) - exemplo básico de análises sobre *datasets* no formato [HDF5](https://www.hdfgroup.org/).

---

Aprenda mais sobre [HDF5](https://www.hdfgroup.org/) na linguagem Python:
[HDF5 with Python: Course Introduction](https://youtu.be/y4DXr3Y10MM)
