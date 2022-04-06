---
title: 'groupLifecyclePolicy: removeGroup'
description: Remove um grupo de uma política de ciclo de vida.
author: psaffaie
ms.localizationpriority: medium
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 55444e29c4fa35e561122412d66b2efcd13176ad
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64588376"
---
# <a name="grouplifecyclepolicy-removegroup"></a>groupLifecyclePolicy: removeGroup

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Remove um grupo de uma política de ciclo de vida.

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
| :------------------------------------- | :------------------------------------------ |
| Delegado (conta corporativa ou de estudante)     | Directory.ReadWrite.All                     |
| Delegado (conta pessoal da Microsoft) | Sem suporte                               |
| Aplicativo                            | Directory.ReadWrite.All                     |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /groupLifecyclePolicies/{id}/removeGroup
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição               |
| :------------ | :------------------------ |
| Autorização | {token} de portador. Obrigatório. |
| Content-Type  | application/json          |

## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro | Tipo   | Descrição                                            |
| :-------- | :----- | :----------------------------------------------------- |
| groupId   | Cadeia de caracteres | O identificador do grupo a ser removido da política. |

## <a name="response"></a>Resposta

Quando é bem-sucedido, este método retorna um código de resposta `200 OK`. Se o grupo for removido da política, um `true` valor será retornado no corpo da resposta. Caso contrário, um `false` valor será retornado no corpo da resposta.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação

<!-- {
  "blockType": "ignored",
  "name": "grouplifecyclepolicy_removegroup"
} -->

```http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}/removeGroup
Content-type: application/json

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

##### <a name="response"></a>Resposta

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
<!--
{
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: removegroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
