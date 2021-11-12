---
title: 'groupLifecyclePolicy: removeGroup'
description: Remove um grupo de uma política de ciclo de vida.
author: Jordanndahl
ms.localizationpriority: medium
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 90581ea2ea2317363e4043c92e520f2bd379bf59
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60936261"
---
# <a name="grouplifecyclepolicy-removegroup"></a>groupLifecyclePolicy: removeGroup

Namespace: microsoft.graph

Remove um grupo de uma política de ciclo de vida.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Directory.ReadWrite.All    |
|Delegada (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/removeGroup
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome | Descrição |
|:---------------|:----------|
| Autorização | {token} de portador. Obrigatório. |
| Content-Type  | application/json |

## <a name="request-body"></a>Corpo da solicitação
Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro | Tipo | Descrição |
|:---------------|:--------|:----------|
|groupId|Cadeia de caracteres| O identificador do grupo a ser removido da política.|

## <a name="response"></a>Resposta

Quando é bem-sucedido, este método retorna um código de resposta `200 OK`. Se o grupo for removido da política, um `true` valor será retornado no corpo da resposta. Caso contrário, `false` um valor será retornado no corpo da resposta.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação

<!-- {
  "blockType": "ignored",
  "name": "grouplifecyclepolicy_removegroup"
} -->
```http
POST https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}/removeGroup
Content-type: application/json

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

##### <a name="response"></a>Resposta
<!-- { "blockType": "response" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: removegroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

