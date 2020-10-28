---
title: 'canal: completeMigration'
description: Conclua a migração de mensagens externas, removendo o modo de migração de um canal.
localization_priority: Normal
author: laujan
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 894c8353b626b1f4cebe62bd00311533933df5a7
ms.sourcegitcommit: 60ced1be6ed8dd2d23263090a1cfbc16689bb043
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/28/2020
ms.locfileid: "48783027"
---
# <a name="channel-completemigration"></a>canal: completeMigration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Conclua o processo de migração de mensagens removendo `migration mode` de um [canal](../resources/channel.md) de uma equipe. `Migration mode` é um estado especial que impede determinadas operações, como a criação de mensagens e a adição de membros, durante o processo de migração de dados.

Depois que uma solicitação **completeMigration** é feita, não é possível importar mensagens adicionais para a equipe. Você pode adicionar membros à equipe depois que a solicitação retornar uma resposta bem-sucedida.

## <a name="permissions"></a>Permissões

A seguinte permissão é necessária para chamar esta API. Para saber mais, *Confira* [permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissão  |
|:--------------------|:---------------------------------------------------------|
| Delegado (conta corporativa ou de estudante)  | Sem suporte.|
| Delegada (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo | Teamwork.Migrate.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{teamId}/channels/{channelId}/completeMigration
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

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.
<!-- markdownlint-disable MD025 -->
<!-- markdownlint-disable MD022 -->

<!-- {
  "blockType": "request",
  "name": "completeMigration_channel"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{teamId}/channels/{channelId}/completeMigration
```
<!-- markdownlint-disable MD001 -->
<!-- markdownlint-disable MD024 -->
### <a name="response"></a>Resposta

Este é um exemplo de resposta.
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 5793eec6-0e5a-11eb-adc1-0242ac120002
2020-10-14 20:22:11 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "completeMigration_ channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
