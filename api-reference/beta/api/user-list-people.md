---
title: Listar pessoas
description: Recupere uma lista de objetos de pessoa ordenados por sua relevância para o usuário, que é determinado pelo relacionamentos de negócios e os padrões de colaboração e comunicação do usuário.
author: simonhult
localization_priority: Normal
ms.openlocfilehash: 3bd9c8cdd3737cbd8d96fd4f9b24f5382ce04793
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872776"
---
# <a name="list-people"></a>Listar pessoas

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Recupere uma lista de objetos de [pessoa](../resources/person.md) ordenados por sua relevância para o [usuário](../resources/user.md), que é determinado pelo relacionamentos de negócios e os padrões de colaboração e comunicação do usuário.

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | People.Read    |
|Delegado (conta pessoal da Microsoft) | People.Read    |
|Aplicativo | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Esse método suporta os seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.

|Nome|Valor|Descrição|
|:---------------|:--------|:-------|
|$filter|string|Limita a resposta apenas às pessoas cujo registro contém os critérios especificados.|
|$orderby|string|Por padrão, as pessoas na resposta são classificadas pela relevância delas à consulta. Você pode alterar a ordem das pessoas na resposta usando o parâmetro *$orderby*.|
|$search|string|Pesquisar pessoas por nome ou alias. Suporta correspondência difusa. Parâmetro funciona apenas para a pesquisa de pessoas de relevantes do usuário conectado, não para pesquisar pessoas relevantes para outros usuários. Também oferece suporte a `topic` palavra-chave para localizar pessoas com base em tópicos extraídos de conversas de email com essa pessoa. Consulte a seção de *executar uma pesquisa difusa* em [obter as informações relevantes sobre pessoas](/graph/people-example#perform-a-fuzzy-search) para obter informações e exemplos.|
|$select|string|Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.|
|$skip|int|Ignorar os primeiros n resultados, útil para paginação. Não é suportado ao usar *$search*.|
|$top|int|Número de resultados a ser retornado.|

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização  | {token} de portador. Obrigatório. |
| Aceitar | application/json |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos da [pessoa](../resources/person.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="browse"></a>Procurar

As solicitações nesta seção obtém as pessoas importantes para o usuário conectado (`/me`), com base na comunicação, colaboração e relacionamentos de negócios.

Por padrão, cada resposta retorna 10 registros, mas você pode alterar esse número usando o parâmetro *$top*. Essas solicitações exigem a permissão People.Read.

#### <a name="request"></a>Solicitação

O exemplo a seguir é um exemplo da solicitação padrão.
<!-- {
  "blockType": "request",
  "name": "get_person_collection_beta"
}-->

```http
GET https://graph.microsoft.com/beta/me/people
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.
>**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "name": "get_person_collection_beta",
  "truncated": true,
  "@odata.type": "microsoft.graph.person",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1326

{
    "value": [
        {
            "id": "33b43a5b-87d6-41ec-91f8-a2610048105f",
            "displayName": "Marketing",
            "givenName": null,
            "surname": null,
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "title": null,
            "companyName": null,
            "yomiCompany": "",
            "department": null,
            "officeLocation": null,
            "profession": "",
            "mailboxType": "GroupMailbox",
            "personType": "ModernGroup",
            "userPrincipalName": "",
            "emailAddresses": [
                {
                    "address": "Marketing@contoso.com",
                    "rank": 30
                }
            ],
            "phones": [],
            "postalAddresses": [],
            "websites": [],
            "sources": [
                {
                    "type": "Directory"
                }
            ]
        },
        {
            "id": "e3d0513b-449e-4198-ba6f-bd97ae7cae85",
            "displayName": "Isaiah Langer",
            "givenName": "Isaiah",
            "surname": "Langer",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "title": "Web Marketing Manager",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "20/1101",
            "profession": "",
            "mailboxType": "Mailbox",
            "personType": "Person",
            "userPrincipalName": "IsaiahL@contoso.com",
            "emailAddresses": [
                {
                    "address": "IsaiahL@contoso.com",
                    "rank": 20
                }
            ],
            "phones": [
                {
                    "type": "business",
                    "number": "+1 918 555 0101"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "sources": [
                {
                    "type": "Directory"
                }
            ]
        }
    ]
}
```

#### <a name="requesting-a-subsequent-page-of-people"></a>Solicitação de uma página subsequente de pessoas

Se a primeira resposta não contiver a lista completa das pessoas relevantes, você poderá fazer uma segunda solicitação usando *$top* e *$skip* para solicitar páginas adicionais de informações. Se a solicitação anterior tiver informações adicionais, a solicitação a seguir obterá a próxima página de pessoas do servidor.

```http
GET https://graph.microsoft.com/beta/me/people/?$top=10&$skip=10
```

#### <a name="sort-the-response"></a>Classificar a resposta

Por padrão, as pessoas na resposta são classificadas pela relevância delas à consulta. Você pode alterar a ordem das pessoas na resposta usando o parâmetro *$orderby*. Essa consulta seleciona as pessoas mais relevantes para você classificando-as pelo nome de exibição e retorna as dez primeiras pessoas da lista classificada.

```http
GET https://graph.microsoft.com/beta/me/people/?$orderby=DisplayName
```

#### <a name="changing-the-number-of-people-returned-and-the-fields-returned"></a>Alteração do número de pessoas e dos campos retornados

Você pode alterar o número de pessoas retornadas na resposta definindo o parâmetro *$top*.

O exemplo a seguir solicita as 1.000 pessoas mais relevantes para `/me`. A solicitação também limita a quantidade de dados enviados pelo servidor, solicitando apenas o nome para exibição da pessoa.

```http
GET https://graph.microsoft.com/beta/me/people/?$top=1000&$select=DisplayName
```

#### <a name="selecting-the-fields-to-return"></a>Seleção dos campos que devem ser retornados

Você pode limitar a quantidade de dados retornadas do servidor usando o parâmetro *$select* para escolher um ou mais campos. O campo *@odata.id* é sempre retornado.

O exemplo a seguir limita a resposta à *DisplayName* e *EmailAddress* das pessoas mais relevantes 10.

```http
GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses
```

#### <a name="using-a-filter-to-limit-the-response"></a>Uso de um filtro para limitar a resposta

Você pode usar o parâmetro *$filter* para limitar a resposta apenas às pessoas cujo registro contém os critérios especificados.

A seguinte consulta limita a resposta às pessoas com a fonte "Diretório".

```http
GET https://graph.microsoft.com/beta/me/people/?$filter=Sources/Any (source: source/Type  eq 'Directory')
```

#### <a name="selecting-the-fields-to-return-in-a-filtered-response"></a>Selecionar os campos para retornar em uma resposta filtrada

Você pode combinar os parâmetros *$select* e *$filter* para criar uma lista personalizada de pessoas relevantes para o usuário e obter somente os campos necessários para seu aplicativo.

O exemplo a seguir obtém o *DisplayName* e *EmailAddress* de pessoas cujo nome de exibição é igual ao nome especificado. Neste exemplo, somente as pessoas cujo nome de exibição é igual a "Nestor Kellum" são retornadas.

```http
+GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses&$filter=DisplayName eq 'Nestor Kellum'
```

### <a name="search-people"></a>Pesquisar pessoas

As solicitações nesta seção também obtêm as pessoas importantes para o usuário conectado (`/me`). Solicitações de pesquisa exigem a permissão People.Read.

#### <a name="using-search-to-select-people"></a>Usando a pesquisa para selecionar as pessoas

Use o parâmetro *$search* para selecionar as pessoas que atendem a determinado conjunto de critérios.

A seguinte consulta de pesquisa retorna pessoas relevantes para `/me` cujos GivenName ou sobrenome começa com a letra "j".

```http
GET https://graph.microsoft.com/beta/me/people/?$search=j
```

#### <a name="using-search-to-specify-a-relevant-topic"></a>Uso da pesquisa para especificar um tópico relevante

A solicitação a seguir retorna a pessoas relevantes para `/me` cujos nomes contêm "ma" e que têm uma associação com "planejamento do recurso".

```http
GET https://graph.microsoft.com/beta/me/people/?$search="ma topic: feature planning"
```

#### <a name="performing-a-fuzzy-search"></a>Execução de uma pesquisa difusa

A solicitação a seguir faz uma pesquisa de uma pessoa chamada "Saguão Hermaini." Como há uma pessoa chamada "Herminia Hull" relevantes para o usuário conectado, as informações de "Herminia Hull" são retornadas.

```http
GET https://graph.microsoft.com/beta/me/people/?$search="hermaini hall"
```

### <a name="related-people"></a>Pessoas relacionadas

A solicitação a seguir obtém as pessoas importantes para outra pessoa na organização do usuário. Esta solicitação requer o User.ReadBasic.All para People.Read.All permissão. Neste exemplo, as pessoas de relevantes do Nestor Kellum são exibidas.

```http
GET https://graph.microsoft.com/beta/users('nestork@contoso.com')/people/
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
