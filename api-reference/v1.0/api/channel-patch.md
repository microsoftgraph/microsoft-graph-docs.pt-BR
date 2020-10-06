---
title: Canal de patch
description: Atualiza as propriedades do canal especificado.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 66d4815220d77e0f7189bf876c32eb043e032c7c
ms.sourcegitcommit: 39e48ed2d95b142ccf3f40ecc52441458f2745bf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/06/2020
ms.locfileid: "48364282"
---
# <a name="patch-channel"></a>Canal de patch

Namespace: microsoft.graph

Atualiza as propriedades do [canal](../resources/channel.md)especificado.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | ChannelSettings. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | ChannelSettings. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All |

> **Observação**: esta API oferece transporte a permissões de administrador. Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}/channels/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornça uma representação JSON do objeto [canal](../resources/channel.md).

> **Observação:** Não é possível atualizar o `membershipType` valor de um canal existente.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.

```http
PATCH https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}
```

<!-- {
  "blockType": "request",
  "name": "update_channel"
}-->

### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Patch channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
