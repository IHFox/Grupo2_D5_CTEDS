# Documento de arquitetura

## Histórico de revisão
| Data   | Versão | Modificação  | Autor  |
| :- | :- | :- | :- |
| 08/08/2022 | 0.1 | Adição do tópico Objetivo |  Maurício Pirâmides |
| 08/08/2022 | 0.2 | Adição da Representação arquitetural |  Maurício Pirâmides |
| 12/08/2022 | 0.3 | Atuaização da representação arquitetural |  Maurício e Pedro |

## 1. Introdução

### 1.1 Objetivo
Este documento oferece uma visão geral arquitetural do 
sistema que será implementado, permitindo assim que os 
envolvidos no projeto conheçam como a aplicação será 
subdivida e quais serão as funções de cada componente.

Outro objetivo desse documento é elucidar quais foram as 
motivações que levaram a equipe a tomar decisões a respeito
dessa arquitetura.

## 2. Representação arquitetural
A arquitetura foi dividida em 4 blocos principais. Frond-end com a utilização de angular, back-end com a utilização de uma API e o Django REST, API de pagamento (Pag Seguro) para controlar pagamentos feitos na plataforma e banco de dados em nuvem (Azure) para armazenamento de informações de login, além de todos os produtos e suas características.

### 2.1 Diagrama de arquitetura
![image](https://user-images.githubusercontent.com/68930353/184456107-0f346744-a65d-454f-8d92-b67de42ec16d.png)

### 2.2 Angular
O Angular é um poderoso framework que utiliza HTML e TypeScript para criar a interface com o usuário, ou seja, o front-end em aplicações web, desktop e dispositivos móveis. A escolha tambem considerou a boa comunicação com o Django REST usado no Back-end.

### 2.3 Django REST Framework
Uma poderosa ferramenta para criaçao de Web APIs. Por funcionar sob a estrutura do Django, permite a construção de APIs em qualquer plataforma, seja Windows, macOS ou Linux.

### 2.4 SQL database da Azure
Banco de dados em nuvem com suporte e garantia da Microsoft.

### 2.5 API de pagamento
Optamos pela Pag Seguro, que fornece diversas possibilidades de pagamento, além de ter taxas menores no mercado.
