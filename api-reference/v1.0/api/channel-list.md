---
title: Listar canais
description: Recuperar a lista de canais nessa equipe.
author: nkramer
doc_type: apiPageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 87895685781982e054714b2991441250cb1738b3
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202223"
---
# <a name="list-channels"></a>Listar canais

Namespace: microsoft.graph


Recuperar a lista de [canais](../resources/channel.md) nessa [equipe](../resources/team.md).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) | Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All |
|Delegada (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All |

> **Observação**: esta API oferece transporte a permissões de administrador. Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte aos [Parâmetros de consulta OData](/graph/query-parameters) $filter, $select e $expand para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Channel](../resources/channel.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-list-all-channels"></a>Exemplo 1: Listar todos os canais

#### <a name="request"></a>Solicitação

O exemplo a seguir mostra uma solicitação para listar todos os canais.

<!-- {
  "blockType": "request",
  "name": "list_channels"
}-->

```http
GET https://graph.microsoft.com/v1.0/teams/893075dd-2487-4122-925f-022c42e20265/channels
```


#### <a name="response"></a>Resposta

Esta é a resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
    {
      "id": "19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2",
      "createdDateTime": "2020-05-27T19:22:25.692Z",
      "displayName": "General",
      "description": "AutoTestTeam_20210311_150740.2550_fim3udfdjen9",
      "membershipType": "standard"
    }
  ]
}
```

### <a name="example-2-list-all-private-channels"></a>Exemplo 2: Listar todos os canais privados

#### <a name="request"></a>Solicitação

O exemplo a seguir mostra uma solicitação para listar todos os canais privados.


<!-- {
  "blockType": "request",
  "name": "list_private_channels"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/64c323f2-226a-4e64-8ba4-3e6e3f7b9330/channels?$filter=membershipType eq 'private'
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
    {
      "id": "19:982abbfca323a582f0a6d00ae2deca@thread.tacv2",
      "createdDateTime": "2020-05-27T19:22:25.692Z",
      "displayName": "General",
      "description": "test private team",
      "membershipType": "private"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List channels",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
