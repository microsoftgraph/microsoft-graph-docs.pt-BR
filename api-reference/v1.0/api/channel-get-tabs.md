---
title: Guia obter no canal
description: 'Recupere as propriedades e as relações da guia especificada. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: dedb3350b5e5ec32d26a56e33d01d1de04fdb094
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202902"
---
# <a name="get-tab"></a>Obter guia

Namespace: microsoft.graph



Recupere as propriedades e as relações da guia [especificada](../resources/teamstab.md) em um [canal](../resources/channel.md) dentro de uma [equipe.](../resources/team.md) 

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | TeamsTab.Read.All, TeamsTab.ReadWriteForTeam, TeamsTab.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | TeamsTab.Read.Group *, TeamsTab.ReadWrite.Group*, TeamsTab.Read.All, TeamsTab.ReadWriteForTeam.All, TeamsTab.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All |

> **Observação**: Permissões marcadas com * usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).

> **Observação**: esta API oferece transporte a permissões de administrador. Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.

## <a name="http-request"></a>Solicitação HTTP
```http
GET /teams/{team-id}/channels/{channel-id}/tabs/{tab-id}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte $select e $expand [parâmetros de](/graph/query-parameters) consulta OData para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [tab](../resources/teamstab.md) no corpo da resposta.
## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.
```http
GET https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/tabs/{id}?$expand=teamsApp
```
### <a name="response"></a>Resposta
Este é um exemplo de resposta. 

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade. 
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "tabId",
  "displayName": "My Contoso Tab - updated",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  },
  "teamsApp": {
      "id": "0d820ecd-def2-4297-adad-78056cde7c78",
      "externalId": null,
      "displayName": "Contoso",
      "distributionMethod": "store"
  },
  "sortOrderIndex": "20",
  "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a channel tab",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->

