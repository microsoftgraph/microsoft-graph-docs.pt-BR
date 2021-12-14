---
title: Listar equipes
description: Listar todas as equipes em uma organização
author: akhilkohlimicrosoft
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8c4a2d90f3c82c7066fee7c98aebbd3ba011c825
ms.sourcegitcommit: c99d3feb3ab5cae506c1f758bc277a637adc9111
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/13/2021
ms.locfileid: "61432738"
---
# <a name="list-teams"></a>Listar equipes

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Liste todas as [equipes](../resources/team.md) em uma organização.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All |
|Delegada (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /teams
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método suporta o  `$filter`, `$select`, `$top`, `$skiptoken`, `$count` [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório. |
| Aceitar  | application/json|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos da[equipe](../resources/team.md) no corpo da resposta.

> [!Note]
> Atualmente, essa chamada à API retorna apenas as propriedades **ID**, **displayName** e **description** de uma [equipe](../resources/team.md). Para obter todas as propriedades, use a operação[Obter equipe](../api/team-get.md). 

## <a name="examples"></a>Exemplos

### <a name="example-1-get-a-list-of-teams"></a>Exemplo 1: Obter uma lista de equipes

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "get_teams"
}-->
```http
GET https://graph.microsoft.com/beta/teams
```
---

#### <a name="response"></a>Resposta
Veja a seguir um exemplo de uma resposta.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "172b0cce-e65d-44ce-9a49-91d9f2e8493a",
      "displayName": "Contoso Team",
      "description": "This is a Contoso team, used to showcase the range of properties supported by this API"
    },
    {
      "id": "890972b0cce-e65d-44ce-9a49-568hhsd7n",
      "displayName": "Contoso General Team",
      "description": "This is a general Contoso team"
    },
    ,
    {
      "id": "98678abcce0-e65d-44ce-9a49-9980bj8kl0e",
      "displayName": "Contoso API Team",
      "description": "This is Contoso API team"
    }
  ]
}
```

### <a name="example-2-use-filter-and-top-to-get-two-teams-with-a-display-name-that-starts-with-a"></a>Exemplo 2: use $filter e $top para obter duas equipes com um nome de exibição que começa com 'A'

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "get_teams"
}-->

```http
GET https://graph.microsoft.com/beta/teams?$filter=startswith(displayName, 'A')&$top=2
```


#### <a name="response"></a>Resposta

Veja a seguir um exemplo de uma resposta.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "172b0cce-e65d-44ce-9a49-91d9f2e8493a",
      "displayName": "A Contoso Team",
      "description": "This is a Contoso team, used to showcase the range of properties supported by this API"
    },
    {
      "id": "890972b0cce-e65d-44ce-9a49-568hhsd7n",
      "displayName": "A Contoso Notification Team",
      "description": "This is a notification Contoso team"
    },
  ]
}
```

### <a name="example-3-use-filter-and-select-to-get-id-and-description-for-team-with-displayname-equals-a-contoso-team"></a>Exemplo 3: use $filter e $select para obter id e descrição para a equipe com displayName igual a "Uma Equipe Contoso"

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "get_teams"
}-->
```http
GET https://graph.microsoft.com/beta/teams?$filter=displayName eq 'A Contoso Team'&$select=id,description
```
---

#### <a name="response"></a>Resposta
Veja a seguir um exemplo de uma resposta.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "172b0cce-e65d-44ce-9a49-91d9f2e8493a",
      "description": "This is a Contoso team, used to showcase the range of properties supported by this API"
    }
  ]
}
```


## <a name="see-also"></a>Confira também
- [Obter equipe](../api/team-get.md)