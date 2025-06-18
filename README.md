# Awesome M-Pesa [![Awesome](https://awesome.re/badge-flat.svg)](https://awesome.re)

> Uma seleção de artigos, bibliotecas e recursos úteis sobre a Open API do M-Pesa em Moçambique.

## Conteúdo

- [O que é a Open API do M-Pesa?](#o-que-é-a-open-api-do-m-pesa)
- [Como posso integrar?](#como-posso-integrar)
- [Processo](#processo)
  - [1. Ambiente de Desenvolvimento](#1-ambiente-de-desenvolvimento)
  - [2. Solicitação de Acesso à Produção](#2-solicitação-de-acesso-à-produção)
  - [3. Acordo e Treinamento](#3-acordo-e-treinamento)
  - [4. Integração em Produção](#4-integração-em-produção)
  - [5. Operação Comercial](#5-operação-comercial)
- [Recursos](#recursos)
- [Bibliotecas](#bibliotecas)
- [Artigos](#artigos)
- [Vídeos](#vídeos)
- [Regulamentação](#regulamentação)
- [Exemplo de E-mail de Solicitação](#exemplo-de-e-mail-de-solicitação)
- [Como contribuir](#como-contribuir)

## O que é a Open API do M-Pesa?

A Open API do M-Pesa é um conjunto de interfaces programáveis (APIs)
disponibilizadas pela Vodacom Moçambique que permite a integração de **aplicações**,
sistemas ou plataformas com os serviços financeiros digitais do M-Pesa.

O objetivo principal da Open API é permitir que empresas, desenvolvedores e instituições automatizem operações financeiras, como:

- Colecta de pagamentos (cobrança)
- Envio de fundos para clientes ou fornecedores
- Consultas de saldo e transações
- Estornos (reversões) de pagamentos
- Validação de contas

## Como posso integrar?

A integração pode ser feita de dois modos:

1. Directo, onde o desenvolvedor faz a intelergicação diretamente com a API do M-Pesa, utilizando as credenciais fornecidas pela Vodacom Moçambique.
2. Usando um agregador, que é uma empresa ou serviço que já possui integração com a API do M-Pesa e oferece uma interface simplificada para desenvolvedores.

O processo para a integração directa está descrito abaixo na secção [Processo](#processo).

## Processo

Em linhas gerais o processo de integração com a API Publica do M-Pesa envolve as seguintes etapas principais:

1. Criação de Conta e Integração no Ambiente de Desenvolvimento

  A primeira etapa consiste em criar uma conta no portal de desenvolvedores do M-Pesa, disponível em: https://developer.mpesa.vm.co.mz.
  Após o registo, será possível integrar o seu sistema ao ambiente de desenvolvimento, onde poderá testar todas as operações suportadas (cobrança, estorno, consulta, etc.).
  Neste ambiente, também terá acesso às API keys necessárias para a configuração e testes iniciais.

2. Validação e Pedido de Acesso ao Ambiente de Produção

  Assim que os testes forem concluídos com sucesso, deverá contactar a equipa do M-Pesa através do email: M-Pesa.business@vm.co.mz solicitando a migração para o ambiente de produção.
  Neste ponto, será necessário cumprir com determinados requisitos legais, que variam conforme o tipo de entidade (pessoa singular, empresa, organização, etc.).
  Os detalhes estão disponíveis no ficheiro de requisitos legais fornecido na secção de [recursos](#recursos).

3. Formalização do Acordo e Treinamento

  Em colaboração com a equipa do M-Pesa, deverá:

    - Enviar a documentação exigida;
    - Negociar as comissões aplicáveis;
    - Assinar o contrato de prestação de serviços;
    - Proceder à abertura de uma conta empresa no M-Pesa;
    - Participar numa formação sobre a gestão da conta e utilização do sistema, incluindo: gestão de utilizadores, reversões de transações, análise de relatórios, entre outros aspetos operacionais do backoffice.

4. Integração no Ambiente de Produção

Após a conclusão das etapas anteriores, será fornecido o acesso às *API keys* do ambiente de produção. Com estas credenciais, poderá configurar o seu sistema para iniciar as operações reais.

5. Início das Operações Comerciais

Com a integração finalizada e os acessos configurados, poderá começar a explorar e operar com a plataforma de pagamentos M-Pesa de forma plena.

## Recursos

- [Descrição do serviço da Open API do M-Pesa](https://www.vm.co.mz/m-pesa/artigo/api-aberta-do-m-pesa) - Documentação oficial do serviço.
- [Portal do Desenvolvedor M-Pesa](https://developer.mpesa.vm.co.mz/) - Portal oficial para desenvolvedores.
- [Requisitos de Acesso à API de Produção e Checklist](https://github.com/PauloPhagula/awesome-mpesa/files/13706274/Checklist.para.Pessoas.Colectivas.-.Versao.1.7.-.2022.pdf) - Documento oficial com requisitos e checklist para acesso à API.

## Bibliotecas

- [mpesasdk](https://github.com/realdm/mpesasdk) - SDK não oficial para facilitar a integração com a API de pagamentos da Vodacom Moçambique em aplicativos Android.
- [mpesa-node-api](https://github.com/thatfiredev/mpesa-node-api) - Biblioteca Node.js para a API do M-Pesa (Moçambique).
- [mpesa-php-api](https://github.com/abdulmueid/mpesa-php-api) - Biblioteca PHP para a API do M-Pesa (Moçambique).
- [mpesa_sdk_dart](https://github.com/realrgt/mpesa_sdk_dart) - Biblioteca Dart | Flutter para a API do M-Pesa (Moçambique).
- [mpesa-sdk-ios](https://github.com/AlgyJr/MpesaSDK.git) - Biblioteca Swift | iOS para a API do M-Pesa (Moçambique).
- [mpesa-wordpress-plugin](https://github.com/herquiloidehele/mpesa-wordpress-plugin) - Plugin de pagamento Vodacom M-PESA para WooCommerce em Moçambique.
- [wc-mpesa-payment-gateway](https://github.com/turbohost/wc-mpesa-payment-gateway) - Gateway de Pagamento Vodacom M-Pesa para WooCommerce.
- [karson/mpesa-php-sdk](https://github.com/karson/mpesa-php-sdk) - SDK PHP para as APIs RESTful do Vodacom M-Pesa em Moçambique.
- [paymentsds](https://github.com/paymentsds) - Conjunto de SDKs para integração de operações do M-Pesa em aplicativos.
- [mpesa-sdk-rust](https://github.com/GraHms/mpesa-rust-sdk) - Biblioteca Rust para interagir com a API do M-Pesa, simplificando integrações de pagamento B2C.

## Artigos

- [Mpesa, mais do que uma API…](https://medium.com/android-dev-moz/mpesa-mais-do-que-uma-api-bc2ead953cc2) - Artigo descrevendo o processo de integração, desde a criação da conta até a produção.
- [Um olhar sobre a API do M-Pesa](https://medium.com/android-dev-moz/um-olhar-sobre-a-api-do-m-pesa-688fd6abe351) - Visão geral da API do ponto de vista do desenvolvedor.
- [Decreto 59/2023 - destaques & implicações](https://www.linkedin.com/pulse/decreto-592023-destaques-implica%2525C3%2525A7%2525C3%2525B5es-m%2525C3%2525A1rio-j%2525C3%2525BAnior-snpzf%3FtrackingId=tVAdOsDNxQFQ8YzQMotn4w%253D%253D/?trackingId=tVAdOsDNxQFQ8YzQMotn4w%3D%3D) - Análise do decreto e suas implicações.

## Vídeos

- [Implementar Mpesa em Android (Dario Mungoi mpesaSDK)](https://www.youtube.com/watch?v=RtY67lsb5TY) - Tutorial de implementação do M-Pesa em aplicativos Android.

## Regulamentação

- [Lei das Transações Eletrônicas](https://github.com/PauloPhagula/awesome-mpesa/files/12642436/Lei-das-Transaccoes-eletronicas.pdf) - Documento oficial da lei.
- [Regulamento de Registro e Licenciamento BR_206_I_SERIE_2023](https://github.com/PauloPhagula/awesome-mpesa/files/14340618/Regulamento.de.Registo.e.Licenciamento.BR_206_I_SERIE_2023.pdf) - Regulamento oficial de registro e licenciamento.

## Exemplo de E-mail de Solicitação

Para: M-Pesa.business@vm.co.mz  
Assunto: Acesso à Open API para {Nome da Empresa}  
De: Responsável pelo Negócio  
Corpo:

```txt
Saudações, equipe M-Pesa,

Espero que este e-mail os encontre bem. Meu nome é {Seu Nome} e estou entrando em contato como responsável pelo negócio para solicitar formalmente o acesso à Open API.
Em anexo, envio todos os documentos necessários especificados no Checklist fornecido. Certifiquei-me de incluir todas as informações exigidas para sua análise.
Aguardo instruções sobre os próximos passos do processo.
Obrigado pela atenção e retorno rápido.

Atenciosamente,
```

## Como contribuir

Por favor, leia o [guia de contribuição](contributing.md).
