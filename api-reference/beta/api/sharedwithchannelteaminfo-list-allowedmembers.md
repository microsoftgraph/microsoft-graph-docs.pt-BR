---
title: Listar allowedMembers
description: Obtenha a lista de recursos conversationMember da propriedade de navegação allowedMembers.
author: devjha-ms
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: aa8d70f76656f01fdcda6fc29304e0a1ba29a25e
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/06/2022
ms.locfileid: "64685282"
---
# <a name="list-allowedmembers"></a>Listar allowedMembers
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha a lista de [conversationMembers](../resources/conversationmember.md) que podem acessar um canal [compartilhado](../resources/channel.md).
Esse método não retorna os seguintes [conversationMembers](../resources/conversationmember.md) da [equipe](../resources/team.md):
- Usuários com `Guest` função
- Usuários autenticados externamente no locatário

> [!NOTE]
> A ID de associação retornada pelo servidor deve ser tratada como uma cadeia de caracteres opaca. O cliente não deve tentar analisar ou fazer suposições sobre essa ID.
>
> Os resultados da associação podem ser mapeados para usuários de locatários diferentes, conforme indicado na resposta, no futuro. O cliente não deve presumir que todos os membros são apenas do locatário atual.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante) | ChannelMember.Read.All, ChannelMember.ReadWrite.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | ChannelMember.Read.All, ChannelMember.ReadWrite.All |


> **Observação**: esta API dá suporte a permissões de administrador. Os administradores globais e os administradores de serviços do Microsoft Teams podem acessar equipes das quais não são membros.

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{teamsId}/channels/{channelId}/sharedWithTeams/{sharedWithChannelTeamInfoId}/allowedMembers
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) `$select` e `$count` para personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [conversationMember](../resources/conversationmember.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.
<!-- {
  "blockType": "request",
  "name": "list_conversationmember"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/893075dd-2487-5634-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2/sharedWithTeams/893075dd-2487-5634-925f-022c42e20265/allowedMembers
```


### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.conversationMember",
      "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJkMTQ",
      "roles": [
        "owner"
      ],
      "displayName": "Eric Solomon",
      "userId": "eef9cb36-06de-469b-87cd-70f4cbe32d14",
      "email": "ericsol@fabrikam.com",
      "tenantId": "df81db53-c7e2-418a-8803-0e68d4b88607"
    },
    
    {
      "@odata.type": "#microsoft.graph.conversationMember",
      "id": "MmFiOWMFxTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJkMTQ",
      "roles": [
        "user"
      ],
      "displayName": "Caleb Foster",
      "userId": "eef9cb36-06de-469b-87cd-70f4cbe32d14",
      "email": "calfos@fabrikam.com",
      "tenantId": "df81db53-c7e2-418a-8803-0e68d4b88607"
    }
  ]
}
```

## <a name="see-also"></a>Confira também

- [Listar membros de equipe](team-list-members.md)