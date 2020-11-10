---
title: 'equipe: completeMigration'
description: Concluir a migração de mensagens externas, removendo o modo de migração de uma equipe.
localization_priority: Normal
author: laujan
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3422c67c34c62fd037b2acf214c4664b21f83900
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48951483"
---
# <a name="team-completemigration"></a>equipe: completeMigration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Conclua o processo de migração de mensagens removendo `migration mode` de uma [equipe](../resources/team.md). `Migration mode` é um estado especial em que determinadas operações são bloqueadas, como a POSTAgem de mensagens e operações de associação durante o processo de migração de dados.

Depois que uma solicitação **completeMigration** é feita, não é possível importar mensagens adicionais para a equipe. Você pode adicionar membros à equipe depois que a solicitação retornar uma resposta bem-sucedida.

## <a name="permissions"></a>Permissões

A seguinte permissão é necessária para chamar esta API. Para saber mais, confira [permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissão  |
|:--------------------|:---------------------------------------------------------|
| Delegado (conta corporativa ou de estudante)  | Sem suporte.|
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo | Teamwork.Migrate.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{teamId}/completeMigration
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


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "completeMigration_team"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{teamId}/completeMigration
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/completemigration-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/completemigration-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/completemigration-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/completemigration-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

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

<!-- uuid: d945a9a4-0e5b-11eb-adc1-0242ac120002
2020-10-14 20:22:11 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "completeMigration_ team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
