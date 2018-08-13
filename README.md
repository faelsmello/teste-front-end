# Teste Front-end Focomultimídia
Este teste é apresentado aos candidatos a vaga de desenvolvedor Front-end para avaliação dos quesitos técnicos.

### O Desafio

O objetivo é criar um app que deve conter no `mínimo` duas páginas, uma que exibe um formulário com os campos abaixo, e outra que liste os dados cadastrados.

* Nome completo
* CPF
* Telefone
* Email
* Cep
* Logradouro
* Bairro
* Cidade
* Estado

### Pré-requisitos: 
 - Deve ser possível criar, listar e excluir os dados cadastrados pelo formulário;
 - O formulário precisa ter validação;
 - Fazer a persistência dos dados no `localStorage` ou `IndexedDB`;
 - Só é permitido a utilização de dois frameworks: `AngularJS` (preferencialmente) ou Angular2+;

Para listagem inicial dos usuários utilizar este recurso abaixo:

> GET https://private-21e8de-rafaellucio.apiary-mock.com/users

Response:

```json
[
  {
        "name": "Rodrigo Carlos Eduardo Vitor Bernardes",
        "cpf": "68872563550",
        "phone": "71988473870",
        "email": "rrodrigocarloseduardovitorbernardes@mac.com",
        "cep": "40250050",
        "place": "Travessa Candeias",
        "bairro": "Cosme de Farias",
        "city": "Salvador",
        "uf": "BA"
    },
    {
        "name": "Thomas Tiago Baptista",
        "cpf": "45111862510",
        "phone": "71989473446",
        "email": "thomastiagobaptista..thomastiagobaptista@dr.com",
        "cep": "40255050",
        "place": "Avenida Almeida Santos",
        "Address": "Matatu",
        "city": "Salvador",
        "uf": "BA"
    },
    {
        "name": "Davi Edson Erick Ribeiro",
        "cpf": "34139880503",
        "phone": "71982833679",
        "email": "daviedsonerickribeiro__daviedsonerickribeiro@contabilidadelibra.com.br",
        "cep": "40435050",
        "place": "Avenida Irmãos Gêmeos",
        "Address": "Massaranduba",
        "city": "Salvador",
        "uf": "BA"
    }
]
```

A partir deste ponto utilizar o `localStorage/IndexedDB` para salvar localmente as informações.

Save:

```json
    {
        "name": "Fernando Nelson Calebe Teixeira",
        "cpf": "18773006599",
        "phone": "402945153",
        "email": "fernandonelsoncalebeteixeira..fernandonelsoncalebeteixeira@openlink.com.br",
        "cep": "40313595",
        "place": "Beco do Jiló",
        "Address": "Beco do Jiló",
        "city": "Salvador",
        "uf": "BA"
    }
```

Lista local:

```json
[
  {
        "name": "Rodrigo Carlos Eduardo Vitor Bernardes",
        "cpf": "68872563550",
        "phone": "71988473870",
        "email": "rrodrigocarloseduardovitorbernardes@mac.com",
        "cep": "40250050",
        "place": "Travessa Candeias",
        "bairro": "Cosme de Farias",
        "city": "Salvador",
        "uf": "BA"
    },
    {
        "name": "Thomas Tiago Baptista",
        "cpf": "45111862510",
        "phone": "71989473446",
        "email": "thomastiagobaptista..thomastiagobaptista@dr.com",
        "cep": "40255050",
        "place": "Avenida Almeida Santos",
        "Address": "Matatu",
        "city": "Salvador",
        "uf": "BA"
    },
    {
        "name": "Davi Edson Erick Ribeiro",
        "cpf": "34139880503",
        "phone": "71982833679",
        "email": "daviedsonerickribeiro__daviedsonerickribeiro@contabilidadelibra.com.br",
        "cep": "40435050",
        "place": "Avenida Irmãos Gêmeos",
        "Address": "Massaranduba",
        "city": "Salvador",
        "uf": "BA"
    },
    {
        "name": "Fernando Nelson Calebe Teixeira",
        "cpf": "18773006599",
        "phone": "402945153",
        "email": "fernandonelsoncalebeteixeira..fernandonelsoncalebeteixeira@openlink.com.br",
        "cep": "40313595",
        "place": "Beco do Jiló",
        "Address": "Beco do Jiló",
        "city": "Salvador",
        "uf": "BA"
    }
]
```
### Dados do Endereço:
Para cadastro do endereço usar o serviço do VIA CEP para autocompletar o formulário

> GET https://viacep.com.br/ws/41275034/json/

Response:
```json
{
  "cep": "41275-034",
  "logradouro": "Rua 13 de Maio",
  "complemento": "",
  "bairro": "Campinas de Pirajá",
  "localidade": "Salvador",
  "uf": "BA",
  "unidade": "",
  "ibge": "2927408",
  "gia": ""
}
```

### Diferencial:
 - A página ser responsiva;
 - Permitir edição;
 - Uso de pré-processador css (SASS ou LESS);
 - Usar Rotas para navegação;

### O que esperamos:
 - Padrão de Projeto e boas práticas;
 - Criar uma breve descrição da solução utilizada.
 - Código limpo e legível.
 - Não COPIE!

## Instruções de estilo
 
 - Todo padrão visual fica a seu critério.
 - Disponibilaremos a marcar para download a partir da mesma criar o padrão.
 - O layout precisa ser limpo e usual, pensando sempre na responsividade do mesmo.

