---
title: 'channel: completeMigration'
description: Conclua a migração de mensagens externas removendo o modo de migração de um canal.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 150bb921c87bcd0ea62d7218315f79e791a170fe
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51207565"
---
# <a name="channel-completemigration"></a>channel: completeMigration

Namespace: microsoft.graph

Conclua o processo de migração de mensagens removendo `migration mode` de [um canal](../resources/channel.md) em uma equipe. `Migration mode` é um estado especial que impede determinadas operações, como o envio de mensagens e a adição de membros, durante o processo de migração de dados.

Depois que **uma solicitação completeMigration** for feita, você não poderá importar mensagens adicionais para a equipe. Você pode adicionar membros à equipe após a solicitação retornar uma resposta bem-sucedida.

## <a name="permissions"></a>Permissões

A permissão a seguir é necessária para chamar essa API. Para saber mais, *confira* [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissão  |
|:--------------------|:---------------------------------------------------------|
| Delegado (conta corporativa ou de estudante)  | Sem suporte.|
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo | Teamwork.Migrate.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/channels/{channel-id}/completeMigration
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
POST https://graph.microsoft.com/v1.0/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/completeMigration
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
