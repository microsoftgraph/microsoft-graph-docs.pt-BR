---
title: Excluir Guia do canal
description: 'Remove (desafixa) uma guia do canal especificado de uma equipe. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 82fc54c629246bcf421a7c79d346ae3b9e54dce6
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607290"
---
# <a name="delete-tab-from-channel"></a>Excluir Guia do canal

Namespace: Microsoft Graph



Remove (desafixa) uma guia do [canal](../resources/channel.md) especificado de uma [equipe](../resources/team.md). 

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) |  TeamsTab. ReadWriteForTeam, TeamsTab. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | TeamsTab. Delete. Group *, TeamsTab. ReadWriteForTeam. All, TeamsTab. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All |

> **Observação**: Permissões marcadas com * usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).

> **Observação**: esta API oferece transporte a permissões de administrador. Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{team-id}/channels/{channel-id}/tabs/{tab-id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <a name="example"></a>Exemplo
#### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a>Resposta
Este é um exemplo de resposta. Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete tab from channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->

