---
title: 'groupLifecyclePolicy: addGroup'
description: Adiciona um grupo a uma política de ciclo de vida.
author: Jordanndahl
ms.localizationpriority: medium
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a5deab02460562f527cd1566769cf9d75b16858e
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60937241"
---
# <a name="grouplifecyclepolicy-addgroup"></a>groupLifecyclePolicy: addGroup

Namespace: microsoft.graph

Adiciona grupos específicos a uma política de ciclo de vida. Essa ação limita a política de ciclo de vida do grupo a um conjunto de grupos somente se a propriedade **managedGroupTypes** do [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) estiver definida como `Selected` .

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
POST /groupLifecyclePolicies/{id}/addGroup
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
|groupId|Cadeia de caracteres| O identificador do grupo a ser acrescentado à política. |

Quando a **propriedade managedGroupTypes** [do groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) é definida como , você pode adicionar até `Selected` 500 grupos à lista. Se você precisar adicionar mais de 500 grupos, a propriedade **managedGroupTypes** do [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) deve ser definida como `All` .

Somente um grupo pode ser adicionado por solicitação.

## <a name="response"></a>Resposta

Quando é bem-sucedido, este método retorna um código de resposta `200 OK`. Se o grupo for adicionado à política, um `true` valor será retornado no corpo da resposta. Caso contrário, `false` um valor será retornado no corpo da resposta.

## <a name="example"></a>Exemplo

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "ignored",
  "name": "grouplifecyclepolicy_addgroup"
} -->
```http
POST https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}/addGroup
Content-type: application/json

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

#### <a name="response"></a>Resposta
<!-- { "blockType": "ignored" } -->

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
  "description": "groupLifecyclePolicy: addgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

